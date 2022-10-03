# Incident Response Hunting Queries

Clicking on the name of the query will bring you to the file for it in this git repo.

***Or try them out right away in your M365 Security tenant:***

Click on the '🔎' hotlink to plug the query right into your Advanced Hunting Query page

### 🔎 [Baseline Comparison](BaselineComparison.kusto)
- Performs an artifact comparison between known good hosts and known bad hosts
- The following datasets are returned: Alerts, Connected Networks, File Creations, Image Loads, Logons, Network Communications, Process Creations, Powershell Commands, Registry Events, Raw IP Connection Events
- 🔎 does not have a hotlink because this query is too long for Microsoft to encode in a URL

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA6WSW0vDQBCFz7Pgf4h9asEL3lAsClIVfJFiKz6oyJoGW0zT0mytivjb_XaSSpQKggy7s5mZc-ZMdlMl8orU0khDjTUxP1BOvKcT9me-YnxO1SGrp1dlclYVq64b1TQlOyC2plTb2tK-NoneqaGmlrVEtOjSwTt6xOrrGkQG20izknmPryZ-A2sZpy_VvIF6MJYIZFHdJzeFK9eqqZqrc-jLrWtV_YUpmIGZ6EmnxBO6-7LyHeQMxoRs6NEFNbSZvU06JnbEcnqEof7rHI2FbN91OGMO-h389-wZiiNY_3IHRYfoy8I8kS7JDTl7_BWR9J_8Pyeo8retp7f_Hf74Dra7EHUMp4d5hIIuGsYWLVA1U5NhSaWqw43GpZKcmkWs59QNDOFsz7iTts00x51xTpksINpWFd7Mij7Kvge6xar3llukYy_H26zhFYdYZm8w581MOKdaJ_vCqukTOfmNtToDAAA&timeRangeId=week) [Compromised Devices SMB Traffic](CompromisedDevicesSMB.kusto)
- Fill given list with known compromised hosts
- Set search window to estimated compromise timeline
- Hunt for suspicious SMB connections originating to/from compromised hosts

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA-1XUW_aQAz286T9h4gnKkWqwrS9TH3oOtAqUUCFag_TNGUJrGkDYZCNIe3H97PvAkm4hJDwsIcp4i7x2T77s89nLumSLOrSgCYY7_F-S0O6obG8MXWItwl9wqpFHzD2QfmM9z7Wx1h5Ta-gg7V45NIC83eaYuT3rVAjmoMW4NulGHMkXBHNZI8RrcnGmy98rvApygzvIXSx3Byzoka0wvgI2hojU9kC5otBH2N2weFhzaIr0bvVGgJQ2_SFWni-0gW9T9m-zsjN9C5T-i37x1i3xDL2K8RjgebCq_DAgiUkI-hh-lpGZcdH0RbIyijD003twpr-gnsjvq0EyR54Q_jB3yPB8HGHwLcdzu2M7xcaKdZn5Z472PK2kYYx8uGanDPo6MCSdxX0JLhM6Q_8Z7R8ycst8J5qhFs5XFs6wklkknwyRaSn1_7H4lyxSBC1UC-Wgtf-9Ocjs5DZkzVTdAayvhH7n4_G6B7jHLxsG9eXJsikdT2AJzwbPlmfLNRc9p6R8A5wUjXqCTRVgzaYY12pVF1lu37SL8FgKzJdXU1DRDaWasXWzTVytxi5yplzXEVuoOvuv5ZZ5Z61dlr2eD3L7EN-Boy4fkeYY_HYXLHVHTWBnLp5YsFiebLudM05l878aTmmV_n3pDPLxHkl2lxtKSPRNnDZRlmngN4poL9BnG1jrlgHp17ln8k6E59dIO8UrnRKbdnXmSQDzTipNTuVqU7mq5P5Kvc_fV5Mu6XX7Ry_c0Ap9890l5n2NPHZBfJO6Y7Z-_lGOr65VAMf_WQgmV0sfQ1JT04Cx2Qf9Wr8D0B_UcLNFTGQyqvuqQX9yNlr3t-EWF1ddgM7nEbS5ZlyqlaF9TmQSaJW14Z6qCjZppiY87seKkVnpb4dVZExSzfFpmrtqaepmmfm-lVf9li1VZ3AEBIB9LFW7k5Pk1A9aLEM96uqD-QbV9kci93RCXJjOQkr8bbcxqzcqRU636lX4xxJtxlX5D6GWF_Q4awrt6A6ltnO_k5njIsIspd-6e2vel7Oqp7sNwemPp6V1lLus4ccWeKnupZ0n1xNh_o3ajqHasXe8ZTf88l_0uIOJt2rOKLtBXdfvKWKEgAA&timeRangeId=week) [IOC Search](IOCSearch.kusto)
- Search for various IOCs (IPs, domains, filenames, hashes)
- Searches processes, file events, network connections, and email attachments
