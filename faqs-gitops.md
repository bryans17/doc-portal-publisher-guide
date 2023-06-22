?> **Tip:** Click the question or triangle to view the answer.

<details>
 <summary style="font-size:20px"><b>Why is my new resource not being deployed by ArgoCD?</b></summary><br>

Resources are seemingly not being detected and deployed by ArgoCD when new manifest files are added
to environment-specific directories in the `cstack-manifests` repository.

The most common reason for this is not adding the resource's manifest file to the `resources:` list
in the `kustomization.yml` file.

If the resource has been added to `kustomization.yml` already, use the ArgoCD portal to
troubleshoot. For more information, refer to the [CI/CD > GitOps (CD) > ArgoCD](https://docs.developer.tech.gov.sg/docs/container-stack-configuration/#/cicd/cd-gitops) section in the [Container Stack Configuration](https://docs.developer.tech.gov.sg/docs/container-stack-configuration/#/) documentation. You may also
[contact us](contact-us) for support.

</details>

---

<details>
 <summary style="font-size:20px"> <b>Do all the ReplicaSets linked to a Deployment mean old versions are still running?</b></summary><br>

No, it does not imply that old versions of your application are not running.

By default, Deployments retain up to 10 ReplicaSets for revision history. This can be configured by
specifying the `revisionHistoryLimit` for each Deployment.

For more information, please refer to the following Kubernetes Documentation:

- <https://kubernetes.io/docs/concepts/workloads/controllers/replicaset/>
- <https://kubernetes.io/docs/concepts/workloads/controllers/deployment/#clean-up-policy>
</details>

---