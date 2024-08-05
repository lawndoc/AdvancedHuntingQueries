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

### [🔎](https://security.microsoft.com/v2/advanced-hunting?queryId=32428&queryTenantId=a092aca4-b5d0-43a3-aef5-ae017bd139bd&query=H4sIANYYSWUAA6WSQU8CQQyF39nE_zB6VxK9GBMPGMAQUYkYvXhZlkUmsKxxBtHE-Nv9pmwIoidNM9DtvNe-ttNQQ06XKvSiof1WCkQiXqYx5pXzPbabEm-hOSdwMs34fgAx14jbpTGfDZmTK2C72lEL_9XyFLrmRJAVqKnaxAvYsUZ-wF9qYjoK_Ft-S7CR_75xItEzzOkES5yGdXCAOZ2T8UJdqjh11FRPAyIO7g1eV3eceyKDmvFbzS56PHU8_UXr7Qn-Zk8dojPrJUNd4uyZon3MYStFJaiEXmVweKnTYF045pWyZ39WUKFgZIy-oSam4tNU5DrVI7b8tpkUCXrnRJvqsY4sNiOSWdZD4m-czS62t5tqjsEv4KVdTH-8nJwbX291ez9tZtb6x26a1B_Vs6mokF5gx6qlaQSbQW43abbe5p0m0jdtnu42e_PMdW77SLl7hl-AcXBTz05XePlaSVi_wCFzdCj2tv9g1UpefkJ-AYHJOUJSAwAA&timeRangeId=month) [Kerberos Traffic From Unusual Windows Process](KerberosUnusualProcess.kusto)

**Severity:** Medium

**Category:** Credential Access

**MITRE techniques:** [T1558](https://attack.mitre.org/techniques/T1558/)

**Description:** Almost all Kerberos traffic should be coming from lsass.exe, so other Windows processes reaching out to port 88 may indicate the presence post-exploitation tooling such as Rubeus.

**Recommended actions:** Investigate the process generating Kerberos traffic. If the activity is deemed to be malicious, take immediate containment actions and look for lateral movement to and from the affected entities.

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA-1X227TQBDdZyT-wURIbaRQmgDlUkWiokVUUBrRlpcKoTRx05TUtmy3oYiP58zZ3cRxnPWSF16Q5dienT0795lMVKhyFahPKsa9r1I1VnegpSoDtYv7RvXBEXKlryb4_YWvTVyh-mlWIq4MydnHSgpqphJgRniG6g1wMqwJRqRGqonvc_VWNdQVqDk4M_A8xTXltQW0mIhFebbwHoOnD_4xnuXVAX7vgPkN6FOs5EAPIM0ldqVGjy7Wc8rdgBRN9VA9UL_BZXWJgBrMNNEWSPCWUo_v5oxlDVchHcKmGiUHb9EGm7NTztU2ZG6qFjGCpWtP3VIX0aIeq-3EekfJtUeHBbShoeVAvKF_54idGsQYO8S60QLiKvmeOdH2adcBdyaURixcj_rciXpGHw3AKc96tBc1GmtbjeiRew-8HSdez8TxGBEvqOEs91yYL52YR4x_8bVfBL5yoh3DF5JlfXpE9p5A74xWuPFAf-1E_0KNY0R5Ch_5ad-uyZliJVs3pto1udQzlccXzZ1HH0wGTbwitO2RRzlj_m_0dWfRR-yIUVkjRNc-csQH0Z1Jc8QT6L8Hfh9MdzaVMTuQYccL151Rc9weIvWCnTBDVQ49q7I7w1ajD2FrXW98TnFnmusUXccTRqFPTevUZKBbo_UyslOTkV_NnHKJO_TqRp2arDwF18irInVMRto5IAFXrK5NDj4BzxS3WLY8O7SUTEMbM6wN4FiUqYmwcEGWR5SmMaPILLMLikxQATtIznPGtEEMewTE6eNbx2tK38gpE8NtM_CIUgzIb_Wumg6thNdYG9N7V3zmmMS0jWyXvAfGBU-U83UXlhN_kH-IVXlGRrLNBU9IpEhnlL7w3nTIA8ogJ2ULvGV77RWq3ymkSEwOadtZtMWJqOFEnFcp64FF_iatLbZ4TOxLWqO6ynXJJRYdcQremq3uVvhFV7H_vqnzja321f7x27P9j691Ymre5VbFlebQsXWLfbbmVud9yxl5Nr6GrOl6Jhwwbk7N_4eMlUz6SasUKZ9J11WvKgqEbv1f5K3uGd01-oyglWf4VkX3ENrybNoq2KxsJfk-pG1z_lu203KPGab3Z9R6QEzJk6KOVu9j4z_ZfYb3yZIVDwvyJdQhJ816JjO0ABa5r_TLH-FhTfX6DwAA&timeRangeId=week) [LoL Drivers](LoLDrivers.kusto)

