?> **Tip:** Click the question or triangle to view the answer.

<details>
 <summary style="font-size:20px"><b>How do I log in to TechPass? I'm facing errors when logging in.</b></summary><br>

You should be able to login to TechPass from an Internet Device. Only the TechPass portal requires
GSIB to access.

The following are 2 of the common issues faced when attempting to login via TechPass.

#### Authentication Attempt Failed

Upon entering your email, "An error occurred" message will appear, stating that the authentication
attempt failed and with `Error details: Unexpected SAS response status code`.

If you encounter this error, it likely means that the Multi-Factor Authentication (MFA) has not
been setup for your WOG account.

Please refer to the [TechPass User Guide](https://docs.developer.tech.gov.sg/docs/techpass-user-guide/#/support/signinissues?id=authentication-attempt-failed)
to setup your MFA.

#### Unexpected Verification Code

Upon entering your email and verification code, this error is shown: `You didn't enter the expected
verification code for this username. Please try again.`

If you encounter this error, it likely means that the wrong verification code was used.

In your Microsoft Authenticator app, there should be 2 entries:

1. SG Govt M365
2. TECHPASS PROD

For this login, please select the "SG Govt M365" entry and use the verification code displayed to
login.

</details>

---

<details>
 <summary style="font-size:20px"><b>How do I switch TechPass accounts?</b></summary><br>

After login with TechPass, this error is shown (`AADSTS90072: User account does not exist`):

![AADSTS90072](./images/tp-session.png ":size=75%")

If you encounter this error, it means that you are logged into another Azure AD account that is
different from the one onboarded to Container Stack.

As of now, there is no easy way to switch accounts or logout of session within the TechPass
login pages without clearing cookies and cache in your browser. Here are some working
alternatives:

1. Use incognito / private browsing modes in your browser
2. Use different browsers for different accounts
3. Use different browser profiles for different accounts
4. For Firefox users, use the [Containers add-on](https://addons.mozilla.org/en-US/firefox/addon/multi-account-containers/)
   and have different containers for different accounts
</details>

---

<details>
 <summary style="font-size:20px"> <b>How do I reset my MFA?</b></summary><br>

In the event of changing mobile devices, you may need to reset your multi-factor authentication
(MFA). Please refer to the
[TechPass User Guide](https://docs.developer.tech.gov.sg/docs/techpass-user-guide/#/support/account)
to reset your MFA.
</details>

---

<details>
 <summary style="font-size:20px"> <b>My account was disabled. How do I reactivate my account?</b></summary><br>

Your TechPass account will be disabled after 90 days of inactivity.

To reactivate the account, please [contact us](contact-us) or submit a
[TechPass Service Request](https://docs.developer.tech.gov.sg/docs/techpass-user-guide/#/support/overview?id=need-more-help).

</details>

---