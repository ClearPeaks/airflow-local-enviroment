# Airflow local environment

This repository contains a docker-compose to get up and running a local Airflow environment for developing purposes.
Don't use this in production environments.

Start the environment with the `docker-compose up` command.

Be aware that in the Dockerfile, it is not specified the Airflow Docker image, so the latest version will be installed.
It is recommended to specify the same version you have in your production environment.

# Get started

## Creating dags

Add your dags in the dags folder.

## Adding variables

In file secrets/variables.yaml you can add variables to be accessed in your DAGs.

## Adding connections

In file secrets/connections.yaml you can add connections to be accessed in your DAGs.

## User and password

When the environment is ready, a user and password authentication will be prompted.
By default, use these credentials:

- user: airflow
- pass: airflow

## Install dependencies

You can add your custom dependencies in the requirements.txt, and install with the following command:

```bash
pip install -r requirements.txt
```
