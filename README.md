# DL
abc
#Hii I am student from TE/IT



SAST to SonarQube Git Lab:
node
{
        stage('clonning from GIT'){
    git branch: 'main', credentialsId: 'GIT_REPO', url: 'https://github.com/Subhashish-Mahapatra/jenkins-sonarqube.git'
        }
}

Image has been added: (add trigger, then after that in code add this)

exports.handler = function(event, context, callback) {
console.log("Incoming Event:" , event);
const bucket = event.Records[0].s3.bucket.name;
const filename = decodeURIComponent(event.Records[0].s3.object.key.replace(/\+/g, ' '));
const message = `File is uploaded in — ${bucket} -> ${filename}`;
console.log(message);
callback(null, message);
};

# basic lambda function:
import json
def lambda_handler(event, context):
 first_number=100
 second_number=200
 sum = first_number + second_number
 return sum

2)
def lambda_handler(event, context):
 if event["name"]=="subhashish":
 return "apsit"
 
 
 #terraform
Install curl on linux using sudo apt install curl
• Execute curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
• sudo apt install unzip
• sudo unzip awscliv2.zip
• sudo ./aws/install
• aws –version
• Create a new access key if you don't have one. Make sure you download the keys in your 
local machine. Login to AWS console, click on username and go to My security credentials
• Continue on security credentials, click on access keys. First setup your access keys, secret 
keys and region code locally.
• In terminal of your ubuntu run “aws configure”
• Create one Directory for Terraform project in which all files of terraform we can save 
onworks@onworks-Standard-PC-i440FX-PIIX-1996:~$ cd ~ 
onworks@onworks-Standard-PC-i440FX-PIIX-1996:~$ mkdir project-terraform 
onworks@onworks-Standard-PC-i440FX-PIIX-1996:~$ cd project-terraform
• Run sudo nano variables.tf

variable "aws_region" {
  description = "The AWS region to create things in. "
  default     = "ap-south-1"
}

variable "key_name" {
  description = " SSH keys to connect to ec2 instance"
  default     = "terraform"
}

variable "instance_type" {
  description = "instance type for ec2"
  default     = "t2.micro"
}

• Go to EC2 and create key pair. Give name to key pair file as terraform and click pem
• Use your Region and Key name in variable.tf as shown and provide instance type which you 
want to create
• After create main.tf file. Sudo nano main.tf

• Then in ec2 console go to ami catalog and select ami linux2 and copy ami id and change in 
main.tf in provider change region 
• Run terraform init
• Run terraform plan
• Run terraform apply
• Do you want to perform these actions?
Terraform will perform the actions described above.
Only 'yes' will be accepted to approve.
Enter a value: yes
• Now login to EC2 console, to see the new instances up and running, you can see 
Jenkins_instance is up and running which we deploy from terraform
• Terraform destroy you can also destroy or delete your instance by using terraform 
destroy command
• Now you can see instance which you created by using terraform is deleted 
successfully from aws console also you can check it will removed successfull
