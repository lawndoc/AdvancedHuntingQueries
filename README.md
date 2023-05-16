# AdvancedHuntingQueries
My collection of Microsoft 365 Advanced Hunting Queries written in Kusto Query Language (KQL). My queries are public domain ([Unlicense](LICENSE)), but I'd appreciate a credit/tag if you republish them somewhere.

This repo includes '🔎' icons with hotlinks that plug the queries right into your M365 Security tenant.

Click on a category to start exploring my hunting queries!

## Query Categories:

### [📈 Anomalies](Anomalies)

- Identify the most significant spikes in various activities

### [🛡️ ASR Rules](ASR)

- Queries that help you build your [Attack Surface Reduction](https://learn.microsoft.com/en-us/microsoft-365/security/defender-endpoint/attack-surface-reduction) policies

### [⚠️ Detection Rules](Detection-Rules)

- Kusto queries that can be turned into detection rules to create alerts

### [💣 Exploits](Exploits)

- Hunt for specific exploits being used in your environment

### [🕵️ Incident Response](Incident-Response)

- Hunt for known IOCs and activity from compromised hosts

### [🎣 Phishing](Phishing)

- Identify potential phishing emails in your environment

### [📝 Rough Drafts](Rough-Drafts)

- Detection rules I've written that are useful for hunting but not ready to generate alerts

### [🏰 Security Posture](Posture)

- Highlight bad operational security practices

### [🧑 User Behavior](User-Behavior)

- Queries related to user activity -- not all of them are relevant to security

### [🛠️ Utilities](Utilities)

- Useful queries that help with identity correlation, metrics, policy building, etc.

---

## Crafting your own queries

### Getting started

To get better at KQL, the best starting place is to just __explore the data__. By exploring the data, your curiosity can lead you down rabbit holes of "how can I find this?" It also helps you understand the data. __You can't make your own hunting queries if you don't know what information you have available to you__.

Choose a table like `DeviceEvents` and take a sample of just 10 random events with `take 10`. This will give you an idea of what data is in that table.

```
DeviceEvents
| take 10
```

I find the `distinct` operator useful for identifying the values I can expect to find in a specific column. That will give me an idea of the ways that I can filter out data or only show specific things.

```
DeviceEvents
| distinct ActionType
```

When troubleshooting a query that isn't giving you want you want, the first thing you need to do is identify *which line* is wrong. Injecting `take 10` or a `where` filter and then a __blank line__ will allow you to check for values you would expect to see or not see.

```
DeviceProcessEvents
| where ProcessCommandLine contains "iex"
| take 10  // the blank line below will end this 3-line query

| summarize Count = count() by InitiatingProcessFileName  // this line won't execute because of the blank line above
```

To clean up the output, you can hide columns you don't care about with `project`, `project-away`, and `project-reorder`. It's also helpful to `sort` by a column like `Timestamp` or `Count`. Having an easily digestible output is as important as the query itself.

Try the below queries with and without `project` and `sort`

```
DeviceProcessEvents
| where FileName contains "whoami"
| project Timestamp, DeviceName, AccountName, FileName, InitiatingProcessCommandLine
```

```
DeviceProcessEvents
| where FileName == "cmd.exe"
| summarize Count = count() by AccountName
| sort by Count desc
```
