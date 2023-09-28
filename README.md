# Ukboxing Airflow

![Ukboxing Airflow Logo](link_para_seu_logo.png)

Bem-vindo ao repositório **Ukboxing Airflow**! Este é um projeto voltado para a utilização e configuração do Apache Airflow para automatização e orquestração de fluxos de trabalho.

## Visão Geral

Este repositório contém os arquivos e configurações necessárias para implementar o Apache Airflow, uma plataforma flexível e robusta para agendamento e execução de tarefas complexas. Você encontrará detalhes sobre a estrutura do projeto, configurações iniciais e exemplos de DAGs para começar.

## Estrutura do Projeto

```
|-- dags/                       # Diretório para armazenar os DAGs do Airflow
|   |-- exemplo_dag.py          # Exemplo de DAG para ilustração
|-- plugins/                    # Diretório para armazenar os plugins personalizados
|   |-- meu_plugin.py           # Exemplo de plugin personalizado
|-- config/                     # Diretório para configurações do Airflow
|   |-- airflow.cfg             # Configurações principais do Airflow
|-- README.md                   # Este arquivo
|-- .gitignore                  # Arquivo para especificar os arquivos a serem ignorados pelo Git
```

## Pré-Requisitos

- [Python](https://www.python.org/) (versão recomendada: >= 3.9 )
- [Apache Airflow](https://airflow.apache.org/) (versão recomendada: >= 2.5.1 )

## Configuração

1. Clone este repositório:

```bash
git clone https://github.com/gfechio/ukboxing-airflow.git
cd ukboxing-airflow
```

1. ```bash
curl -LfO 'https://airflow.apache.org/docs/apache-airflow/2.7.1/docker-compose.yaml'
```

2. ```bash
mkdir -p ./dags ./logs ./plugins ./config
echo -e "AIRFLOW_UID=$(id -u)" > .env
```

3. ```bash
docker compose up airflow-init
```

4. ```bash
docker compose up
```

5. Acesse o Airflow através do navegador usando `http://localhost:8080`.

## Exemplos de Uso

- Consulte o diretório `dags/` para exemplos de DAGs prontos para uso e personalização.

## Contribuição

Sinta-se à vontade para contribuir com melhorias, correções de bugs ou novas funcionalidades! Para saber mais sobre como contribuir, consulte nossa [Política de Contribuição](CONTRIBUTING.md).

## Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).
