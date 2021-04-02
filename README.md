* Clone this repository
* Change directory into this repository `cd scuba-school-terraform`
* Create a DigitalOcean API Key with write privileges. Copy that. In the console run `export TF_VAR_do_token=<YOUR_TOKEN_HERE>`
* Run the command `wget https://releases.hashicorp.com/terraform/0.14.9/terraform_0.14.9_linux_amd64.zip`
* Run the command `apt update && apt install -y zip`
* Run the command `unzip terraform_0.14.9_linux_amd64.zip`
* Modify the `vars.tfvars` file to your liking
    * `nano vars.tfvars` to open. `ctrl + o` to save. `ctrl + x` to close
* Run `terraform plan --var-file vars.tfvars`. Make sure you like what you see
* Run `terraform apply --var-file vars.tfvars`. This will spin up the infrastructure. It'll ask you to confirm, type `yes`
* When done, run `terraform destroy --var-file vars.tfvars`

