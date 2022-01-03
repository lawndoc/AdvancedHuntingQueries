# Security Posture Hunting Queries

Clicking on the name of the query will bring you to the file for it in this git repo.

***Or try them out right away in your M365 Security tenant:***

Click on the '🔎' hotlink to plug the query right into your Advanced Hunting Query page

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA22QywqCUBCG_3XQOxxcGbhvVRDVIoho4QuYSQneSLvSw_c5hbaQYXSY__yXczY6KlGhRin91FalTnShtW4_pNZYI73ldNeZ3YV2CmHkTDUnIqaK3ZyOjO9rivJkkNl7hDhWtptRTh7YSgvtmWNlIBGchv-Dr2fqBboO75qpNKz1brP7MGOq1NVy7yxX8peiBsmpVjXVy5yX3XlnGXq-D9PpgLIjVcJ7pKBJpxuwH3b8IhWVGSey921vHAze_wPAk99NhgEAAA&timeRangeId=week) [Cleartext LDAP Logins](CleartextLDAP.kusto)
- Files with the substring "password" in the name
- Results probably contain users' passwords in plain text
- Included file extensions: .doc .docx .xls .xlsx .txt

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA62STQ6CMBCF39rEOzSu_TmDCZq4MWw8AKFEmiA1FoSFh_fN8KNxpcFMyMDrm68tMxEy3OGQMu-ZC-YdlQwlKgTMMcMDBg1yajc-ZvQdkeCiSgqv_oQrJasMFrjyKzAart1gqXzHkp2t1jkSc2WtqXju0jHMGEL-ldFOpLR0hb8wpp6kIqHqGRuGwUrDsM4ypK7ljQvUrHXaI-nN6-93fqkdemPpC6RKH1Nmg-htQoYTLakf6HDqTHr_GTG5Xp3S-S3fZDJqnY0TJ6LUys_7dZqnZvVksRJzPAEo8phwnAIAAA&timeRangeId=week) [Files With Passwords](FilesWithPasswords.kusto)
- Files with the substring "password" in the name
- Results probably contain users' passwords in plain text
- Included file extensions: .doc .docx .xls .xlsx .txt