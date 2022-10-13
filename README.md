# Introduction 
TODO: Intro

# Setup Service Connection
To use this Pipeline create a Service Connection to Authenticate to your Dynamics Environment.

## Create App Registration
Create a new App Registration for your DevOps Pipeline
![new app registration](assets/appreg_new.png)
Create a Secret for the App
You will need this Secret in a future step.
![add secret](assets/appreg_secret.png)
Notice the App informations for the App you will need the Tenant ID and the App ID.
![app registrations overview](assets/appreg_overview.png)

## Authorize App in Dynamics
Authorize the App in the Power Apps Admin Center
![env overview](assets/env_detail.png)
Notice the Environment Link, you will need it in a future Step.

Add a New Application User to the Environment
![env overview](assets/new_user.png)

Add your created App - search if necessary with the App ID
![add app](assets/add_app.png)

Give your app the System Administrator Security Role.
![permissions](assets/create_app_user.png)

## Create Service Connection
Configure a new Service Connection in Azure DevOps
Go to the Project Settings and add a new Service Connection
![project settings](assets/servconn_projsett.png)
Select Type Power Platform
![type pp](assets/servconn_pp.png)
Fill in the information from the previous steps
![Service connection new](assets/servconn_new.png)
And Save

# Configure Pipeline

Complete the Variables Part in the Pipeline with your Values.
![azpipe variables](assets/azpipe_var.png)

In your Project go to Pipelines -> Pipelines -> New Pipeline
![azpipe new](assets/azpipe_new.png)

Select Azure Repos (Git)
Choose from existing file and select your Pipeline
![azpipe add existing pipeline](assets/azpipe_addex.png)

RUN it :)



