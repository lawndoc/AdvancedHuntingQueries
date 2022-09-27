# Detection Rule Hunting Queries

Clicking on the name of the query will bring you to the file for it in this git repo.

***Or try them out right away in your M365 Security tenant:***

Click on the '🔎' hotlink to plug the query right into your Advanced Hunting Query page

### [🔎](https://security.microsoft.com/v2/advanced-hunting?queryId=32216&query=H4sIAAAAAAAAA72STQrCQAyF31rwDqMH6ClUcCMiuJZaWy3-jHSKiohn95voRnClrZR0yMvLyySTgXKdVCrjnGC1zvKqtNUQPNcBJKirjm5yxDZgFeY047-HW3POwXZgGX7MSFE8kOfUh5NrDZKAeXxn-t_kx2gCfgX9dKMxsZLsEnZtCmtNiXnrLvCNQHfWaWq6Tj3drUqGTmRGNMEu2LNKis7qR_WCSLxjAfvSgn4AKbAKRvPqXkebcdqCdmmKR6LeJtR8hb1td-QGrLB9W5H_31oZPTZfb2m8M5z4PouXvzWvje5Ci7Nb2oad3rQfyxt38J4EAAA&timeRangeId=week) [Mega Cloud Storage Exfiltration](MegaExfiltration.kusto)

**Severity:** High

**Category:** Ransomware

**MITRE techniques:** N/A

**Description:** A non-browser executable was identified making a network connection to mega.io or mega.co.nz. This could indicate potential ransomware/extortion activity.

**Recommended actions:** Immediate investigation of the activity is advised. Isolate the host and restrict app execution if ransomware is suspected.

### [🔎]() [Rclone](Rclone.kusto)

**Severity:** Medium

**Category:** Ransomware

**MITRE techniques:** N/A

**Description:** The cloud sync program Rclone was seen making network connections on a host. This could indicate potential ransomware/extortion activity. This alert may generate false positives for legitimate use of Rclone.

**Recommended actions:** Immediate investigation of the activity is advised. Isolate the host and restrict app execution if ransomware is suspected.

### [🔎](https://security.microsoft.com/v2/advanced-hunting?queryId=32222&query=H4sIAAAAAAAAA62RO6vCQBCFTy34H9RKm2svWPkAm8vFwj6sUYMmETfXB4i_3W_HiIopLGSZzeacM3NmZ4eKtVcix_eXKHRQrp3WGoHHykC86qrprAbcCmxHNDSBS2ATRbZnWuoPLrdanjUG3VjdSKnlNHVhb6FyMDk5sX6II9Eylwhsjqb9Qf2Z9eLhQqWgX3AaEKm2Vun05N0vvVdUK-C9euqyXnsJd1-WvYTzJ_es7mNiswtMRuamYhr9iml8w_nuNDSVQ5Fw36JUPXynsCcQx9-i9Lx18m9v4MkJaITvdzq7aebUd-S9T2L6MomOrqI0FPOeAgAA&timeRangeId=week) [Renamed Rclone](RenamedRclone.kusto)

**Severity:** High

**Category:** Ransomware

**MITRE techniques:** N/A

**Description:** A renamed version of the Rclone executable was found making network connections on a host. Since it's been renamed, it's likely to be ransomware/extortion activity.

**Recommended actions:** Immediate investigation of the activity is advised. Isolate the host and restrict app execution if ransomware is suspected.

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA7VW227aQBCd50r9hy2KlESi9AMqHpISqlQijQg8VVXk2IY44WLZBkpV9dt75uxim2ADrVJZYHt2bufMzK4nEkomRu5wn0kqEd4iWeLtsyQyl4XEciOeTCFJodfGL8a7L89yj3uCy5O1nEFu5AMuIxcS4DKQz7BiZJx7Ug-ZPGJFY64pNfA1d7EDREkgSXeyeStvGEGvU0TwabWAlnr6Ct8hM8kgTWB5Ks0dmwAoIlhEWM8OaF86jJr1cf47WJlCQyOYUrTDup-IPyNLE1xhTYQraulqjF9Elg5Fqrbp49-D3XtGnrBK_5ZT0SVGbqkbgbc1PSSMYhlTDlfwWOfnGms-M9D4Y8i6tAtZKyMDPC_c8yWeIkQKar31mIVmluI3otWV_IDskV05Jgt3tF_WernhbKyYx3POyQi-x8jAdkNE2XEdovysXIcPWYk6vYQsHNvZt0SqVfb5Hxzw_3rVV0-xq_m-DO_IfMgIhzq2XJVq_Kp_Lh95v2YXzFiJDEg6uCeOCdVfo-5Lp5HS4he8rphN4uYn3sKwqWibe12De81mFzIV_hs1Xv3c1wBaMaUbn-Wp6ZGXB8fxI2xi7olFpwY1MTpuOpTJInOVLokmzHduI-9c5Ea-S9t5mCCLgBpejjNiF6VuZy4m8gK-dWrWnNXtHFNpQbLJMoTvjKwHnN35FuI2T4G524Wt9zOeKgm79l6eOLczSO1ZEuXoPGTcxXPI-U_RBy35BlQDdEoLUfq4DzERDfmOtTJWu-P77AN7CinqcSmvWc5WhCkvGLH9ENHOc2dbyHMk4-woFsPOLry1arjoUmP63_nokoneHk7CV2IkYf_O3XyUZ9HAxqI9lp2LLf9tF3cE3PbkmsI249fGdk-dYxfR7u6Xcmk4mWWsUULukzUflhPOje11i3DDQhXS_hZSe6pZ79Voivx6uAeMELn9-W-x7fZNc2eyCoTVNSy-vKpRrvBuO8HDeRdSZlcUn3p-uQPtQ6h9_Bv3syO_Lc9zFp-wZs-hZ94DsKVn0IhTsnDfM2Zn77_m6TzPsz7JrVpgSqdpzK7f_nocIotivz_hBI6BUa2qNDdZppBOeaKpxU_y8cCuH-B96vZmj3Vtvujt5l7ubGWLfDcctfeg6LCLYnb0OrdQT1-g88CcMvLx0nsVxiJf7fL20bHs94DaZKxOwZWV1TNkWMsUUf4ACYnKf5IMAAA&timeRangeId=week) [Sensitive Group Modification](SensitiveGroupModification.kusto)

