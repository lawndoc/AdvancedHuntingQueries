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

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA-1Wy47TQBDsMxL_YJlLVoq0cEaLtJAVRDwurMIBcTCOk5h14sieJBjx8dTUzPidB0QRB9Bq43l2d3VXzcy1XIsnI4lE4T-TpcSyQivH6E4WHF9wxsNvICF6nmw5kmNtitUefmecN-MF2mt8U5njN4BNj1Y9zKSysbZWWB1z1QordF9xXU77G0kYh97_Fe1Ihtz1HZZT9FOsVI25lHb1nriM-bE8Aj6N8B5rHyyumL5StDSekDEZ7wu0d_guMbMijilRxVhl9i4wo1Eez0bQyUIVzcvS9gwzGqsihnY8M4sqwIoE31cykTt88zLXGmvM2LT1hPXy5GPPvCc39FnAdsA6hzKQz-LDqlsX0pPPWHx5g5E5ELr-e9iZYmyD3W7sHTPmyxe5kuc1hK9tJC5yjXXNuhW0ojHoPCnsDuA_6uRRR6yYb9XIu-knzH_O9rMexsToaUxFIy-TlodPlismry5Ho1rN79FaIp_NWCd7vFWV-EnMMSPUfAttXZp2PrAShr9dH_VYh6y-zsAYdp2Hb9SB5twDv1PEn5BViixSVrnnInoLxnqW3VUUHv5Mtde0kXP31rItt9gq1jp1JGRD1lNxh2tn9RuxZvsq22R5AS6aflKeN4NeJVyVfnJyeckcxPKjFq3jQqXGAfZ58F-cVce_qRFzerqz8xRd3DV2_NfHv6aPup8xZpp8uMXOgP7cPaz5cUO2HVJYm1X9di6rvds9N-2T8v5u3_w7q4n6zX9Mn0NGnTHbc2a9rnfFt0H1wjIvgBWZE9JeQIa6t0TMdkidZ1bBx5k75ksrsm-ezN6I-2ozaqG-RB1-V53Hb22jnD-PqK3UbUOp3TPXccFEuf_10TzvzsXbPY0vjfsQqm4WolZ8DrceV2Tg9Mh5pcj4Tcm8GLHPwLpTTowX-H9qX6UVMyrVtm2YF6zzUO04bMdh7bfmI_dp7Q3hQy-HXxvtbGgsh2vmcmOsDVqKrfR5Wp5dbJmtj2GgOWuqk-YX4ss2QCYOAAA&timeRangeId=week) [Vulnerability Percentages](VulnerabilityPercentages.kusto)
- Pie Chart for your viewing pleasure
- Determines whether each version of every program in your environment is vulnerable, expoloitable, or neither
- Takes into account how many devices have each version of a program
- By default, account for all CVE severities