# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: Alert.spec.js >> Alert Handling
- Location: tests\Alert.spec.js:3:5

# Error details

```
Test timeout of 30000ms exceeded.
```

```
Error: locator.click: Test timeout of 30000ms exceeded.
Call log:
  - waiting for locator('//button[@class="btn btn-primary"]')
    - locator resolved to <button onclick="confirmbox()" class="btn btn-primary">click the button to display a confirm box </button>
  - attempting click action
    2 × waiting for element to be visible, enabled and stable
      - element is not visible
    - retrying click action
    - waiting 20ms
    2 × waiting for element to be visible, enabled and stable
      - element is not visible
    - retrying click action
      - waiting 100ms
    17 × waiting for element to be visible, enabled and stable
       - element is not visible
     - retrying click action
       - waiting 500ms
    - waiting for element to be visible, enabled and stable

```

# Page snapshot

```yaml
- generic [aria-hidden] [ref=e1]:
  - banner [ref=e2]:
    - generic [ref=e5]:
      - link [ref=e7] [cursor=pointer]:
        - /url: http://www.automationtesting.in
      - heading [level=1] [ref=e10]: Automation Demo Site
    - navigation [ref=e11]:
      - list [ref=e14]:
        - listitem [ref=e15]:
          - link [ref=e16] [cursor=pointer]:
            - /url: Index.html
            - text: Home
        - listitem [ref=e17]:
          - link [ref=e18] [cursor=pointer]:
            - /url: Register.html
            - text: Register
        - listitem [ref=e19]:
          - link [ref=e20] [cursor=pointer]:
            - /url: WebTable.html
            - text: WebTable
        - listitem [ref=e21]:
          - link [ref=e22] [cursor=pointer]:
            - /url: SwitchTo.html
            - text: SwitchTo
          - generic [ref=e23]: 
        - listitem [ref=e24]:
          - link [ref=e25] [cursor=pointer]:
            - /url: Widgets.html
            - text: Widgets
          - generic [ref=e26]: 
        - listitem [ref=e27]:
          - link [ref=e28] [cursor=pointer]:
            - /url: Interactions.html
            - text: Interactions
          - generic [ref=e29]: 
        - listitem [ref=e30]:
          - link [ref=e31] [cursor=pointer]:
            - /url: SwitchTo.html
            - text: Video
          - generic [ref=e32]: 
        - listitem [ref=e33]:
          - link [ref=e34] [cursor=pointer]:
            - /url: WYSIWYG.html
            - text: WYSIWYG
          - generic [ref=e35]: 
        - listitem [ref=e36]:
          - link [ref=e37] [cursor=pointer]:
            - /url: "#"
            - text: More
          - generic [ref=e38]: 
        - listitem [ref=e39]:
          - link [ref=e40] [cursor=pointer]:
            - /url: http://practice.automationtesting.in/
            - text: Practice Site
  - generic [ref=e44]:
    - list [ref=e46]:
      - listitem [ref=e47]:
        - link [ref=e48]:
          - /url: "#OKTab"
          - text: Alert with OK
      - listitem [ref=e49]:
        - link [ref=e50] [cursor=pointer]:
          - /url: "#CancelTab"
          - text: Alert with OK & Cancel
      - listitem [ref=e51]:
        - link [ref=e52] [cursor=pointer]:
          - /url: "#Textbox"
          - text: Alert with Textbox
    - button [ref=e54] [cursor=pointer]: "click the button to display an alert box:"
  - generic [ref=e56]:
    - insertion [ref=e59]:
      - iframe [ref=e61]:
        - iframe [ref=f2e1]:
          - generic [ref=f9e2]:
            - link [ref=f9e4] [cursor=pointer]:
              - /url: https://adclick.g.doubleclick.net/pcs/click?xai=AKAOjsug0DvpQa1ubBKUmzVfO9uHlqNPwu84FfVtgd6TKqlpAHTLv9mjW4YYfcUP-XDB_W1OPE8IeGycpkFfOr0vhvcvsTRf2fAzgDwns4E_UNB3jRzuOxuS0doT7hgNA-umeXpI4MXzdrIfNsciBiudPjOZuaGIFyW4oge2Mk4E6e-uQNaHGuzOpfiaKEwAwBxHZazufV5ZvnGsAGcbhx6yeh97j4xDX8_SoY0jopQcHcEVON9r8D5ZIARVO95fFpKz-S_ubNdXpNETpbXcQXQKubEXHKCWSAIZo9nMNTvQyrDU9-Sn_hhozUxkdSPdu_-PPD0Kf16peM66r76s7EZ7SqN6Jh_6ooXfJvSwO4DFdFdGOpkG9haBjvxLWNVor06rvbYXgNzoYfF925-mWM4h2oD5z0vQgfzT536AftLLIWhZjflwdyxOrMna6taA1VE4C0jSwT_uipnFkatmGqXAlDxlrhxAUI3KyNgvpxUpXICJpochPFW2JpA6DiDwGOkfBQtL3SSndArq-Y0at3Ow6QCnMDHENixjZM-EplzPIQ0g-xtKDNjSIsxSr4AhLkPBHGpFAdMCT8n5WqiXcFIUCe2Uccb2ApvIwKHfcvDlH8ZMY6iHWASJDjkyFBwBiPVHNqfNEkE4tWQCH2jHBAoLX4u1J2oseAr4-mt3tWJR0B-TsZVAnaVN6dKKzyfKKdDcfFTMw89aS_fTRnMCAm3g6-GlECwLJ-WMxE0-DLy2mhcKyLRZQg8VyKixUJMGhLMCJpvMoL_6odHfklZOm-8ehQILarNlDCla9p1zKGfqLOMnyBAzGhcqip6CCQDFnj9tz-BxkPxm7l4XPIfAFjyo7rXjbAM3ec-WrTS24SQSYsj31U4_tFbnEFsJ8j_b-CJwMPLw3hg4yDY4AzavoONklJpHx8raZU2FzcN7LzSooNRGLiZypeSKf1_W58CabpXnn1lJrfhOYl1TfJEd-kj6GjnqO9x0b-XX2ZHgqXC3GD3knQggMP5olOhFgILGJVbpFz7RRMU9m8gAPKprpM97-X26qQ_bX4B-RlSil8fr-i0QsGkEhYZbBS_jY77rEO0WHk5Mgpjd8GdUTR455BZoWeYOKiLi2XHKPGjpp_8dMPd4z9HujEM5S4fCLeCJ_hBSFJPzaXJkTJJTLTo9ze1m6FwE1be4cX16IjHhPrxnszyoN4RvZ7cpnY0SutJa7PUKiA0wC_cNrl9nIYBuQebcvYfbWw8dmoo4EZugD6bzWGmzcki8aEyV86pO-vuetqwBsRjk7AkktC4N_FBd38Q1FExkBC0Ebr7QNKb3uxGjYq4qdvAgNq52tkCJDxPvWpa5HaF7hyBuJA6y8MKO6PMDegcXYN5TsW_I79LbZk7UgeXj_E1NhH5tJFkJzZ18QVLLcRNMrjsv8evC4gCx-Ma3pY8eJSEOkyU__xAiZ87kiQ7oDysWyq-tyqdGVXQ2o9mc-WJikZJRHOVJjcFhSznggkLWeXzbbR4mdSiwueP1S45LKg9V95Fi7GkTJ9pxBfuxbgHgDxkwW8btnscGH2iwuf-9aoTvCG55lU5GRX8daUWoB2OWYnJG5NGa4qv8Qur2WEprn2lpN3rUpJvfCfCmSZB0PCMUjtj2Ke8H5ZKEE0BQW-dXotlRmdvc3MzV_sUTfLq2X9qZwakDjnKWWrhiX0JH20VNuYEQTN5RCkN-DE9lL0qJ9G8Q_ivXd5-erHOdHlVizA1hoOBCJBiDEk3O5rarIveG1SDuv6B0aJYVebwovTanQ7-vWsHMsJ4xucdoRfLIYRXIcUeEck_StFUDAg5ZZwLkDm4vY4CGFB_4rOFdP7mSdEEhzKKQrRA5EMD6Cq4S0nVh7DoXA7kYSwL8DdCaNBdwPkHjC61XQJ4irHQrkrPEKuQQNh80R1SAuSl1qU7qcVzqnVzOzaRs7h9QXYZr4JdHsROarwJHp1XfvMtQuhDrYtd-BYaeARmNqZjt5AdwPHIeveSrbaPapMRwUWW8Reu8CcQXh22OW9uXf-cR0GnL&sai=AMfl-YSs3KXFy79FHTZva_hzVCkIPLV4FWLrse-x7wUkBJtQqg9DkrAajg6LvU2tM5Gu2MHNXyYsDIpeOLAVYSgYz3TQQjKn94b4qBrr4FGGMPTN0l8jUNLgFwcoRgAgI3ISpsPVRhQwsvN0PUVFqWVuz5eF1PRBdtmM0EjXHH5tUPduJWMNGQ3m1uFpYynu00k3AmZ_fHEa6RN5eLWbE8pCrkKlWRdZhMDRaOraxHzpI6aoqf9PNc_SuiFteNwy50Bt3mBvyhjk6DhawJSdlUw-KMRR-dmQbJlHY3kiYqUZGbm8eVbtBz2cVCAB9CwKw1CpQuWEEIZIoQn2krljfNzYVZpfEYoThnQcMORFCOXdwC0rGENUEzuH6JLGfPv_rcUy9HbYJIpKenDqxIn2FPcX0_cbQLoQq8C53ToJqO2MtR-k5BhaLv8T6yeJjb2Bc4kZMP6RH_N0EaaKdcUMKNlxo-kXebj7J6HQ9TRihkacj8rn--M-vQw5izEFuh2eMGLyoBSAHkEkw-k3AL_7kpy1sKZc8JTU5gmEUUABprU7TIAyVznqeAg_GSdc7FBbOZhippwyVMC-dAF0wPUDsSHy7ClWvg-44MWgIofFc7HQNuKznNn4Ij-QFbv6jm84Mj24yOP6TGUS6e2fZIfqYYvuIkqi_6bp-puTPRhr0MILVRnDTs5T4dXOO7VrzieGRChjHEwFng4dn69uujvVNZMaaTz5OGDugUVMvFWxoMuWSJNC7Qkhd6EnLA2hkmPg3zZ3xQ2EYJAiHGwJ7Gc9CH5P3K08v8YV0rd2INyXaWSye1AKHtUOjZWGOgBtCOAjU7sOS06AAHtNeoYjbUVm-W5RBlTG5tvgMbZ29jcRW-Lui3UJ5mf9Dpz8_9DlKvCFjPJVyirY99OQhCQlsRJ6G7xyqA5tRV6aI_XXfNCTCt-DJefwuGdXQidR7F34CVbtcCfrzqBtZmDvDF9OiNDVC0M_85cxcOLh7UieKYYfws5N-7Jgp-PzPjM&sig=Cg0ArKJSzAYqUO_aNLqv&fbs_aeid=%5Bgw_fbsaeid%5D&urlfix=1&adurl=https://www.visitdubai.com/en/dubai-ready-for-a-surprise%3Futm_source%3Dprogrammatic%26utm_medium%3Ddisplay%26utm_campaign%3Dseasonalaonsasia%26utm_term%3Dind-en_q4brandambassadorbanners%26utm_content%3Dconsideration_banner160x600_OPXInmarketAll%26dclid%3D%25edclid!%26gad_source%3D7%26gad_campaignid%3D24320247089
              - img "Advertisement" [ref=f9e5]
            - generic [ref=f9e6]:
              - generic:
                - generic [ref=f9e7] [cursor=pointer]
                - button [ref=f9e12] [cursor=pointer]
    - insertion [ref=e64]:
      - iframe [ref=e66]:
        - iframe [ref=f3e1]:
          - generic [ref=f7e2]:
            - link [ref=f7e4] [cursor=pointer]:
              - /url: https://adclick.g.doubleclick.net/pcs/click?xai=AKAOjsvyqUaJEYTUsfKpn0r72rHXN2JgLcGdVyETa6XWi1sJTj9wrOQJ05yPCQdaDOkqDJ-ZW7uoBcUEroi6_TBZScOQMJD0LKZOFZxrq_CrIn5cxytWAJzjZ-O6nmI7QDFlPbR_rFi4VhaJD6vSwBxBgkueFcMyD8LX9fXEwFcNgyq0gbRCnNyhBhZkj3Rvpvps2kZ4cwm8XZuQrT_pvyPeVAnmo7Dj7Ukif7iI7Qhv3bvAmqshW7D9ahSLVLbE42zU-EnUEoYiquYbM6beDACZkVtbyO1ZvQ3YQKdwC3ysEDNz3bA_fOlMAcmFL_Pp3nMQB7nH57AjIW7MmMvQmsPJtpY4pPkd0lCflIhM5SLPTf1hINIEP4pN-MyfK5X61isGdtXKgK_BEoER1nn-fpc4vmybi6lbTsBHPd_RbSsSnWPm9khfyOof-CCl3UAoj-scbwV13QxV6ymtcly27TV3PGQuOH9qe2BT4KDFNNNRlC_6TcFGZZb5RX-HvlfLNkAmKtZKxesrBhyXtrTzA1n4e8pTzvR7po4RdlQtQ2IdOy7NUhdRyaKdvp2wMqyi5OCUMLz4VG8qZiGPYvX8dbmLBsyb8wzf0T_sqq8ajWnUuYpoy-w_vueSYYHoqYJjB13rjRuBpTnyAZ3TnW1OoCNkMeX-twGejXBenw31iFnWAo-3Bvso5t2a3gX2f8xnn_SP0IntKpyX0yt3V3ADqUKsTZ_BkaVGSw_FUhVA4pCY7J7QqNCzxWenZyevc7tvPC5eaUeNRCD8HZ7rtENaI5d1iSZs4Rb4wk3WZIbWcipPLWKBgwMrsxIdKT4J80zsb5Jsiaczlh1KS3DfcZRSMTyJTNSMdiPhiU4pchuwyNYXq4NosDuZLRHrprBGt8mCDJihs5JwKKZorSGUoRt0AM3ju7lGKhQhTqhxWfYoLZoVp11mkFUa3tU-aV3dfYIduBpsR78NaRGH3dPMM3g9qYK7Dqm7ttbE8NOOfX9849w4HX4-bDtqYlEydKhDj6AEbskvihfVtDz656sngwweG-iq3s_szcdRpL00jvguPP0bOSk1uHLkmaxZ-n2nJ9u0kbvnunmdHYo2HlyBp7BI85R5nW33Z9Q-eRgzcpf8L8huT0wtvlZMpjDu8Y4QsZgYd3CEt-jKHJCcb8f-nRfKwy8P8CBf1YdfIQdr5GadJHVGCK1aBWeyg9rER3lZ9hsdS_stjfX_EhWzomaXhEJ1ODOG78myLHAFunLfVROCfC5xSf6TMEi0nb0V9UC6YsD43783VrFn6WZ6Mrk9w_cgpYbWIPAFo2XcypawgUZHcuilusv9U7qkDkOV3WQ5_E1LjQXMtdzwtvE59P0llSAeNUVy9LWR-hJTpyb_tCwgiNisdzUdDEs0uTzuAQ2ndRG_AHYqSJ_4xvyPi9Wxa4ELyp4UddfczTCBmYFZ-nYKdEgwdJzYdvY4ZtT6m8iuHlV_tXGGy4cnMjiFUlvAPMX26MSiIfmen7oFcek9iN6LPf7VRef2Ceut6ET5ZYabXE2oStd6dY-DVuARqXqGJg2f1B0xdeEsSxDF5_pUWrpPMmGOIuQrdDkv45fqy3JIK2TIQ_uPSUVos-3xzThV4ETwoF4TrA0imVdU9pTYjLBLLSWK38IufHpibfWH0PdfSlQUliI05LL9BlgEBIvWWvFYsTJJpUH5ZFbI1bMI9UUa2wZEwg_EPq39WEZtGfWiIHHFInck6cGvYUz62QMI82PvFxkDt9t5ixRvsBSQx7JIkFk9hpirW63D3CBQup09wgYFr_GkEB57UKQGIOLOwDwUMrdF_un7IwB9s9OorRg3PA0PNcTpjpbbUlKdBmA_iCqPe5ubGJ2BgYZ_dwB_3fjPsYV7LJpD1GfmlliGH6iT32fraOVMs78LE1J4jgs68EvY3DVqi3Ku4vNf41iY9dB2L-xzSn1Qe66BVm-y6rUvUaxkqPJ0sAHiW8EP6zNmCJWNeBEEL9biXULHx7YUIShbkVlgaIdlRQzO6-LcQKsP-mTuGE9G4n7za3qq56Gq&sai=AMfl-YS0xof3mrAjsesDvazIpbcSBjt90fEx2j-cpbZD_PQdQogfqJvhjI_oxHtUSTDXGkAeBfM8A5Y4G56kbYdSWt9CI9IrmLY8ogE94Tt4PD1MKegDwc2n9REvkXRdM-iL-eO8LLj2_9lo5dWFy9VtQggQUW1jobtciuDEb96n4egFyLFBwZ2wASuQ6cOH200rMdGQj6RlGnFEfgvYlyMIaVvNeAixsGmKvTAmj-aB3L43LYh7-Oloxt5SEH49MZO28qOcXjJKwJ3vYmKcHjOVzpp69Osc8T9bRIqrSlqkRytRxEhTiXnCa8-WOCzQm3zvtmbMUT9t3xd2StMDycmOdSxwBvODYKp7eH3Lk_xX5KiyR5d4aGsNrAeOOUFmr2T_cDQutj5mtfXpGFaoIQFe6vsHJa_KMdvN0e4eolVHdMjAwr8Xf9iNMmJfqjzJ1UmamwKm2tuzm4sjlV2ewrvUU0RAwkK1nBzYgcXGbyHzxoThRs4HEwErm4WAeAxxrVv8TTEflM2ajqFfPgOEGcAQAoJ8k7ZRARoXnQG-kIL6dgTpo2P-GyFgBEkoT0LR5t0TZ8NX7Ci3759WUKvhw0NQbjPq42H2Y_LDdMq_XY6az2zAufTBQqWoKPWV-l_x0DFixwgbb2t4MdkYC42BH4katzYeS9agkC1rKDIRquPU_jLZsMdQMH8ZHTq_dHDfZAvlUJWoqszgsrbHqKDEUSsLO3zAORHUs9NWqNH_m85R-0fute0zAX9Ag87qhM3OsAQZx6V0gWqtEr0MA4mKcaom4NqEA9PW_aBEEMztgmj2Qw8AcMkSo-5qNjTBwReY8CsJCB_0quaVzhhl040U1Lq_8iBaYtAZ87vycaGAhyT1orh3Iw2NPyRFOp2PnLOBI6h3Hz402Fe3wxxa6F4EflM7XiyvptvHc8Wh3slcXbLrM0q8noIpdFjhKP0g31_wL8-_rWViDSqOykbcB-fQjudjXcKmLpcwpJkcerEYzp5GpcUwX4EkBzk&sig=Cg0ArKJSzOzwd9XXmXGb&fbs_aeid=%5Bgw_fbsaeid%5D&urlfix=1&adurl=https://www.visitdubai.com/en/dubai-ready-for-a-surprise%3Futm_source%3Dprogrammatic%26utm_medium%3Ddisplay%26utm_campaign%3Dseasonalaonsasia%26utm_term%3Dind-en_q4brandambassadorbanners%26utm_content%3Dconsideration_banner160x600_OPXInmarketAll%26dclid%3D%25edclid!%26gad_source%3D7%26gad_campaignid%3D24320247089
              - img "Advertisement" [ref=f7e5]
            - generic [ref=f7e6]:
              - generic:
                - generic [ref=f7e7] [cursor=pointer]
                - button [ref=f7e12] [cursor=pointer]
    - insertion [ref=e69]:
      - generic [ref=e72]:
        - heading [level=2] [ref=e74]: Discover more
        - link [ref=e75] [cursor=pointer]:
          - generic [ref=e76]: Automation Software Testing
        - link [ref=e80] [cursor=pointer]:
          - generic [ref=e81]: Test Automation Tools
        - link [ref=e85] [cursor=pointer]:
          - generic [ref=e86]: Alert Box Tutorials
        - link [ref=e90] [cursor=pointer]:
          - generic [ref=e91]: Confirm Box Examples
        - link [ref=e95] [cursor=pointer]:
          - generic [ref=e96]: Software Testing Services
        - link [ref=e100] [cursor=pointer]:
          - generic [ref=e101]: Automation Testing Training
        - link [ref=e105] [cursor=pointer]:
          - generic [ref=e106]: Automation Demo Access
        - link [ref=e110] [cursor=pointer]:
          - generic [ref=e111]: Register Automation Users
    - insertion [ref=e117]:
      - iframe [ref=e119]:
        - iframe [ref=f5e1]:
          - generic [ref=f11e2]:
            - link [ref=f11e4] [cursor=pointer]:
              - /url: https://adclick.g.doubleclick.net/pcs/click?xai=AKAOjstKbVPEDg-C2CC28OdgX5pCEAvRAVQICXVMWPvOFw2YZY2HR62j3fC9ja2sGBgvUGxiTlPO6lXpL_FPWcv26_uBO0oKnHW6ptxnxoOvksJlJNl6a82mKJHA9jEuB8npAI9REFJWYEAVCMoWfx7j37TJVBcXUDgnxs1bhQwR2thy_AOpCLv2VdFOqxqsSOq9NUtk6YqVkCfT__ZYetma0aJlmhBJ_VpKLdQwsjaTg4U4zmWTSUWYDKotMEfm4mEduB6I74ra7zMgFf3pui5laTSBjZVwarloaJ49DU-KHz0Vrxijqcbujcy6XKGSJEGaRLwxRAReRgV8TXFTHSl0li1Lank53eUpAcor1rYXzUNWrT-iJwGCVI_XvZ-NAvLKbs_mWMA6SUofnZCvtfpSk5nPg_e1G_TwbVCKcPW_XedfGXrcCd7Qjmv21n5IKzvkSIon-s7L3Qa90LFCvC_BVLzMMiJ4likCiew0VjQURULD9vyH1Rx5_Xoe2gA1WAwuAvhY6XfLTVAaRmTaLS0hxsGoNERc2aXI3g8atU1gOXLmOlq7ri62niNzpsl9f37ZkyCfUOeCgvK0CCALRhRsAKWlLr1I-ukkz66iaS2rJ3Zbo9VZCIsOPQcz2ZjZmXIw7CO0kXNzGGRQD8sFaaEEKy1yBcY5DssZC0JMj6EsIToBbSkIi0g4YFyEEwtKcIAenRA21ykOqnYH7MFTskb5AEo-yXfuIGHLWzTnS_UgRnhR-CIJ38imahcswTjYtrXf38bG3euh3fHmZ13DC5hWZ0-Tj9hGFTf8fvAslntyMGJ2ZVu3xIUJJkdNr_fcLb4Ii951BO7kv_e6YVz4uw7rUzuc9-uGBy22yZcrDLK7xlU0nlNpwAqeteZhcAe58rrvk-540KEWcElW5QutmJMG1aCW_SX2CK1bq-r-qunqsyMKgnWUb7VXyR_xEccCCyhiutDlJXDe-8ESGnNxrwVQlGYusR8J_IsL_c_qqK7ASDhS1p2wgNey5a_eZU_zRmXV_G7tgd1lIruu8O2xHhI6DPsVYQnJq2XxxfFmF5gbtkgqkOcY2GpZTrwTwHBRdXj2Xqg_Utcho2B14iEccS8Qza_RfxowU5UoKUWAv_543O3XbkvJaggV5MngUVgur-UHcy68FD16J-c0pV4YoeJIS37CbmTq7E4Xv2RC9DJpPXB2lHGIxnM7QK1wozmqpHli_BYvxic97CqTkluM-Mpq2zHtOd4KdXYIHRfg_gXhQjVDC3rW-JP1u8m55XOhuU7LZiSaHoDVYPjW5QiZ1lizae-H2HbScVHSyV3_b64u8LxDxPSXA8MF_GoeruZP8RmLQ25UDJNm2i4VjJE9YNNtyLGpJAfBoc6dEn7Ws8y5IO7kvq5ldzAGb1bu4-seWmG2q7mB1p9wzaAkZ14LKPjFXM9LOzQLJDry1ZOpTp4UyyUtYTf8D9tVjupclJdDbscNbg552grJCL73qeJc4zB5OLEV5G4tJ5cg6ksfkP_6-bgXXbb_Do9j-bkwlRs3tIl-SZbvhJIeZOTtVEkKvhbFcEIN4Qnq3lW8anU66JuYpS4iQatfHHUPqRm8yv5gqtS9SB0N6J2IHBzRyiIH64ULvO4te0dayebXpG0TnICnM3gKbiCQ9juWI0HMI48-s7qrQnYt5C_drVeHktu5EV_UVjyHEYQBJ8BeZGyK5Jmq711QUCMMA0UY7ARU-Hu_4_lE0s7In-e0-jlfKOFAYP_WPBTklmVuy2tHfGvj5PFO60JkXKi2cwnOJGMttuxGd6Am2iieXZrSYhCdUnFG2cYckSci81WEdKP_GDQEcPYGFELXvv5NLNwzrqJrYU0yFK-K0YW8H-tzB5Lqqd89UEbjtsRcYQX_GmMLZU8monvJDZ7HI623-ZSSuJ2gUlOgCyup-D8vzUfReLXM0_GRYm8w6ggAQKlzCC3r7ZCOlg0eZ7tsKljnW6NDcLOGF66VNWFNVvdui8h2llEpM8ArOQLJFm9DiMB2jdFKEqddWMlfpReVX1kHaf5b0WHqhbUJRnryQ_vBhiEfR7s&sai=AMfl-YSzOZ4ytu8p6MejABzzLhv4SFdLnbzMHd0D3TuXmRgfIe17hRvRXx0Rv6cezweg4RQ5iVkE-vGlHyFHZtqCf6R3EYgNOuyTauwkO24f-y-6BZNSRjM0Srzhtxl1B4cgjHrhOhu3tyhVU9Qnwm_YopI6j7Nuzuqjz1YfHFXJ35VafhfeCCXT88CyC3tgZp_m2RWi27WVCanJ_o4WVDSroAnP73spHGRY8rP0Shr1tK1nj-HVkumXejcqoPkQ40zgnV-GT5zJapuA2sKIP1vX8Fc64clwT-pIBR2Ui7ECgWF5g8PpJpccmTTANtUEcWBWLIRs1AS2cErpXPCgk49otz_WYxQztv3IHjfe3XD4Morv6zv-3-lWwSsuaiCsolPCDQ9zvEoaPfxSHxwxKGGX3Pd315JlgjRucwtDjbt9-srODTtrlI_FnrHPlhTkLPQyGEFFUH76Gy62QmpMu-fO_3yiOXoqXnF7cy3gceAXn3rrHUb6n9DARFtzOLs-JKvYO9LrbeOP_U8nNk0uXv6mRlXBkRNdef-_V-0qklqnNoLOPEji5YjCdLInO5rXVieIuoI-YAOIdnbQD73kXQ5LpM50ZNiNy_F5sggVzS2AoOIEn4prxe4tr4QZkrLjHFj0etKQ46ohflodTylYd_gHJcyrmVeaRMalxg6_77TdiLd-0IP3cRh9fY9HkBtv3NbAS9PltwFtJaxePv3HlDlIAkPGUKkzalft5a_SchwlfRvSLFzDMJTD4s7o_SpujzfOPueMxWBbus_oCKoI3VhzZ93KUeX9_Kjyq5YsVyMoDLkphUJ_5_EPOdVHxsV3vai2RKJJO-waQsOhf1rrcVleiGOXWBvSfIWixWT9jBTq7zIQsUl_fWtpy2sirFEFc24w6Qc1vuYjA72vo7qxujU2reRIq2SX3yFA9QsBmO00-GWrR-i4CuEkoPLsHPGft2BA2nIaBmm6s7GqGFydNE8lGzyR4wmyivcU3rXsOipT7NP8UB35GgA&sig=Cg0ArKJSzBTvEXhTQ9tu&fbs_aeid=%5Bgw_fbsaeid%5D&urlfix=1&adurl=https://www.visitdubai.com/en/dubai-ready-for-a-surprise%3Futm_source%3Dprogrammatic%26utm_medium%3Ddisplay%26utm_campaign%3Dseasonalaonsasia%26utm_term%3Dind-en_q4brandambassadorbanners%26utm_content%3Dconsideration_banner160x600_OPXInmarketAll%26dclid%3D%25edclid!%26gad_source%3D7%26gad_campaignid%3D24320247089
              - img "Advertisement" [ref=f11e5]
            - generic [ref=f11e6]:
              - generic:
                - generic [ref=f11e7] [cursor=pointer]
                - button [ref=f11e12] [cursor=pointer]
    - contentinfo [ref=e121]:
      - generic [ref=e123]:
        - generic [ref=e124]:
          - text: "\"@ 2016\""
          - link [ref=e125] [cursor=pointer]:
            - /url: "#"
            - text: Automation Testing
          - text: "\"All Rights Reserved.\""
        - generic [ref=e126]:
          - link [ref=e127] [cursor=pointer]:
            - /url: https://www.facebook.com/automationtesting2016/
            - generic [ref=e128]: 
          - link [ref=e129] [cursor=pointer]:
            - /url: https://twitter.com/krishnasakinala
            - generic [ref=e130]: 
          - link [ref=e131] [cursor=pointer]:
            - /url: https://www.linkedin.com/nhome/?trk=hb_signin
            - generic [ref=e132]: 
          - link [ref=e133] [cursor=pointer]:
            - /url: https://plus.google.com/105286300926085335367
            - generic [ref=e134]: 
          - link [ref=e135] [cursor=pointer]:
            - /url: https://www.youtube.com/channel/UCmQRa3pWM9zsB474URz8ESg
            - generic [ref=e136]: 
```

