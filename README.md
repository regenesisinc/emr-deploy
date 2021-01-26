# emr-deploy
AWS Resource Deployment Artifacts :: Elastic Map Reduce (EMR) 

#  Setup CDK Development

## Installing CDK and components

###  Prepare to use CDK with python env

#### Install Prerequisites:

```
sudo python -m ensurepip --upgrade
sudo python -m pip install --upgrade pip
sudo python -m pip install --upgrade virtualenv
 ```

#### Initialize Project Dir:

```
mkdir my-project
cd my-project
cdk init app --language python
```

#### Setup Your Environment

Initialize Virtual Python Environment
```
python3 -m venv .venv
```

Activate your environment
```
source .venv/bin/activate
```

Install the AWS Construct Library modules into your environment
```
python -m pip install aws-cdk.aws-billing-alarm
python -m pip install aws-cdk.aws-cloudformation
python -m pip install aws-cdk.aws-dax
python -m pip install aws-cdk.aws-ec2
python -m pip install aws-cdk.aws-efs
python -m pip install aws-cdk.aws-elasticache
python -m pip install aws-cdk.aws-emr
python -m pip install aws-cdk.aws-emrcontainers
python -m pip install aws-cdk.aws-events
python -m pip install aws-cdk.aws-guardduty
python -m pip install aws-cdk.aws-iam
python -m pip install aws-cdk.aws-lambda
python -m pip install aws-cdk.aws-logs
python -m pip install aws-cdk.aws-networkfirewall
python -m pip install aws-cdk.aws-networkmanager
python -m pip install aws-cdk.aws-s3
python -m pip install aws-cdk.aws-secretsmanager
```

Create an Initial Requirements File
```
python -m pip freeze >requirements.txt
```

Edit Requirements and drop the lines below:
```
# Editable Git install with no remote (test1==0.0.1)
-e /home/mcorcoran/projects/aws/cdk/test1/test1
```
Once you have your project requirements file, you can reloaed it like this:
```
python -m pip install -r requirements.txt
```

### References:
   - https://docs.aws.amazon.com/cdk/latest/guide/work-with-cdk-python.html
   - https://pypi.org/search/?q=aws-cdk
   - https://aws.amazon.com/emr/?whats-new-cards.sort-by=item.additionalFields.postDateTime&whats-new-cards.sort-order=desc
