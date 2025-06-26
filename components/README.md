# Vantage Compute Components
The Vantage platform consists of multiple python apis and clis that enable its functionality. These services can be deployed with or without the Vantage platform.

## Jobbergate
Jobbergate is a job submission engine for Slurm that supports SSO authentication and permissions control to manage job submissions across multiple clusters and clouds. It provides a unified interface for users and administrators to submit, monitor, and manage jobs in HPC environments.

The jobbergate project is maintained at [https://github.com/omnivector-solutions/jobbergate](https://github.com/omnivector-solutions/jobbergate).

### Jobbergate Components

Jobbergate consists of several components, each serving a specific purpose:

- **jobbergate-cli**: A command-line interface for users to interact with Jobbergate, submit jobs, manage job scripts, and view job submissions.
- **jobbergate-api**: The backend REST API that handles authentication, job submission, job script management, and communication with Slurm clusters.
- **jobbergate-core**: A Python library containing core logic and utilities shared by the CLI and API, such as data models, validation, and helper functions.
- **Vantage Compute UI**: A web-based graphical user interface that allows users to interact with Jobbergate and related services through a browser.

---

### Jobbergate CLI

The CLI provides a convenient way to interact with Jobbergate from the terminal. It supports authentication, job script management, job submission, and querying job status.

* PyPi [`jobbergate-cli`](https://pypi.org/project/jobbergate-cli/)

```bash
python3 -m venv venv
pip install jobbergate-cli

jobbergate login           # Authenticate with SSO
jobbergate job-scripts list        # List available job scripts
jobbergate job-submissions list    # List your job submissions
```

---

### Jobbergate API

The API is the core backend service for Jobbergate. It exposes REST endpoints for authentication, job script management, job submission, and querying job status. The API is typically deployed on a server and accessed by the CLI, UI, or other integrations.

- API Documentation: [https://apis.vantagecompute.ai/jobbergate/docs](https://apis.vantagecompute.ai/jobbergate/docs)

---

### Jobbergate Core

This is a Python package containing shared logic and utilities for both the CLI and API. It includes data models, validation routines, and helper functions to ensure consistency across Jobbergate components.

* PyPi [`jobbergate-core`](https://pypi.org/project/jobbergate-core/)

```bash
python3 -m venv venv
pip install jobbergate-core
```

---

## License Manager

The [license-manager](https://github.com/omnivector-solutions/license-manager) is a custom license-optimization middleware that integrates with Slurm to enhance license scheduling for HPC environments. It ensures efficient allocation and tracking of software licenses required by jobs.

### License Manager Components

- **lm-cli**: Command-line tool for managing licenses, viewing license usage, and interacting with the License Manager API.
- **lm-api**: REST API backend for license management, providing endpoints for license allocation, release, and monitoring.
- **Vantage Compute UI**: Web interface for managing and monitoring licenses alongside other compute resources.

---

### License Manager API

The API provides endpoints for managing software licenses, tracking usage, and integrating with Slurm job scheduling.

- API Documentation: [https://apis.vantagecompute.ai/lm/docs](https://apis.vantagecompute.ai/lm/docs)

---

### License Manager CLI

The CLI allows users and administrators to interact with the License Manager from the terminal.

* [lm-cli](https://github.com/omnivector-solutions/license-manager/tree/main/lm-cli)

```bash
python3 -m venv venv
pip install .

lm-cli login               # Authenticate with SSO
lm-cli licenses list       # List available licenses and usage
```

---

## Clusters and Clouds

Clusters and cloud accounts can be managed from within the Vantage Compute UI. This allows administrators to add, configure, and monitor compute resources across on-premises clusters and cloud providers.

- **Clusters**: [https://app.vantagecompute.ai/compute/clusters](https://app.vantagecompute.ai/compute/clusters)
- **Clouds**: [https://app.vantagecompute.ai/admin/cloud-accounts](https://app.vantagecompute.ai/admin/cloud-accounts)

---

For more information, please refer to the documentation links above or visit the respective GitHub repositories.