# Test source

```ts
  1  | import { test } from '@playwright/test'
  2  | 
  3  | test('Alert Handling', async ({ page }) => {
  4  |     await page.goto('https://demo.automationtesting.in/Alerts.html')
  5  | 
  6  |     await page.on('dialog', async (dialog) => {
  7  |         await dialog.accept()
  8  |         console.log("Simple Alert:", dialog.message())
  9  |     })
  10 | 
  11 |     await page.locator('//button[@class="btn btn-danger"]').click()
  12 | 
  13 |     await page.locator('(//a[@class="analystic"])[2]').click()//show alert button
  14 | 
  15 |     // await page.once('dialog', async (dialog) => {
  16 |     //     await dialog.dismiss()
  17 |     //     console.log("Confirmation Alert:", dialog.message())
  18 |     // })
  19 | 
> 20 |     await page.locator('//button[@class="btn btn-primary"]').click()
     |                                                              ^ Error: locator.click: Test timeout of 30000ms exceeded.
  21 | 
  22 |     await page.locator('(//a[@class="analystic"])[3]').click() //show alert button
  23 | 
  24 |     // await page.once('dialog', async (dialog) => {
  25 |     //     await dialog.accept('Hii Buddy')
  26 |     //     console.log("Prompt Alert:", dialog.message())
  27 |     // })
  28 | 
  29 |     await page.locator('//button[@class="btn btn-info"]').click()
  30 | })
```