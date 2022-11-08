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
