Welcome to your new dbt project!

### Using the starter project

Try running the following commands:
- dbt run
- dbt test


### Resources:
- Learn more about dbt [in the docs](https://docs.getdbt.com/docs/introduction)
- Check out [Discourse](https://discourse.getdbt.com/) for commonly asked questions and answers
- Join the [chat](https://community.getdbt.com/) on Slack for live discussions and support
- Find [dbt events](https://events.getdbt.com) near you
- Check out [the blog](https://blog.getdbt.com/) for the latest news on dbt's development and best practices

### Steps for setting up DBT core with Azure Databricks:
- Run pip install dbt-databricks
- Create Databricks workspace in Azure with own resource group
- Fill in deploy Azure Databricks workspace with Secure Cluster Connectivity as yes
- If necessary, increase the amount of regional vCPUs to run the workspace by submitting a quota increase
- In Databricks, create a cluster to run dbt jobs. In the cluster settings you will find the host name and http path
- Generate a personal token in the Databricks user settings
- Import the required data in Databricks in a SQL warehouse
- In the profiles.yml, set the adapter type, host, token and http_path
- Check connection to Azure Databricks by running dbt debug


