# Learning-Airflow

## Setup:

* Criando o ambiente virtual:

```bash
    python3 -m venv .env
```

* Ativando o ambiente virtual:

```bash
    source .env/bin/activate
```
### Airflow:

* Cria-se  uma variável de ambiente que aponta para a pasta onde o Airflow será instalado:

```bash
    export AIRFLOW_HOME=$(pwd)/airflow
```

* Instalando o Airflow:

```bash
    pip install apache-airflow==1.10.14 --constraint "https://raw.githubusercontent.com/apache/airflow/constraints-1.10.14/constraints-3.7.txt"
```

* Para iniciar o banco de dados do Airflow:

```bash
    airflow initdb
```

* Para iniciar o Webserver (interface da ferramenta):
* 
```bash
   airflow webserver
```

O airflow será iniciado na porta 8080, por default.

* Para iniciar o serviço de scheduler:

* 
```bash
   airflow scheduler
```
### API do Twitter:

Documentação da API do Twitter: https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-recent 
