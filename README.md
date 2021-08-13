# AdvancedHuntingQueries
Microsoft 365 Defender Advanced Hunting Queries written in Kusto Query Language (KQL)

## Queries:
### [AnomalousLogonTimeline](AnomalousLogonTimeline.kusto)
- Gets the top 5 users whose logons had the most anomalous spike and projects their daily logins onto a timechart for visual aid
- Service accounts showing up in this query are especially suspicious

### [EmailsWithOAuthRequests](EmailsWithOAuthRequests.kusto)
- Hunt for potential phishing emails that link to a Microsoft OAuth login
- OAuth tokens can grant the 3rd party permissions without stealing credentials
- Logins take place on login.windows.net or login.microsoftonline.com which is less suspicious

### [Exfiltration](Exfiltration.kusto)
- Non-browser uploading data to Mega cloud storage
- Rclone sync tool (low-confidence malicious activity)
- Renamed Rclone sync tool (high-confidence malicious activity)

### [PhishDelivered](PhishDelivered.kusto)
- Detects high-confidence phishing or malware emails that were delivered to one or more mailboxes

### [SeriousSAM](SeriousSAM.kusto)
- Hunt for potential exploitation of [SeriousSAM](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2021-36934)

### [UserAndHostCorrelation](UserAndHostCorrelation.kusto)
- Find all users currently logged in on a given host
- Find all hosts that a given user is currently logged into
