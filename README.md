<H1>Project Setup</H1>
Prerequisites
Terraform installed on your local machine
Google Cloud SDK installed and configured with your GCP account

Setting up Terraform Environment Variables
export GCP_PROJECT_ID=your_gcp_project_id
export GCP_REGION=your_gcp_region
export GCP_CREDENTIALS_FILE=path/to/your/gcp/credentials.json

Deploying the Infrastructure
#Clone the repository:
git clone https://github.com/your-username/your-repository.git

#Change into the project directory:
cd your-repository

#Initialize the Terraform working directory:
terraform init

#Review the Terraform plan:
terraform plan

#Accessing the Deployed Application
 It will be in the format https://<service-name>-<revision-suffix>-<region-suffix>.a.run.app.

Running the Bash Script
#Change to the root directory of the project:
cd ../

#Make the Bash script executable:
chmod +x get_cloud_run_ip.sh

#Run the script with the desired environment as an argument:
./get_cloud_run_ip.sh dev

Troubleshooting
 Authentication Issues:
 Terraform Errors:
 Bash Script Errors:

Problems Encountered and Solutions
  Authentication Issues: Initially, I encountered authentication-related errors when running the gcloud commands in the Bash script. 
  I resolved this by adding the necessary environment variable configurations and running gcloud auth login to authenticate with Google Cloud.
