
# aws regions check using aws cli

$ aws ec2 describe-regions

$ aws ec2 describe-regions --all-regions

# Get aws region name

$ aws lightsail get-regions --query "regions[?name=='eu-west-1'].displayName" --output text

# refer the below link

[Aws Regions and Azs ](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html)
