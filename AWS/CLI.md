##### Get list of the names of EC2 instances

`aws ec2 describe-instances --query 'Reservations[].Instances[].Tags[?Key==`Name`].Value' --output text`

*Prerequisite*: The name of the instances should be present as tag in the EC2 instances

