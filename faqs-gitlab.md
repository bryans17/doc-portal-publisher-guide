?> **Tip:** Click the question or triangle to view the answer.

<details>
 <summary style="font-size:20px"> <b>How do I use SSH with GitLab when using SEED?</b></summary><br>

When Cloudflare WARP is enabled for SEED, you may encounter the following error when attempting to
use Git SSH:

```shell
kex_exchange_identification: Connection closed by remote host
Connection closed by <IP> port 22
fatal: Could not read from remote repository
```

To resolve, please follow these instructions to configure **Git SSH with Cloudflare WARP**. For more information, refer to the [Configuring GitLab > Git SSH with Cloudflare WARP](https://docs.developer.tech.gov.sg/docs/container-stack-configuration/#/gitlab/git-ssh-cloudflare) section in the [Container Stack Configuration](https://docs.developer.tech.gov.sg/docs/container-stack-configuration/#/) documentation. 

</details>

---

<details>
 <summary style="font-size:20px"> <b>How do I self-approve merge requests?</b></summary><br>


!> This should only be set temporarily for the Quick Start guide and reverted after. Allowing
self-approval for Merge Requests (MR) goes against DevSecOps best practices and may result in your
application becoming non-compliant.

Allowing self-approval for MRs involves modifying project-level settings which requires
`Maintainer` role. The following are 3 main ways to achieve this, in order of ease of configuring.

#### Modify Minimum Approvers Required

1. Set the **Approvals required** for the **Any eligible user** row to 0.

    ![Merge approval rules](./images/mra-approval-rules.png)

#### All MR Approval By Author

1. Clear the **Prevent MR approvals by the author** checkbox. 
1. Approve MRs created by yourself.

    ![Merge approval settings](./images/mra-approval-settings.png)

#### Allow Modifying Approval Rules In MRs

1. Clear the **Prevent users from modifying MR approval rules in merge requests** checkbox.

1. Set the **Approvals required** when creating MRs, similar to the above.

    ![Merge approval settings](./images/mra-approval-settings.png)

</details>

---

<details>
 <summary style="font-size:20px"> <b>How do I delete a project or a repository?</b></summary><br>

If the project exists at the root of your subgroup, please [contact us to grant
permissions.](contact-us) to
delete the project.

<!--If the project exists in a [nested subgroup](user-guide/gitlab/adding-developers/?id=add-subgroup)
that you created previously, any user with `Owner` role will be able to delete the project.-->

If the project exists in a `nested subgroup`
that you created previously, any user with `Owner` role will be able to delete the project. For more information, refer to the [Configuring GitLab > Adding Developers to Projects](https://docs.developer.tech.gov.sg/docs/container-stack-configuration/#/gitlab/adding-developers) section in the [Container Stack Configuration](https://docs.developer.tech.gov.sg/docs/container-stack-configuration/#/) documentation. 

</details>

---