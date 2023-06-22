?> **Tip:** Click the question or triangle to view the answer.

<details>
 <summary style="font-size:20px"><b>I do not see any projects, how do I view my project's SonarQube analysis results?</b></summary><br>

Granting access permissions to your SonarQube projects is currently done manually, as SonarQube
accounts occasionally do not get automatically created upon onboarding to SHIP.

For Container Stack to grant permissions, please ensure that you have logged into SonarQube with
your SHIP account **at least once**. This will trigger the SonarQube account creation if it has not
already been completed. After which, please [contact us](contact-us) to assist in
granting permissions.
</details>

---

<details>
 <summary style="font-size:20px"><b>Do I need to generate a token to use SonarQube?</b></summary><br>

No. SonarQube Service Accounts have already been configured for you in the baseline CI pipeline and
will work out-of-the-box.

You will not be able to use the generated tokens as all user accounts do not have permissions to
run analysis on repositories.
</details>

---
