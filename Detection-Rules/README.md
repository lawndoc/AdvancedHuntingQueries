# Detection Rule Hunting Queries

Clicking on the name of the query will bring you to the file for it in this git repo.

***Or try them out right away in your M365 Security tenant:***

Click on the '🔎' hotlink to plug the query right into your Advanced Hunting Query page

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA62W22rbQBCG5zrQdxC-csEt5AC5KA24qZM45GAip7SEXAhbSRwUS7EV2yl5-H4zjqyVbWhgjVjt_rMz_86MVrObSCy5BDKUVEbyJJEk0pIZshjZWAbItQ_kO60vr6AIvYH0pC43UpMM6R19g_ka45SZKpot8Az28RIqZzOefAmVsxFMPRgVf5ItZH5PjXhzx_Pcoi5QD88mji9DuV-gR3AVxQ6-Jzcl6wi_pxv0-YnVdp2cTFitQPpV-hWcOjGo5V4FuV4XeGdFsrth78s1U8Yl-ovnGf2tfJZvtt5P1p_YTovliD6hbyHRnZnzfVTnDdupPCAb0QKkOaPEdOoLqwvbszHMgRzQ9tfaLmsHxtKHc8pMjqb6-VV-SFO6jKo50f_n4xyHck58vhwdOfPkaMlvmh_HCdloenK0ycexN0col54cp0Ry5c0RboDB96vo_vLnCNll_hxtT45Q_njn9Bf_rT-Db0aVo4jkzbSKs7YPCqmAiemXPHrujhfy1ZrWeGee19Evsk2VW1fdVrlv0N6h3gZIh7zr_70FlMwZeilnX0x11vtDFx3l1PobWZ1Xb9wK7vrbNKs5a5c7RfYuXxfbEVoJ2dE4Osg1lw2L5wSebRu34RkYY2RvPa075mHPfBqzi1MYNTLN9JnpxB-0bdrNI5UXO3eu7TagllfMPyOdR13VciNws9Bm9cI2s2znJvsHqH1RNIgJAAA&timeRangeId=week) [Double File Extension](DoubleFileExtension.kusto)

**Severity:** Low

**Category:** Malware

**MITRE techniques:** N/A

**Description:** A file was detected with two extensions at the end of the file name, with the final extension being an executable file type. This could indicate an attempt to trick a user into thinking an executable file is some type of document or media.

**Recommended actions:** Investigate the file with the double extension and determine if it is malicious or not. Quarantine the file if you determine it is malware.

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA72STQrCQAyF31rwDqMH6ClUcCMiuJZaWy3-jHSKiohn95voRnClrZR0yMvLyySTgXKdVCrjnGC1zvKqtNUQPNcBJKirjm5yxDZgFeY047-HW3POwXZgGX7MSFE8kOfUh5NrDZKAeXxn-t_kx2gCfgX9dKMxsZLsEnZtCmtNiXnrLvCNQHfWaWq6Tj3drUqGTmRGNMEu2LNKis7qR_WCSLxjAfvSgn4AKbAKRvPqXkebcdqCdmmKR6LeJtR8hb1td-QGrLB9W5H_31oZPTZfb2m8M5z4PouXvzWvje5Ci7Nb2oad3rQfyxt38J4EAAA&timeRangeId=week) [Mega Cloud Storage Exfiltration](MegaExfiltration.kusto)

**Severity:** High

**Category:** Ransomware

**MITRE techniques:** N/A

**Description:** A non-browser executable was identified making a network connection to mega.io or mega.co.nz. This could indicate potential ransomware/extortion activity.

**Recommended actions:** Immediate investigation of the activity is advised. Isolate the host and restrict app execution if ransomware is suspected.

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAAx2MQQqDQBAE6xzwD-ID_IE3E_AS_ILIEpdEF1Q0h-DbUyxDz0DXdLcEDiKj96l2ThIrb-76gUVno-DGj1I26a2qpJNFaWTIe-FFL0u5a3Meup_cOzDnTMPlrvwaJclMoFZfVfEHylBSLowAAAA&timeRangeId=week) [Rclone](Rclone.kusto)

**Severity:** Medium

**Category:** Ransomware

**MITRE techniques:** N/A

**Description:** The cloud sync program Rclone was seen making network connections on a host. This could indicate potential ransomware/extortion activity. This alert may generate false positives for legitimate use of Rclone.

