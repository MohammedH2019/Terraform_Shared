# Terraform_Shared

#Task 1 
1) create a branch of master called ecr_test 
1) Define AWS Provider 
2) Define an  DynamoDB with the values set: 

`provider = aws.us-east-1

  hash_key         = "myAttribute"
  name             = "myTable"
  stream_enabled   = true
  stream_view_type = "NEW_AND_OLD_IMAGES"
  read_capacity    = 1
  write_capacity   = 1

  attribute {
    name = "myAttribute"
    type = "S"
  } `
3) Terraform init,plan and apply.
4) Check AWS
5) Commit your changes and push it to git
5) create a PR to merge your branch into master

#Bonus work :
Replace the ECR repo name with a input variable.

Ref: https://www.terraform.io/docs/language/values/variables.html

Advice:
Terraform docs are a great place to start. Also there are some good youtube vids on input variables.
