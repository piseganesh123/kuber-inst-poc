# kuber-inst-poc
POC to install kubernetes on Ubuntu servers for demo purpose

Pre-Requisite
1. Ensure compute engine api is enabled before creating infrastructure

Steps:
1. clone repository
2. Update variables (variables.tf file) according to your GCP account
3. run terraform init && terraform apply

Create secret to pull image from gcr

$kubectl create secret docker-registry gcr-key-1 --docker-server=gcr.io --docker-username=_json_key --docker-password="$(cat /home/pgan432_gmail_com/gcr-user-level-epoch.json)" --docker-email=any@valid.email
