# Ukboxing Airflow

![Ukboxing Airflow Logo](link_to_your_logo.png)

Welcome to the **Ukboxing Airflow** repository! This is a project focused on the use and configuration of Apache Airflow for workflow automation and orchestration.

## Overview

This repository contains the necessary files and configurations to implement Apache Airflow, a flexible and robust platform for scheduling and executing complex tasks. You will find details about the project structure, initial configurations, and DAG examples to get started.

## Project Structure

```
|-- dags/                       # Directory to store Airflow DAGs
|   |-- example_dag.py          # Example DAG for illustration
|-- plugins/                    # Directory to store custom plugins
|   |-- my_plugin.py            # Example custom plugin
|-- config/                     # Directory for Airflow configurations
|   |-- airflow.cfg             # Main Airflow configurations
|-- README.md                   # This file
|-- .gitignore                  # File to specify files to be ignored by Git
```

## Prerequisites

- [Python](https://www.python.org/) (recommended version: >= 3.9)
- [Apache Airflow](https://airflow.apache.org/) (recommended version: >= 2.5.1)

## Configuration

1. Clone this repository:

```bash
git clone https://github.com/gfechio/ukboxing-airflow.git
cd ukboxing-airflow
```

2. ```bash
curl -LfO 'https://airflow.apache.org/docs/apache-airflow/2.7.1/docker-compose.yaml'
```

3. ```bash
mkdir -p ./dags ./logs ./plugins ./config
echo -e "AIRFLOW_UID=$(id -u)" > .env
```

4. ```bash
docker compose up airflow-init
```

5. ```bash
docker compose up
```

6. Access Airflow through the browser using `http://localhost:8080`.

## Usage Examples

- Check the `dags/` directory for ready-to-use and customizable DAG examples.

## Contribution

Feel free to contribute with improvements, bug fixes, or new features! To learn more about how to contribute, please refer to our [Contribution Policy](CONTRIBUTING.md).

## License

This project is licensed under the [MIT License](LICENSE).
