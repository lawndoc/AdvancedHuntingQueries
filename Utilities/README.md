# Utility Hunting Queries

Clicking on the name of the query will bring you to the file for it in this git repo.

***Or try them out right away in your M365 Security tenant:***

Click on the '🔎' hotlink to plug the query right into your Advanced Hunting Query page

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA-1UwU4CMRCds4n_sOGCJiYkeuZAEBMTVA4azsuyC6sLJbugYozf7ptHy1qyKkbhZDbddl6nb6Zv2jakIYHMxcgMfSQhxrGMYOeSYlQAfcJoLmOMQlnIkFYAW_tCDuVAzuH5CDtC38Eolul67pUMY2A5WiAteM3ha-BzK0vEVbQAFsJDV5Xx6vAugNbJFNgvxMrhp0wxZzdZXN4x-vo6rwL4BF_I3b5wfRt8C-YfSJOaOPtIjmEPEKk6dslquBPnWzKqh7aGp3oCnsxqPWL-qlVI_imQf92_1v0E-IXV8BqckzVmgA2pQI96jn9cowy4kQfu_qP65a3QGumscmo2EZCENdm8T8tva6Yxt6tbU97wr9k6dfEP0QrsI6fWK9YUaIZVypbA9utR-1XMGzAmdh9t6qBa9zBjiGk2u4tneH5a8JztPfoVVI0Yqc_qn8kpM0mRieqd7TC2v8NLrLrnmXMcfxm3h38sz-TvQ-10L0rf8eTmYCwsX8fmsOBbNeA9r4qo0WbMy2kSeLfNfxu2ey8UV5VTe5vcm-zvv4ptm1XV8Xwvd9ZXr2-XTLG8A6xR9Hm4BwAA&timeRangeId=week) [ASR Audit Hits](ASRAuditHits.kusto)
- Attack Surface Reduction (ASR) rules in Audit mode generate events that would be blocks in Block mode
- View ASR audit hits to build your exceptions before putting rules in block mode
- There are 3 queries in this kusto file:
    - All categories with audit hits, sorted by hit count
    - All files with audit hits, sorted by hit count
    - Individual process information for audit hits in a single category (uncomment category)

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA6VVTW_TQBCdMxL_werJlgIVHEEcUppCUJUgnIgDqqo02aSunDiynUJRfzxv3q63dmq3BLTy7mR2Pt7MzkyO5VgCGchIJti_gR6CPpMxqDGoQKYS8ybEGUH6M_gxpGPHsRoTakxwO8B5gv0cnO-gz3Gv8i_lBbTV21xmssF5JQa70nfkZrIGL8HvmZQ4M0plssR-jbMAV-_W0CukB-4Op5F8j2tAz6Cf0voCK-dd4SViYDp1dIbbQPryG9ZUrg8kimUHq6WTU-wp7krqGljNIXONXx_wLYDfIkjADeWHHGFdIDfva1EreiNbUG_knYs3p8eU8dpcpERdRVu4_CxwJtgNMSX8jMN1CuqWng3QbpCtjPx7IktoR3M6J_q69MhlrcdXymSFZaAzhvTUZbbwtrb4lckNuE9b-sg85g7rgx2bqy1zp7xL2Cr4xuET3iPvfw1vr6C9xUpZMd2ebOWE1A3c-lv8lR2Lt8vHa0_XdW1dPacZ8y0VW3Rwdqd7FW99la5ecr70CpFXchG1NKdfiWXtvHfp2QgecN1AImE2h436u_O1VmX7sY-22n_L2l-yO0uX56XrwRJ1rxGtcHtLXwFO7Ymdr3bF9JNyOWXb8qT9M4P8pZ8tYaNro0ZdVKuaA_XuH2MeVW8ydF24Ocje4_c61MLAT7N-Y5b9T5Rt9dCN654z9Rffy86iM-RHJ9WoUYW2kuacZqF88q9Yr98jfrZXdrW8RP8ws_ZRKO8LIrzCv43WaOp4XRls66f2buk9Wxl_ADEwGPJIBwAA&timeRangeId=week) [Identity Correlation](IdentityCorrelation.kusto)
- Enter any number or combination of the following fields:
    - Hostname
    - Username
    - EmailAddress
    - SID
    - AzureAccountID
- Query will fill in the fields you don't know for each unique identity and fetch each person's Job Title
- Only needs minimum of 1 value for any 1 field
