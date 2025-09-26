# PiHPC  

[![Stars](https://img.shields.io/github/stars/calvindseamons/pihpc?style=social)](https://github.com/calvindseamons/pihpc/stargazers)
[![Forks](https://img.shields.io/github/forks/calvindseamons/pihpc?style=social)](https://github.com/calvindseamons/pihpc/network/members)
[![Issues](https://img.shields.io/github/issues/calvindseamons/pihpc)](https://github.com/calvindseamons/pihpc/issues)
[![License](https://img.shields.io/github/license/calvindseamons/pihpc)](https://github.com/calvindseamons/pihpc/blob/main/LICENSE)
[![Last Commit](https://img.shields.io/github/last-commit/calvindseamons/pihpc)](https://github.com/calvindseamons/pihpc/commits/main)

*A Lightweight Mini Supercomputer Testbed*  

PiHPC is a **barebones, lightweight high-performance computing (HPC) cluster testbed** built for experimentation, demos, and hands-on learning.  
This repository serves as a **launchpad for HPC systems design** using modern infrastructure tooling such as **Ansible, Kubernetes, SLURM, Splunk, and Grafana**.  

Think of it as a **mini supercomputer lab** you can run anywhere — perfect for testing configs, workflows, and monitoring pipelines before scaling to real HPC environments.  
O.o

---

## Features  

- **Infrastructure-as-Code** with [Ansible](https://www.ansible.com/) for cluster provisioning  
- **Containerized workflows** via [Kubernetes](https://kubernetes.io/)  
- ⏱**Job scheduling** with [SLURM](https://slurm.schedmd.com/)  
- **Observability stack** with [Grafana](https://grafana.com/), [Prometheus](https://prometheus.io/), and [Splunk](https://www.splunk.com/)  
- **Scalable design demos** — networking configs, storage backends, and cluster layout examples  
- **Pluggable examples**: toy workloads, monitoring dashboards, and cluster workflows  

---

## Repository Structure

```bash
pihpc/
├── ansible/       # Cluster config + provisioning playbooks
├── kubernetes/    # Manifests, Helm charts, containerized HPC demos
├── slurm/         # SLURM configs, sample job scripts
├── monitoring/    # Grafana dashboards, Prometheus, Splunk queries
├── demos/         # Lightweight HPC-style test apps and workflows
└── README.md
```

## Getting Started  

### Prerequisites  
-  Linux (Ubuntu/Debian/Rocky recommended)  
-  Python 3.x  
-  [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/index.html)  
-  [Kubernetes](https://kubernetes.io/docs/setup/) or [Minikube](https://minikube.sigs.k8s.io/)  
-  [SLURM](https://slurm.schedmd.com/quickstart.html)  

### Setup Steps  

```bash
# Clone the repository
git clone https://github.com/<your-username>/pihpc.git
cd pihpc

# Run base Ansible provisioning
ansible-playbook ansible/cluster.yml

# Deploy Kubernetes components
kubectl apply -f kubernetes/

# Launch monitoring stack
kubectl apply -f monitoring/
```

### Example Workflows
- Submit a SLURM job to run a toy MPI benchmark  
- Monitor cluster health & metrics in Grafana  
- Send logs and job events into Splunk for indexing & searching  
- Deploy a containerized workload with Kubernetes and compare performance vs. bare metal  

---

### Toolchain References
- **Ansible** – Automation & configuration management  
- **Kubernetes** – Container orchestration  
- **SLURM** – HPC workload manager  
- **Grafana** – Dashboards & visualization  
- **Prometheus** – Metrics collection & alerting  
- **Splunk** – Logging & observability  

---

### Goals
- Provide a sandbox environment for HPC concepts  
- Explore modern DevOps + HPC workflows (containers, observability, IaC)  
- Share config examples for reproducible, lightweight clusters  
- Serve as a learning resource for HPC engineers and enthusiasts  

---

### Contributing
- Contributions, PRs, and suggestions are welcome!  
- Got a new demo workload, monitoring integration, or optimization tip? Open an issue or send a pull request.  

---

### License
MIT License – Free to use, modify, and share.  

---

**PiHPC** — because sometimes you just need a tiny supercomputer to play with.

