# DBT Setup en voorbereiding op presentatie

### Notities:
  - Setup en installatie van DBT is redelijk omslachtig. Geen sample of test omgeving om mee te testen. Voordat we aan de slag konden moesten we eerst veel
  installeren en omgeving klaar zetten.

## TODO: 
  - Hoe werkt testing met DBT?
  - Vergelijk snelheden en tijden met DBT tussen verschillende cloud platformen
  - Vergelijk snelheden tussen DBT en handmatige queries
  - Voorbeeld maken hoe DBT can generate DAG's

# Alec:
  - Opzetten in Databricks
  - Tutorial afmaken

# Bram:
  - Opzetten in Bigquery
  - Tutorial afmaken

### Steps for setting up DBT core with Azure Databricks:
- Run pip install dbt-databricks
- Create Databricks workspace in Azure with own resource group
- Fill in deploy Azure Databricks workspace with Secure Cluster Connectivity as yes
- If necessary, increase the amount of regional vCPUs to run the workspace by submitting a quota increase
- In Databricks, run a SQL warehouse. In the warehouse settings you will find the host name and http path
- Generate a personal token in the Databricks user settings
- Import the required data in Databricks in a SQL warehouse
- In the profiles.yml, set the adapter type, host, token and http_path
- Check connection to Azure Databricks by running dbt debug

Maybe use this dataset? https://www.kaggle.com/datasets/rajugc/imdb-movies-dataset-based-on-genre
