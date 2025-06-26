# Getting Started with Vantage Compute 

Welcome to the Vantage Compute Getting Started repository! This project provides multiple ways to begin using Vantage Compute in HPC and cloud environments. Choose the method that best fits your infrastructure and automation preferences.

## Quick Start Options

- [Manual Install](#manual-install)
- [Ansible](#ansible)
- [Terraform](#terraform)
- [Juju](#juju)

---

## <a name="manual-install"></a>Manual Install

For step-by-step instructions on installing Vantage agents directly from PyPI or Snap, see:
- [Manual Source Install Guide](./external_integrations/maunual/source_install.md)
- [Manual Snap Install Guide](./external_integrations/maunual/snap_install.md)

---

## <a name="ansible"></a>Ansible

Automate agent installation and configuration using Ansible roles:
- [Ansible Snap Role](./external_integrations/ansible_snaps/roles/vantage_agents/README.md)
- [Ansible PyPI Role](./external_integrations/ansible/roles/vantage_agents_pypi/README.md)

---

## <a name="terraform"></a>Terraform

Provision and configure agents using Terraform modules and examples:
- [Terraform PyPI Example](./external_integrations/terraform/examples/vantage_agents_pypi/README.md)
- [Terraform Snap Example](./external_integrations/terraform/examples/vantage_agent_snaps/README.md)

---

## <a name="juju"></a>Juju

Deploy and manage Slurm clusters and Vantage agents using Juju charms:
- [Juju Slurm Charms & Vantage Integration](./external_integrations/juju/README.md)

---

## More Information
- Each subproject contains a detailed README with prerequisites, usage, and troubleshooting tips.
- For questions or support, contact Vantage Compute <info@vantagecompute.ai>.