**Severity:** Low

**Category:** Privilege escalation

**MITRE techniques:** [T1068](https://attack.mitre.org/techniques/T1068/)

**Description:** A vulnerable driver was discovered that is known to be exploited by malicious actors for privilege escalation.

**Recommended actions:** Investigate the origin of the driver and determine if it was created by a malicious process. If the driver is legitimate, determine whether the driver can be updated to a non-vulnerable version.

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA72STQrCQAyF31rwDqMH6ClUcCMiuJZaWy3-jHSKiohn95voRnClrZR0yMvLyySTgXKdVCrjnGC1zvKqtNUQPNcBJKirjm5yxDZgFeY047-HW3POwXZgGX7MSFE8kOfUh5NrDZKAeXxn-t_kx2gCfgX9dKMxsZLsEnZtCmtNiXnrLvCNQHfWaWq6Tj3drUqGTmRGNMEu2LNKis7qR_WCSLxjAfvSgn4AKbAKRvPqXkebcdqCdmmKR6LeJtR8hb1td-QGrLB9W5H_31oZPTZfb2m8M5z4PouXvzWvje5Ci7Nb2oad3rQfyxt38J4EAAA&timeRangeId=week) [Mega Cloud Storage Exfiltration](MegaExfiltration.kusto)

**Severity:** High

**Category:** Ransomware

**MITRE techniques:** N/A

**Description:** A non-browser executable was identified making a network connection to mega.io or mega.co.nz. This could indicate potential ransomware/extortion activity.

**Recommended actions:** Immediate investigation of the activity is advised. Isolate the host and restrict app execution if ransomware is suspected.

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA6WQQQrCMBBF_1rwDrEH6B2E6kqruHYT04hCbaUNFsHD-zKCK3cyDJO8-fmZpFLUQ1cF6praUleQqE5Jo-aa6SWnSRfYQLqvrpbXzUhWN6gnOgmlU6FSPTSy-u3R49HYfo_P59SCOXq72ePU4ZidjsRSd6IypTeyQRlYt7bb2hsG2EieUWW6swlqSKJm8v80B1RBTzL_QamT9Qq9Abr72LRKAQAA&timeRangeId=week) [OneNote in Non-Standard Location](OneNoteWeirdLocation.kusto)

**Severity:** Low

**Category:** Initial Access

