# Flow chart

  Regions:         location ex: mumbai                             
                          
  Availability-zones: ap-south-1a, ap-south-1b,ap-south-1c - physical data center isolated from each other


 ![image](https://user-images.githubusercontent.com/42309948/146536929-bb3bffa4-84b2-4d6d-bdef-e3653a790ada.png)




# aws regions check using aws cli

$ aws ec2 describe-regions

$ aws ec2 describe-regions --all-regions

# Get aws region name

$ aws lightsail get-regions --query "regions[?name=='eu-west-1'].displayName" --output text

# refer the below link

[Aws Regions and Azs ](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html)