**Recommended actions:** Immediate investigation of the activity is advised. Isolate the host and restrict app execution if ransomware is suspected.

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA62RO6vCQBCFTy34H9RKm2svWPkAm8vFwj6sUYMmETfXB4i_3W_HiIopLGSZzeacM3NmZ4eKtVcix_eXKHRQrp3WGoHHykC86qrprAbcCmxHNDSBS2ATRbZnWuoPLrdanjUG3VjdSKnlNHVhb6FyMDk5sX6II9Eylwhsjqb9Qf2Z9eLhQqWgX3AaEKm2Vun05N0vvVdUK-C9euqyXnsJd1-WvYTzJ_es7mNiswtMRuamYhr9iml8w_nuNDSVQ5Fw36JUPXynsCcQx9-i9Lx18m9v4MkJaITvdzq7aebUd-S9T2L6MomOrqI0FPOeAgAA&timeRangeId=week) [Renamed Rclone](RenamedRclone.kusto)

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

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA62RWwrCMBBF77fgHoILcBGi4pdbkNIUH9im9GFBXLxnIvTHH8FhSAZuDodJslWlh64q6Xv6nb4jqdRoUK-lFnopaNKFrGOFmTuqUJ0ToyP0xMkAGbTSSRuoREUd2MfMrPWEaTk3c5gr4f7dXMLXWEYym6rHe2NP0P-b7eYFaePsjnnqj9nPeuYdkquvy7_VOjrN52cz1_fPvAFVokLUygIAAA&timeRangeId=week) [SharpHound Output Detected](SharpHoundOutput.kusto)

**Severity:** High

**Category:** Discovery

**MITRE techniques:** T1033, T1069, T1069.001, T1069.002, T1082, T1087, T1087.001, T1087.002, T1482, T1615

**Description:** Files were discovered that had names consistent with SharpHound output. The files likely contain information that can help an adversary determine privilege escalation paths within your Active Directory domain.

**Recommended actions:** Investigate the process that created these files and respond appropriately to any discovered threats.

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA3WP3QqCQBCFz3XQO2ze5xt0EVoUVEQ9gZiUkAquVBfRs_c5GSQVy-weZvb8TKxMF-VKebeqVRnynBn9TKUa8FAD3eV01YleTTnNYZ1BGyUqrDPRgztAZ6pYodZMUhg5Kpl21BHsUayZNOCKSah9p9R6hbw3Kvjp2U8YgQtOAvOgVefjmFemlVjHWyansWm8E7SK7o_LElZu-V4pS1h95-_dR2z_uXtkGTx3-y_UAuR7-z0BPRLZYXoBAAA&timeRangeId=week) [Silent Power Automate Registration](SilentPARegistration.kusto)

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

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA61WXW_TQBDcZyT-gykviZSPAm8gIwUapIpQorYRIPHiJE6a1rGtxGkbCfHbmZ07x057R0WETnbs9e7s3tzcXrrSlUC-ywAjkJksJJEYT7Hc4kqloDWDNcH9DrYpLGPZ4t6Xe5nAkkhHepJjJIifSISoBbxT-HyUr_IFvxliruE7IeISPjfwSWWOtxT2AtiZrGAN4KOxqfU2SGt5Ls9Qa5eYmWyQSytRjOkuq1ZeyBV_c6DFiIsZHbOGWW2uU3zPWHWMJ1NTgioixlXZ9C1iriUrVKSIs7jCvUD8Wt7Sd446NPsGc-1wFktYNYfO4hbPJ5bTl8RRPK25DR6V3zY8IzCrTGvGNj2mtpqELAXEWuJ5BoyIT4GEuF4j87s9T8XJwOgGuN8sU7qGxv8VYtXmj_nA78bbj9Vl7o4cW6QTamdBZXyyeurv1GTW8Rdi7rhOhs9LO6c1PHROOWzvyfMcWRqOOTedOGW-sx0zMStdw8usTSBHqNXwfeTByKgtfR9ypTXqhRPpJ8YA72PWtcLaqaUHT9XSFt4LXMZ2hmsgP-RC3pAvo8Oqhpx6rPZIncdTZG49sJVzbDnm3fLMQ-0X5HiFe-jgXT3OYcmp9WKXufT8jGuLyDE10PAgPFZRtV7X-GJ0dWN1FPI3tfuwQc_Ajv0Z1_vEQ02VEf9LWz68U-RcMMr0Oe1hQ67dhFnWDhWG8pt6iWsdU59ju_6H5xrafqU8-POuwdUEuBlZ8Of-mwbr2jqvda8RYpJH1qHVj9p7tT5-CfXkRKnnLseInXrF_VN1tqdZ0AwTngrKQ1WpK0efnV6ZOgx9hPpTL3bKkyJ06s4ds7-zTKwqUeuIoU__Tmt7u7JvD7oreGr8-14_LI-va9QVuoQe29RvTo6mDgYLoOjdKE1P_Qb8zP-DcrfvIzclsP9XfIrfz-E6Nxq71W9Lvcs2yaDpXDF3qvoe29M3wG7siP98rfqmzrmwp5BLXWEt5x_6gfAE1gkAAA&timeRangeId=SetInQuery) [XLL Dropper Malware](XLLDropper.kusto)

**Severity:** High

**Category:** Malware

**MITRE techniques:** N/A

**Description:** An XLL file was discovered followed by a network connection by the Excel.Application COM object. This may indicate that the XLL file was a dropper malware.

**Recommended actions:** Investigate the XLL file and URL of the network connection. Quarantine the device if malicious activity is suspected.