**MITRE techniques:** [T1566.001](https://attack.mitre.org/techniques/T1566/001/), [T1193](https://attack.mitre.org/techniques/T1193/)

**Description:** A .one OneNote document was found in a non-standard folder which may indicate the use of a macro-enabled .one attachments as a phishing attachment.

**Recommended actions:** Download and analyze the .one file and determine how it was created on the device. Look for suspicious activity coming from the OneNote process if the .one document was opened.

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAGTDDWUAA-1Y207bQBCd50r9hzTqA7QGSqsWoTZVIxIEEtCWwEOvKImTEMhNttOU3r69Z87uxnbikASJ9gVZJt7Zuc-Z8ZoN2ZCcVKQsJ_j9IG_lVI7xVJZDKcq-HOC5BKpZHWG1h71j3PflnnSkIRFoDelKVdpYn4kvfbvqYaeAO4_976B0ZUCJdamTJy8vqWWDPuxDsgGZCJJNuQJlAK5oTKtCNifv6Z3KK3cO1AhXFZRzaDS8YULrCnSpZEjuHv62KNOWb3gOQVM_6-AYWo1NxqGaqtQYUq7POLuUVVsq1QKlBo4Odkf0KgBdPQ7o72oqR-9ACbnrI1bV1LLaC8y3y2AxI6J9_G3CSg6Xict5VIffAS7D12HehozWR3ZzoPUpp9p73E3mQzMc0meXD_X4F3ZGsN6g3hyQ0baZiGwVc_KauW9BfkWeyRNYW82UrdAzn-td3Fr3ItY-90PG_8DyhJBUX85BU1sBotN8rwApb3B7M3GWbXvXVvIEcQ9IUd4_REUeFK2galWEXpAjXofIh66u13xkMZJEhqlpQG2Ke9X2lRk0Ff-EbK3JtnyRn8jcb_mMax3UIqgfwbMmP8Ycj-UhpOOqt1O4GSQQZWKLWOs4S4pP7ZSrcRTqUWTzbbppBxw9ot70X53xmL49ILJdn8ZInuxLp8dfGtF3eLsdvDk8xVjbhqVNrJdDnJnUXWLETd8W86e-VYm4IDE3lsPXIbHbxsTqZqBMq1eDjRppdxj71xirs3KR9SeEf3XGlmct8jes-R6oLdidrHcJv01aMu_Qu3r_73q7SrvT1k0rvkObTm_61FfEVcJTmZZ1oqRPghHPLGYWqMU6qWYaVel_MD7xOSRNymdJFxOyxs-Ycps4ClCTNrNTAf-Q-Ggwo5PoyS-Yh7gqF1ibU3ccS5n2kjXpT3CoFadhQP0XVv8aohrhVsuP8O7Iiqmc8C_GaMFW_pTnzGAmco5pqQ2pto002eHpDitMdVQRT3VmUSUdjr0FOi2JwAHkI_ZVZDGl5yZ9r7WIJxOr8g85m0z-5p2BvLlvMG_uzFP_jJ7sL4fpul_y10eu9Ne8o2_SDybGxauzaKe8yqRvJs4bs7_5BvzqCtkb2p0d-91lTr81onT5yZHluU98Ncivnp7xjNLEpTPXZ0eYGZsVSzZ91Ua_lYg19iI37ntTxy3rxZWtRlOSp_pF6x5Xq8yvu16qukeMcMTz2yVPYlpJg63ZMyErNi81T6b3CzPzlJaKuCoknr2lUOhxxg6BBeetsTF9UnCzojD1FvSueZ95C50FJrlKRK3-50PrmbQz-W43knvQ91Seywuu51UpncWYkpyMFUbhcjmgrvTcDy3N9dF0vf4CNS9CZygSAAA&timeRangeId=SetInQuery) [Potential QR Code Phish Victim](QRPhishVictim.kusto)

**Severity:** Low

**Category:** Initial Access