**Severity:** Medium

**Category:** Privilege escalation

**MITRE techniques:** T1078.002

**Description:** A highly privileged group was modified. This could indicate an attacker elevating an account they control to gain privileged access.

**Recommended actions:** Determine whether the group modification was expected, legitimate activity. If its legitimacy can't be confirmed, lock the account(s) involved in the privilege escalation.

### [🔎](https://security.microsoft.com/v2/advanced-hunting?queryId=32326&query=H4sIAAAAAAAAA62RWwrCMBBF77fgHoILcBGi4pdbkNIUH9im9GFBXLxnIvTHH8FhSAZuDodJslWlh64q6Xv6nb4jqdRoUK-lFnopaNKFrGOFmTuqUJ0ToyP0xMkAGbTSSRuoREUd2MfMrPWEaTk3c5gr4f7dXMLXWEYym6rHe2NP0P-b7eYFaePsjnnqj9nPeuYdkquvy7_VOjrN52cz1_fPvAFVokLUygIAAA&timeRangeId=week) [SharpHound Output Detected](SharpHoundOutput.kusto)

**Severity:** High

**Category:** Discovery

**MITRE techniques:** T1033, T1069, T1069.001, T1069.002, T1082, T1087, T1087.001, T1087.002, T1482, T1615

**Description:** Files were discovered that had names consistent with SharpHound output. The files likely contain information that can help an adversary determine privilege escalation paths within your Active Directory domain.

**Recommended actions:** Investigate the process that created these files and respond appropriately to any discovered threats.

### [🔎](https://security.microsoft.com/v2/advanced-hunting?queryId=32327&query=H4sIAAAAAAAAA3WP3QqCQBCFz3XQO2ze5xt0EVoUVEQ9gZiUkAquVBfRs_c5GSQVy-weZvb8TKxMF-VKebeqVRnynBn9TKUa8FAD3eV01YleTTnNYZ1BGyUqrDPRgztAZ6pYodZMUhg5Kpl21BHsUayZNOCKSah9p9R6hbw3Kvjp2U8YgQtOAvOgVefjmFemlVjHWyansWm8E7SK7o_LElZu-V4pS1h95-_dR2z_uXtkGTx3-y_UAuR7-z0BPRLZYXoBAAA&timeRangeId=week) [Silent Power Automate Registration](SilentPARegistration.kusto)

**Severity:** Medium

**Category:** Persistence

**MITRE techniques:** T1078, T1133, T1543, T1543.003

**Description:** Power Automate was silently registered with an MDM provider. This could indicate abuse of legitimate tools to obtain both persistence and command & control.

**Recommended actions:** Investigate the tenant that Power Automate was registered with and determine if this was expected activity or not.

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA42U22rbQBCG57rQd3DcQGxQkp4DKYYUnItAKKWNr0IJqqQmTmxJWNs4gTx8v_0lq0pryWbZ0xz-2ZmdmZkl5qxnv21hM7uxkFNh36BGzFS8EXPA7YFbglyK1MxiVsccWM76CCVjj-2qwjpGq0BiYVM0rm3I_dJOrI8Vx8jhHtsh47ntA_afOiWcI-iHoGa2BGVlo4AWsd5jLRPd20ig9u0HdpbcHZr-3b-QWNhcrx3Bd_Kjz3uG9tJe2JPkb-RZwnm9Nz3bkTchN8fpr4W-vWKukHL4md0qfq4VbSW9imkKr1dHtIx4Lls-CleVr22RHrbgndm4wnJoTPWbg9rKpb0mVkMLpN37b4wll9hnNGL2uIEVVzwH6py9ifqmE3VCbp03kJoZ0kR5uwXKd8k65cpmxHediBf8pf__sM74Lqz3G7BC5Ld504dOnOd1cS79uy1QP3ai-trOVRNlNW_GOxLe-gzfR2KprGzL9UB1v1fj7YH2SWhjMO6x5zvNF2XTUu-6s1PoZfcparu3VQ5396pMErvwEyrf0UE8fw7dezupankkn3fl7bX60UGVU211fFFletkD5vCDf7ImUM00PQqlEagSU_WLqSTLCH-VhUiYBVUWMTI88n5MwE-lWb4qaGRV0JoZwZrf_QN39aNc4AUAAA&timeRangeId=week) [URLhaus Reported Network Connection](URLhausNetworkEvents.kusto)

**Severity:** High

**Category:** Malware

**MITRE techniques:** N/A

**Description:** An endpoint has contacted a URL that has been reported as malicious to UrlHaus.

**Recommended actions:** Investigate the cause of the activity and look for related events.
