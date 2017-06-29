# How to run
1. Create key pair in AWS console for SSH, HTTP access to instance <br />
	https://console.aws.amazon.com/ec2/v2/home?region=us-west-2#KeyPairs:
2. Download Terraform <br />
	https://www.terraform.io/downloads.html
3. Set PATH variable for Terraform. Terraform.exe installs in C:\Program Files\terraform_0.9.5_windows_amd64 on Windows <br />
	https://www.java.com/en/download/help/path.xml
4. Open Powershell as an administrator, cd into root the folder of this project, and run <br />
	terraform apply -var 'key_name=YOURKEYNAME'
5. You're done. Check AWS console to see newly-created resources

# Useful commands
show what will be built <br />
terraform plan -var 'key_name=YOURKEYNAME' <br />
destroy infrastructure managed by terraform <br />
terraform destroy -var 'key_name=YOURKEYNAME'