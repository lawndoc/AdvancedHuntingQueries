# ASR Hunting Queries

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

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA5WSUUvDMBSFz7Pgfwi-1IJ_YQ_iVPRBhfku3RZndW1H2zkm_ni_3KzrkBWUEJKce8_JuTcZy-tTuWas1-y8SrVqdKoTfctpozewmul0SVZLbkXOs7ZaGdqAZWQE1oZoC8MpIbsBTUzJ7UYGcz6o5C36W2UNFs6eNdn7asALRrg515fxr9Bbm3-nEXO2P58r1YVlZKa0IBJ4Hp2YG5Q-OL-AeGMc85iSOWXvND7o2wPcgjXc8Ej2k_Wr0IT4HPWg1HuJaFfHO3gO7nQHGrsfqt1yLvVK1JmDY8qdxgq0Qsmb42FvNzhYMjpsZG9Xk5dZxbdw4g84ZJ3ZDLsJ_JpojMWO3nPzlP4Ez8sdo3-HoZ53zsPLNlZx-U_vf7u75RRrDDcsqPGYm_TgV1X2k7tX7tV-AAq0JUYoAwAA&timeRangeId=week) [ASR Top Users Audited](ASRTopUsers.kusto)
- Top users triggering ASR rules, sorted by number of audit hits
- Each user is displayed with which rule(s) they are triggering, their job title, and device name
