# tech-challenge-manifest

[![Maintained?](https://img.shields.io/badge/Maintained%3F-yes-green.svg)]()
[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![EKS](https://img.shields.io/badge/EKS-1.30-blue.svg)](https://docs.aws.amazon.com/eks/latest/userguide/what-is-eks.html)
[![Helm](https://img.shields.io/badge/Helm-3.7.0-blue.svg)](https://helm.sh/)


This repository contains the Helm charts for the applications that are deployed in the ArgoCD instances.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Usage](#usage)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)
- [References](#references)

---

### Prerequisites

How to prerequisites for utilization of this repository.

1. A GitHub account.

2. Access to the ArgoCD instances for each environment (DEV, STG, PROD):
    - **PROD**: [https://argocd.tech-challenge.com.br](https://argocd.techchallenge.com.br)

3. `kubectl` installed on your machine. You can install it by following the [official guide](https://kubernetes.io/docs/tasks/tools/install-kubectl/).

4. Access to the Kubernetes cluster where ArgoCD is installed.

---

### Usage

How to use this repository.

1. Clone this repository:

```bash
git clone https://github.com/yourusername/tech-challenge-helm.git
```

2. Change to the repository directory:

```bash
cd tech-challenge-helms
```

3. Create a new branch with a descriptive name:

```bash
git checkout -b my-feature-branch
```

4. Create a new directory for your application:

```bash
cd apps && mkdir my-app
```

5. Clone the Helm chart for your application:

```bash
git clone app/chats
```

6. Add the application to the `values.yaml` file in the `my-app` directory.

7. Substitute the values in the `values.yaml` file with the values for your application.

8. Commit your changes:

```bash
git add .
git commit -m "Add my new application"
git push origin my-feature-branch
```

11. Open a pull request to the main repository.
12. Wait for the pull request to be reviewed and merged.
13. Check the ArgoCD instance for the environment where you want to deploy the application.
14. Sync the application to deploy it.
15. Check the application status in the ArgoCD instance.

---

### Contributing

We welcome contributions! Please follow the steps below to contribute to this repository:

1. Fork the repository.
2. Create a new branch with a descriptive name:
   ```bash
   git checkout -b my-feature-branch
   ```
3. Make your changes and commit them with a meaningful message:
   ```bash
   git commit -m "Add my new feature"
   ```
4. Push your branch to your forked repository:
   ```bash
   git push origin my-feature-branch
   ```
5. Open a pull request to the main repository.

For more details, refer to our [Contributing Guidelines](CONTRIBUTING.md).

---

### License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

### References

- [Helm Documentation](https://helm.sh/docs/)
- [Kubernetes Documentation](https://kubernetes.io/docs/home/)
- [Amazon EKS Documentation](https://docs.aws.amazon.com/eks/latest/userguide/what-is-eks.html)
- [kubectl Documentation](https://kubernetes.io/docs/reference/kubectl/)

---


