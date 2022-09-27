# Utility Hunting Queries

Clicking on the name of the query will bring you to the file for it in this git repo.

***Or try them out right away in your M365 Security tenant:***

Click on the '🔎' hotlink to plug the query right into your Advanced Hunting Query page

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA72WXUvrQBCG51o4_0G8Fgp67UWpCoIfxc_rmKRNNbUhm1oPHPztPvMm7bGlgmAiS5LZ-XpnZ3dm07Oe7drcXiy2mU0ZKXQFb8Y35ZvbpKEi8SOeCt5UvAo915kxnlc6GfLKAtRCVCYftW2wAssYzognhhPLKrUxPkr7a39sx46Zv0qe2glUHVWQrMf4J98Z_FJx9NH0qDzqW3wU4h7ZO-89pAG9viXIH5Fc80TM3Hqg6HJmQ2YzIQZGn6wkij7lu_cj5BN705rnaEZEkGtVU2hHHsi2atbYNe4VeR81me0O-Zx3pDwOZJU0GBO4OVbubdQy5hUrHOEvrE5UYjfQJXZF61ifs9j9CdrcNa_UPprFr6NfkNtYSA-q6kM7UCQTIvG9zTvEXl_hGVZPOt9LH23iDqUd0ApNhTiun1yPYU63ysjAFHm7qAFuXbW199_Y32t27gXKz9UC2i3b9P-5Crf1pGOsF9j7PeJ9uU3sO_WdUn2h9rctgm4R76AeO9y_e3zluqXL1YpusBmLl5Bfz_6r5O3gLm8OX1EuvMRORScNSrxa6b285OrJX9ep4xfyt6zp3bW_gEvs_Z9jH_6pKmKT9x99KKxMfO8Sk-bmqdSxxhs7sc3bd6y2461rLXu111fCrVj_S30ApogSEnYJAAA&timeRangeId=week) [ASR Single Rule Audit Hits](ASRSingleRuleAudits.kusto)
- Attack Surface Reduction (ASR) rules in Audit mode generate events that would be blocks in Block mode
- View ASR audit hits to build your exceptions before putting rules in block mode
- Query shows individual process information for all audit hits in a single rule

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA5VQQQrCMBCcs-AfcquC4As8iNqjeBDvtQ200BoxqUXx8c6uNBXRgywh2dnZ2dmsYXFFhZz3hi-LEwI8xhjhAYMOJbELj8GSrECuI2ePG86KemIZGdLVsRrYYZCQ7YkmqjRnmBiO-L9qK-UFVhxqhkWBVN-F-hM12cEzDqpaU6fXf7no52dEip8OrFY_d2mJSS5zk_g7nnjDEMcV7tovTlv1arDgyWM-wZT5kZO-z54RT4nJdltqNhEb9tzpVuWbA6e_1esO05_taNCO2gEAAA&timeRangeId=week) [ASR Top Files Audited](ASRTopFiles.kusto)
- Top files triggering ASR rules, sorted by number of audit hits
- Each file is displayed with which rule it is triggering

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA5VRywrCMBCcs-A_5FY99Qs8iI8vEO-xDVaoRppUUfx4JyNtUfQgS9nd2cnsozlyGER4nOkLWMYOe-YNDowC0SujiIqRRYtSmWGefMAYIyzJvDAv6FeMHE597SGFiljDz2BOViTXk7PBjX0TGohZMtKroV9GdiCaScn0lqb7V2khXmTFo6Y5brJWXGq2pFZo44CtVGtd46X_PoElUv6cwKn6uUd3udQ36y8TiB9pVve-632atNWsBjP9lS6fYMp8x07few-qXhfouIPiE2X_VBHwAQAA&timeRangeId=month) [ASR Top Rules Audited](ASRTopRules.kusto)
- Top ASR rules being triggered, sorted by number of audit hits

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA5WTQU8CMRCF39nE_9B4QRL_AgcjavQgJng3C1RA2V3CLhKMP95vpmyWKCSSZtP2zbw3b9puX1GfmmvMfMsqqlCtSuc607eCNpqBrfiCrsmqyS3JedFWS0crsIwMY22I1jCCOmRXoB1XCruRwZwcVYoe_a2yBrN9ZO6c4Gvse_M2Z65cbaA3Ruq21aqokTOsi7m-nH0De-38oN5OLe0v1dWVZ2TuakrEeNFrWK4pfbB_BYnOOOSwS-aIdVB_7w6e4ObMVmFA9rP3mGtIfIK6KbVeEtr08Q5uvQY9gKabtJPbsi_ouyRSevyvcqOxBC1Riu74uLc7HCwYDdbzd7AiL_OO7-Gk17TPuvDPVkP4K6Iplk70kcojzsc8L3aM9h6OnXnj3F5J5R0XJ3r_X-2aXerRKkzp8ZCb7t6rKv2vaG65VfsBONLn1nQDAAA&timeRangeId=week) [ASR Top Users Audited](ASRTopUsers.kusto)
- Top users triggering ASR rules, sorted by number of audit hits
- Each user is displayed with which rule(s) they are triggering, their job title, and device name

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA6VVTW_TQBCdMxL_werJlgIVHEEcUppCUJUgnIgDqqo02aSunDiynUJRfzxv3q63dmq3BLTy7mR2Pt7MzkyO5VgCGchIJti_gR6CPpMxqDGoQKYS8ybEGUH6M_gxpGPHsRoTakxwO8B5gv0cnO-gz3Gv8i_lBbTV21xmssF5JQa70nfkZrIGL8HvmZQ4M0plssR-jbMAV-_W0CukB-4Op5F8j2tAz6Cf0voCK-dd4SViYDp1dIbbQPryG9ZUrg8kimUHq6WTU-wp7krqGljNIXONXx_wLYDfIkjADeWHHGFdIDfva1EreiNbUG_knYs3p8eU8dpcpERdRVu4_CxwJtgNMSX8jMN1CuqWng3QbpCtjPx7IktoR3M6J_q69MhlrcdXymSFZaAzhvTUZbbwtrb4lckNuE9b-sg85g7rgx2bqy1zp7xL2Cr4xuET3iPvfw1vr6C9xUpZMd2ebOWE1A3c-lv8lR2Lt8vHa0_XdW1dPacZ8y0VW3Rwdqd7FW99la5ecr70CpFXchG1NKdfiWXtvHfp2QgecN1AImE2h436u_O1VmX7sY-22n_L2l-yO0uX56XrwRJ1rxGtcHtLXwFO7Ymdr3bF9JNyOWXb8qT9M4P8pZ8tYaNro0ZdVKuaA_XuH2MeVW8ydF24Ocje4_c61MLAT7N-Y5b9T5Rt9dCN654z9Rffy86iM-RHJ9WoUYW2kuacZqF88q9Yr98jfrZXdrW8RP8ws_ZRKO8LIrzCv43WaOp4XRls66f2buk9Wxl_ADEwGPJIBwAA&timeRangeId=week) [Identity Correlation](IdentityCorrelation.kusto)
- Enter any number or combination of the following fields:
    - Hostname
    - Username
    - EmailAddress
    - SID
    - AzureAccountID
- Query will fill in the fields you don't know for each unique identity and fetch each person's Job Title
- Only needs minimum of 1 value for any 1 field
