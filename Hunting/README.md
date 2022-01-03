# General Hunting Queries

Clicking on the name of the query will bring you to the file for it in this git repo.

***Or try them out right away in your M365 Security tenant:***

Click on the '🔎' hotlink to plug the query right into your Advanced Hunting Query page

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAEANVWTU_CQBCds4n_oXjSg3DwZuJJNOEgMY16NbD9oIG22C1fxvjbffNagghEBKoxZLfdmTfzZmenszSkIY48SE8isXgL8ByIjzcjqSSSSweShLoLjBcZQZtB5kN2LEccDXpp0-JcutCnMoFekQ4shvCZwpNHXyFkHlbq28GcYr4DNuTaEDsCwoEH1WaQh9ArUxPPMbwYPNsYOXgU0ZcbyH1GXMT1BvsJ9qUx6H5czDGwOZ6PkA3W7vEEmCKSOmQp1g7972Kv2jrkr5Cui6gFXQTriLkoMnPP3Blm18pteRptIGLa1OSdLAZ-FKnSOsYUo2Bxyl8H_rw9WbQaNNYA6GmFPBaSAEPrqjqWFHXos5qq44jouaj3rNKzifkVKNZiBKxLj9_JX3Aa7Lk63uWO8lyu-1xVuVv7CzntsiLHKxyLvuqWPTGhnZUZ3kzZOVP2oVPqJ-i9RUfS79ZjNzS0icEw4NlF7K2WsRvGOmbkMznbs7_ukoOrMgfZpx1uzoKyF5bellnRWy3E_N_yUvs2Lz9neSLWcqcJ8drVr3mHDFnJszUn04O3HHorlzyH5Yg0A-GXb2J-X-4aUYu5VE3C09muag4bw5yzSZThvTSkB0UtInA_1V1Qcm7-_3LYGAuMByat19XsuEvZ-QDY41I96AkAAA&runQuery=true&timeRangeId=week) [Exfiltration](Exfiltration.kusto)
- Non-browser uploading data to Mega cloud storage
- Rclone sync tool (low-confidence malicious activity)
- Renamed Rclone sync tool (high-confidence malicious activity)

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA62STQ6CMBCF39rEOzSu_TmDCZq4MWw8AKFEmiA1FoSFh_fN8KNxpcFMyMDrm68tMxEy3OGQMu-ZC-YdlQwlKgTMMcMDBg1yajc-ZvQdkeCiSgqv_oQrJasMFrjyKzAart1gqXzHkp2t1jkSc2WtqXju0jHMGEL-ldFOpLR0hb8wpp6kIqHqGRuGwUrDsM4ypK7ljQvUrHXaI-nN6-93fqkdemPpC6RKH1Nmg-htQoYTLakf6HDqTHr_GTG5Xp3S-S3fZDJqnY0TJ6LUys_7dZqnZvVksRJzPAEo8phwnAIAAA&timeRangeId=week) [FilesWithPasswords](FilesWithPasswords.kusto)
- Files with the substring "password" in the name
- Results probably contain users' passwords in plain text
- Included file extensions: .doc .docx .xls .xlsx .txt

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAEAIWSS0vDUBCFz1rwP4S6UTB2L7goVaFQHwsXbtM02EheeJOoIP52vztpJNGWMrR37syZM3PmZqqpAm2Uao0lKrg9a4kFqhTpU5lKzjX3RB_8YjWqwZeGPZVTS2zD3REPfvEO_4aKmJpMF5rBV-GlRKIBQ4sXcc71oDud6VhHzOSneqOy65yD9bfAKv28NVbR49KwL3DURBut6BSDzomWIHyfFv_atNU6MR7PV3OGzJdh4R-toSH8Pvw0vra1uRMUtVsmZ7kvpnmnc7Kd7xZchncPT26RK33zP7Ht9bvoNjnZybCAPbW5uy0VqHskV1q1w_b3GL_F_z6V8bzaK_o9PsGUG2ttXJXOiQ719j18fEbE77Yx_cPMeL657T8nX7DDpWnocIe17a8d4xZke1XOvg6vZ8Ub7lL1A3NOUNvmAgAA&runQuery=true&timeRangeId=week) [HiddenXLLPayload](HiddenXLLPayload.kusto)
- Excel spawned by svchost.exe
- Used to bypass ASR rules and deliver payload through COM
- Implementation and writeup can be found at [optiv/Dent](https://github.com/optiv/Dent#remote-xll-payload-mode)
