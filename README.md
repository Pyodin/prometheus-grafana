# Monitoring Stack with Ansible

This project uses Ansible roles to automate the deployment of a comprehensive monitoring stack consisting of Grafana, Prometheus, Node Exporter, and Nvidia GPU Exporter. It is designed to streamline the setup process and create a robust monitoring environment for your applications, including specialized monitoring for NVIDIA GPUs.

## Features

- **Ansible Roles**: Use of Ansible roles for a modular, reusable, and easily configurable deployment.
- **Grafana**: Open-source platform for monitoring and observability, configured to visualize data from Prometheus and Nvidia GPU Exporter.
- **Prometheus**: A powerful time-series monitoring service, pre-configured to scrape metrics from Node Exporter and Nvidia GPU Exporter.
- **Node Exporter**: A Prometheus exporter for hardware and OS metrics with pluggable metric collectors.
- **Nvidia GPU Exporter**: A Prometheus exporter for NVIDIA GPU metrics.

## Getting Started

### Prerequisites

- Ansible
- Access to a server or virtual machine

### Installation

1. Clone the repository
    ```bash
    git clone https://github.com/Pyodin/monitoring-stack-ansible.git
    ```
2. Navigate to the project directory
    ```bash
    cd monitoring-stack-ansible
    ```
3. Run the Ansible Playbook
    ```bash
    ansible-playbook main.yml
    ```

Once the playbook has finished, you can access the Grafana dashboard at `http://yourserverip:3000`.

## Usage

Once deployed, the monitoring stack begins to collect and display metrics. You can view and analyze the metrics using the Grafana dashboards.

## Acknowledgements

This project wouldn't be possible without these open source tools:

- [Ansible](https://www.ansible.com/)
- [Grafana](https://grafana.com/)
- [Prometheus](https://prometheus.io/)
- [Node Exporter](https://github.com/prometheus/node_exporter)
- [Nvidia GPU Exporter](https://github.com/NVIDIA/gpu-monitoring-tools)