**MITRE techniques:** [T1566.001](https://attack.mitre.org/techniques/T1566/), [T1193](https://attack.mitre.org/techniques/T1193/)

**Description:** An AAD/Entra Identity Protection alert was triggered for a user that may have recieved an email with a QR code.

**Recommended actions:** Download and investigate the potential QR code image, and investigate the Identity Protection alert. Reach out to the affected user for details if needed.

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIALk5sWYAA71XXU_bUAz186T9h4B4gGmMdS-TmNCECkyVOsqg0vaatikNDU3XhPKh_fgdn3tvvpq0IKapapM4vtf28bGveyAH4smJnMqVtOVSOnIhffz25FwO8eaYb9t4_o67RAJZyJK_-jQXX-5lhucRnn18hzKRUCI-z6EVQxJAM-H7saR2rY9VHjRnMoDOHa66QndKsWMMnSl3iyFT6RDykE9v5Q18Vq_P4VUfnh-u8VEt7Mstnm656yNkgTxwx7tsT9VL6HFMX0N4FUHHg8aEUdzJNe6KMY0gWzA2D7oh_FX9U-ytb6OST5eQXNOGif-XdPExKGjcPfoSYeeYcecr27Thc10PXt1YLHIUip8rvNWcLOwKtRDRYko_75kb9W3At8PC7urHmBh5uA8oM6jP4HvRp8iuWHB3j8guiXAA3dTaUeRixrWOFfqrsUS0mFvplJjRruGBxnNE686bkP6E8oSnXe7qcDmBZIk3avW8xLFTej4jPsUVBttulrNZhkMdJw27h9x_nqFZrY8B2ZfA4pDYJDaPzuYfIjdhLAFrL7fQx9o5pUeMevsZCB1XPNpea63DGFOi6LJ-UcrVBZll0DpjPhVNn3nP_SrH98FW23YNuk01G7CGIkSWFPDdJWcNQ9XeDe5C1q5jbcxIQ_ijHPAzHPbWxn1pe4NipN3Pky2b4xR7hNb6trTkk3xGPB_ttwVZkSkx7Q_Igyk7x4Idb0zeechgDxH32K3U_mPWdVJWh95NsGLOPDu-fYX0CXeLgpeeRaZal6aTLdHvHqA7xl4P8LQF2T4-ajWB3NTfciVDr-PGKh-2LB8UhWJ-c0bk6P1ARKHF7dh24IT9wHhexG5ou43r7qaLxkTRSBfYLapEZOx8s11mTI1opRrN7rfsKaYzR7QRUDMmKqZv-pZ5GrU70wz-J3aPLnS0NnX3KrY5d6e8joBVaOt3wVWh_MY1qPSuMubF3uVlZ6NX-ZR7n8nO-1rNHaI2Jic2Z7xDfEzV77D76gmpa1f1_oW9po5Ttl3Veh2r2yU2dC0XWuLVdoj6zqccnjbwoq4r9vHezBJqIWKfuGdnSDP-qRflE9sxKpF8qhhTYs5ocxLP7XlsqirKJrPb7C4_26vImb7h5o8mXnkrGVBZHSNWO29VdsHYUsq7XK-xOM1c4vTU4z35wutL5oh8lnL9oelk2jzH_K_q3lzVxep6buU-r-qb7TyvRl9e63mG2pSb7nuHHCgyUcb2gPdJxvDmfwUJqyhGPXl2YnazazmvLqday2YOHNVw3EyiVWmrgftGe1XeyqyVa22fU6TPTvCuoJVY3rvJss_ZJ2D38XnSF3Fr_l9WN285G8V-2XzG_6TOGTtbVJr6Nk97QzshTOQvxccSo4wOAAA&timeRangeId=month) [Remotely Spawned DCOM Process](RemoteDCOMChildProc.kusto)

**Severity:** Medium

**Category:** Execution

**MITRE techniques:** [T1175](https://attack.mitre.org/techniques/T1175/)

**Description:** A DCOM server process accepted an inbound network connection and then spawned a child process. This may indicate the abuse of a DCOM provider to facilitate remote execution.

**Recommended actions:** Investigate the source of the network connection and the child process that was spawned. If malicious activity is suspected, isolate both the source and the destination assets involved in the remote execution alert.

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA62RO6vCQBCFTy34H9RKm2svWPkAm8vFwj6sUYMmETfXB4i_3W_HiIopLGSZzeacM3NmZ4eKtVcix_eXKHRQrp3WGoHHykC86qrprAbcCmxHNDSBS2ATRbZnWuoPLrdanjUG3VjdSKnlNHVhb6FyMDk5sX6II9Eylwhsjqb9Qf2Z9eLhQqWgX3AaEKm2Vun05N0vvVdUK-C9euqyXnsJd1-WvYTzJ_es7mNiswtMRuamYhr9iml8w_nuNDSVQ5Fw36JUPXynsCcQx9-i9Lx18m9v4MkJaITvdzq7aebUd-S9T2L6MomOrqI0FPOeAgAA&timeRangeId=week) [Renamed Rclone](RenamedRclone.kusto)

**Severity:** High

**Category:** Ransomware

**MITRE techniques:** N/A

**Description:** A renamed version of the Rclone executable was found making network connections on a host. Since it's been renamed, it's likely to be ransomware/extortion activity.

**Recommended actions:** Immediate investigation of the activity is advised. Isolate the host and restrict app execution if ransomware is suspected.

