# How to set up DBT and BQ 

1. Set up a gcp project/ or take one you allready have

2. Make sure the following services are enabled 
```bas
  Biqquery 
```
2. See if you can run the following commands 

```sql
    select * from `dbt-tutorial.jaffle_shop.customers`;
    select * from `dbt-tutorial.jaffle_shop.orders`;
    select * from `dbt-tutorial.stripe.payment`;
```

3. cp ~/.config/gcloud/application_default_credentials.json .devcontainer/application_default_credentials.json

4. mkdir .dbt 

5. touch .dbt/profiles.yml

6. dbt init 

```
Which database would you like to use?
[1] bigquery

(Don't see the one you want? https://docs.getdbt.com/docs/available-adapters)

Enter a number: 1
[1] oauth
[2] service_account
Desired authentication method option (enter a number): 1
project (GCP project id): johan-kubeflow
dataset (the name of your dbt dataset): dbt_test
threads (1 or more): 1
job_execution_timeout_seconds [300]: 30
[1] US
[2] EU
Desired location option (enter a number): 2
13:51:38  Profile test_3 written to profiles.yml using target's profile_template.yml and your supplied values. Run 'dbt debug' to validate the connection.
13:51:38  
Your new dbt project "test_3" was created!

For more information on how to configure the profiles.yml file,
please consult the dbt documentation here:

  https://docs.getdbt.com/docs/configure-your-profile

One more thing:

Need help? Don't hesitate to reach out to us via GitHub issues or on Slack:

  https://community.getdbt.com/

Happy modeling!
```







### Links 
- https://docs.getdbt.com/docs/quickstarts/dbt-cloud/bigquery

