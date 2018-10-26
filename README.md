## Deployment manager script for the below shell script
### https://github.com/spinnaker/spinnaker/blob/master/codelabs/gke-source-to-prod/install/setup.sh

`service-account` - code to create service account and assign roles <br />
`pubsub` - code to create pubsub topic and subscription <br />
`basic-gke`- code to create GKE cluster <br />
`gsutil-cp` - code to upload files to GCS buckets and images to GCR.

### NOTE <br />
params are in .yaml file of the respective folders and description is in .schema file of the respective folder.

## Steps to setup

go to the respective directories
### cd <dir_name>

## Create Deployment
syntax: gcloud deployment-manager deployments create <deployment_name> --config <config_file> <br />
example: gcloud deployment-manager deployments create basic-gke --config basic-gke.yaml <br />

## List Deployment
syntax: gcloud deployment-manager deployments list


## Delete Deployment
syntax: gcloud deployment-manager deployments delete <deployment_name> <br />
example: gcloud deployment-manager deployments delete basic-gke <br />
