## Helm Package Management for Resume Matcher

Automating Kubernetes deployments using Helm charts. Managing releases, templates, and chart lifecycles for scalable applications.

## Access the walkthrough

[![Helm Walkthrough](https://img.youtube.com/vi/FpXploqjdEs/0.jpg)](https://www.youtube.com/watch?v=FpXploqjdEs)

[Watch the YouTube Video](https://www.youtube.com/watch?v=FpXploqjdEs)

---

# 🛠 Deployment Strategy

# Step 1: Cluster Creation
Created a multi-node Kind cluster using `kind-node.yaml`, defining one control-plane and three worker nodes.
<div align="center">
<img src="images/helm/S1 HELM/helm1.1.png" width="250"/>
<img src="images/helm/S1 HELM/helm1.2.png" width="250"/>
</div>

# Step 2: Chart Creation & Structure
Initialized the Helm workflow by creating a dedicated directory structure and executing `helm create resumematcher`.
<div align="center">
<img src="images/helm/S2 HELM/helm2.1.png" width="250"/>
<img src="images/helm/S2 HELM/helm2.2.png" width="250"/>
<img src="images/helm/S2 HELM/helm2.3.png" width="250"/>
</div>

# Step 3: Template Customization
Refined the `templates/` directory and utilized `values.yaml` and `values.override.yaml` for modular configuration.
<div align="center">
<img src="images/helm/S3 HELM/helm3.1.png" width="250"/>
<img src="images/helm/S3 HELM/helm3.2.png" width="250"/>
<img src="images/helm/S3 HELM/helm3.3.png" width="250"/>
<img src="images/helm/S3 HELM/helm3.4.png" width="250"/>
<img src="images/helm/S3 HELM/helm3.5.png" width="250"/>
<img src="images/helm/S3 HELM/helm3.6.png" width="250"/>
</div>

# Step 4: Release Management
Packaged the Helm chart, generated repository metadata, and utilized `git subtree` to isolate the `helmrepo-branch`.
<div align="center">
<img src="images/helm/S4 HELM/helm4.1.png" width="250"/>
<img src="images/helm/S4 HELM/helm4.2.png" width="250"/>
<img src="images/helm/S4 HELM/helm4.3.png" width="250"/>
<img src="images/helm/S4 HELM/helm4.4.png" width="250"/>
<img src="images/helm/S4 HELM/helm4.5.png" width="250"/>
<img src="images/helm/S4 HELM/helm4.6.png" width="250"/>
<img src="images/helm/S4 HELM/helm4.7.png" width="250"/>
<img src="images/helm/S4 HELM/helm4.8.png" width="250"/>
<img src="images/helm/S4 HELM/helm4.9.png" width="250"/>
</div>

# Step 5: Advanced Configuration & Deployment Verification
Resolved GHCR image-pull issues with Kubernetes secrets, verified connectivity via port-forwarding, and confirmed deployment via logs.
<div align="center">
<img src="images/helm/S5 HELM/helm5.1.png" width="250"/>
<img src="images/helm/S5 HELM/helm5.2.png" width="250"/>
<img src="images/helm/S5 HELM/helm5.3.png" width="250"/>
<img src="images/helm/S5 HELM/helm5.4.png" width="250"/>
<img src="images/helm/S5 HELM/helm5.5.png" width="250"/>
<img src="images/helm/S5 HELM/helm5.6.png" width="250"/>
<img src="images/helm/S5 HELM/helm5.7.png" width="250"/>
<img src="images/helm/S5 HELM/helm5.8.png" width="250"/>
<img src="images/helm/S5 HELM/helm5.9.png" width="250"/>
<img src="images/helm/S5 HELM/helm5.10.png" width="250"/>
<img src="images/helm/S5 HELM/helm5.11.png" width="250"/>
</div>

# 📝 Notes
* **Helm:** Efficient packaging and lifecycle management.
* **Infrastructure as Code:** Standardized, repeatable manifest deployment.
* **Authentication:** Secure integration with private container registries.
* **Outcome:** Successfully deployed a production-ready application architecture using Helm.
