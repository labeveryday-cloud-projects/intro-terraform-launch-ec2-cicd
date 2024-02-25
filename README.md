# intro-terraform-launch-ec2-cicd
This the pipeline that will be used to lint, test and deploy our infrastructure. 

Prerequisites 

An active [AWS account](https://docs.aws.amazon.com/accounts/latest/reference/welcome-first-time-user.html)

AWS Command Line Interface (AWS CLI), [installed](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) and [configured](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html)

[Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git), installed and configured on your local machine

[Terraform](https://developer.hashicorp.com/terraform/tutorials/aws-get-started?utm_source=WEBSITE&utm_medium=WEB_IO&utm_offer=ARTICLE_PAGE&utm_content=DOCS), installed and configured on your local machine



### Command Terraform Commands

The main Terraform commands:

`terraform init` — initializes a terraform working directory and installs backends, modules, and plugins.

`terraform plan` — Takes your configuration and creates an execution plan. You then can verify what changes will be made before they are applied.

`terraform apply` — Create or update the infrastructure

`terraform destroy` — Destroy previously created infrastructure

**Other Terraform commands to know:**

`terraform version` — shows the current version of Terraform

`terraform validate` — Checks to ensure code is syntactically and internally consistent.

`terraform fmt` — Reformats your configuration files in the standard format and style. (Cleans up your code)

`terraform output` — Shows output values from the root module

`terraform console` — Enter into the Terraform console

`terraform import` — Used to import existing resources into the terraform state

`terraform state list` — To list deployed resources

`terraform show` — View all of the resources in your infrastructure’s state

`terraform taint` — Used to mark a resource as not fully functional and will be replaced with the next terraform apply

`terraform workspace` — Manages Terraform workspaces

#### Resources

[Terraform AWS Provider Documentation](https://registry.terraform.io/providers/hashicorp/aws/latest/docs)

[THE AWS INTEGRATION & AUTOMATION TEAM'S BEST PRACTICES FOR TERRAFORM](https://aws-ia.github.io/standards-terraform/)

[Create a CI/CD pipeline to validate Terraform configurations by using AWS CodePipeline](https://docs.aws.amazon.com/prescriptive-guidance/latest/patterns/create-a-ci-cd-pipeline-to-validate-terraform-configurations-by-using-aws-codepipeline.html)