### [🔎](https://security.microsoft.com/v2/advanced-hunting?queryId=32333&query=H4sIAAAAAAAAA7VX2W7aQBS9z5X6D1O_BKSUfkDFAwkhSiWSKpCnqIpcbIgbFss2UKSq394zZ8YrNpCokQW279zl3HXGc_ElESUj3JcSS4C3QDZ4u5ZIVrKWUG7FlQUoMfi6-IV4n8iLPOEe4XJlJy3QlXzBpaQnHi4F-hIrSmaZJq0hkWesaJs7UhV0raxtD1YiUOI9NB_lAy3o6wwWJpRag0truoNun0gSUCNInsn5nowHLwJIBFhPjnBfWB816tP097GyAIe2oArWDK86yH3JCCSM0xyX32Djilx6NcQvYJz2bZ0ic49_F3KfaXnOPL0NU14nSr6TN0DkdtQQ0YqJmY7iFhqb9NxgbUIE2v4MtAHlfGZLyRjPa_t8gacAlrxGbUOi0Mhi_KaUupLfoD2zLmeMwojym0Ytt-yOLXG8ZDGZQvcMCEw9BKSdViM6Pltb4w_MRBNfxCicWtv_L5taU2hzeMjiiJH0aeFYBRajXO-P5m_LV95vmNUlI5vAkz7uugomln-HPG4sR0yJP9C6JZrI9kNY8iHNUJfTy-H0SOeKqtHvNGidZLrG4ApJTXUWu2DIuPy0MX6GTMgpl1ee12Cjb6tdRzJHrqkbeuNns1jJJ2vZyeauqe85UHjkcDM_A06A2M7avMN60K27YMfeK2OMpUOMRveU_ZbYHJp4upzzQYbTTPdV7fwu7wKp7z4QJ-T12OGrUhy7Vp-Z1gZzi7tPRAtP8ovdvQS1V8HiAu0Azz6nRIzq6sgjYjVG_XVg5R73B_SZIz-wlkbQLeRYcVamXqpSTaZ-uiW_6r0acH3x7p4N6NPwld5FrNWVzVHZx6lFfpqfvZL2Li1McbXsnrOAZMKTQjnPbe6ODidPisSxNOO7A55jHVnsbq_UX2WUud0h7h4xBuzI12Pez-z5XhXn0Z8V8r_Mujg_DSX0rJqlLd5NX7nYgXzSzEpdRA55p6vsL-6tE8967UL3mxhGFluOdW33MGV3-KKPuWepD6aTNJqm_tf1P-Oe-5Bpfp8p0EO9XWNijiF_h_PENzxf4q0DyyM839veOY70_SdWM9Zqpx9Hm-8fh6u9zr-2re_9LFXpRZnjmIq76dswORmSdHLkHE6pkic8-7jsoOIs8-xXQcCd0Jw3A9sJCWNmurs4c84Pdlw1Jmnkq_TU-1y77qVu5RunT3z6VKO_toq6ynwjfkVpujnJaV0Jz1Spp7GlKZxQdrV-KnZpDK3_ABs1JzYeDgAA&timeRangeId=week) [Sensitive Group Modification](SensitiveGroupModification.kusto)

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

### [🔎](https://security.microsoft.com/v2/advanced-hunting?queryId=32425&queryTenantId=a092aca4-b5d0-43a3-aef5-ae017bd139bd&query=H4sIALg_XGUAA81YaW_bRhCdzwX6Hxj1Q6RUihqnZwIBFRwlNZCqri2nAYLAoCXKVqzDMEk7LoL-9r55s5SWhxg1SIGAoEjuzs715thVV7oSyIksZSIrGUsqC4nwleB3gpkjPBeY0e9A-hhbyAzzgYwwupK5fC1fgYdymWMmBmWA8Sl-E0cR432Mt4VcgWLuOE_lmmNP8H4B2gSzMb6U1znoEoymciYP3dqufCfv5Sf8_ii_4LmH58-4p5g5kt9xdWRfQqwLIWMFHikkbbQbyh_QeUB5amtEvZa0LZA7fOszxqorXCtol1BL01gpQ_omkFuOTaBXCKoJ1mRSOl_AtbF4IK_hkZdA91gOYP0Qz0Be4C2Q3zB7hLuN90PQDIDtMX4D9_6K733c-6BX7w6wfoTvv8BrhPXGX9f2MdPHmMlQ-XPnzT59qTjfEHXDKZAeMTCs9D7jiiY00MhJ4GH1bASsNJ6uGXHn1PUZRm_wPcbzmPHhU-TpW6B_Q30CdzXkT6zR1ZfULsZlMdsg94Z7br_Ms0W7AkrUHLlmnMwZSXlb8nqMMKLx9AorI9DoykyHCHEeMlssVzYWP1rrZ3q8xp1Ckq4OKFcj_9bppNEQcDZiNprdhsw34LUnj-V7-YGavZWnX1wUZ1FkUVPObYujBccjoh6yBv3NWPL93aRPfXyy6GsSm5gZv6SvntBnxSj6FZ7__6pUF9JC4NalNSpXRxa4lG8M_BtAyCqPSlSLpqxRZn0P8wktbEDfVs72D1x3QdvVZ0V7A7lHe0NWvNiT0SjlY6PE2bLgHebGxKrIvUif4bBkhGYoGJJXlKKrTp3VZXTKtvkc_bnsKtpgsrQ3-Sg317q8AXZvIaddye0EKL7cgcejGh7PXU8Zuo4S19hfJ2OPMrZJ2Xd5cc44udtB58fkV_TvAnp06GXVz3ArWmC8y3bVo1_NRTHSyhey4p0WtC3rX-TSclX0gVfTW17NHKFLPcNteZ7v9sXObtVT38fIiPrY7zCDQ3q6GLVt1pD7a1_fh6fbO3nMz9xyJN-jF_5hPWigs6f0Wsgd25z5ah44wved60vH5HeT6zj-_AgUeY-NWVVtV9ihTXNQPxXbPQXEIkZnqdO9jHVe9xu8j9nnsm74kNESfSZd8pF3SD9duj1JxNpteGd5qLOnrqM2XVa0vB4ZIPasOxlNsN7bbHaMEb28ZFUN1rljUTMm2vEa83yvy7yVVYZ8N9vWDz8l2xJGysr5vCqbilzfgdpOAJd8TsBHn0u3C2lWVqMU8zPild_DZfIGnq-K-7zDnMfqKIf04i3RvMxRVulUjNE-89i0HCGqrlyc9pgjmaYqz9DS6Gls5fz5va95YB4s0tVlXnbCKXNXHcy2WyJoObjJu03M1nsmj88-5YZr__jZq5w1g1PuarWbzlnLQ-yDh1ip-2g9OcZejdpYoD0hpY4X5F3OyecuIsu7729z--jsPHrGbhJwvxNShkax7Z4T1pMzl8m-3pNcxg4Kc_4Zp5jNum6XHNp2bjL0i30g4-qjns-KDO8xOSRujxnLx85TGeeJOyXN6P2kQodyJm4i00fohfOaj0Ys_s42rfkvwrxQdbL6L54OyXNWg121n-tsLGf8yfpc1nNxPUUOaiYpCil18Luh5ZJ15GoqnTlgHU141kkcSvn8q17bWmsZ068L2mRnJe35M7f_SNzJs0eK99C4PNeq0DF2K7SnntLyBGszH9iKAeuK4ro581evK9dBzcS7T8Bkg3-5s25HuWzzx-Rs3ws-wFlgG5XKs52HRUq13F1trkJlu9_bYv_uZbvfA1fXPrgMsx1xtde1M8TgWO2rfwF25WkfVBQAAA&timeRangeId=week) [Undocumented RMM Software](UndocumentedRMM.kusto)

**Severity:** Low

**Category:** Command and control

**MITRE techniques:** T1219

**Description:** Legitimate IT remote control software was observed on a computer for the first time. This could be legitimate activity such as vendor support, or it could be a threat actor trying to blend in.

**Recommended actions:** Investigate the origin of the RMM software, and reach out to the end user to gather more information. Update the detection rule if the use case is legitimate and will be reoccurring to reduce false positives.

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
