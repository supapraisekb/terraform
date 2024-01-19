# Using Terraform to create an EC2 instance in AWS

This tutorial assumes that you already have an **AWS Root account** and on it you have created an **IAM user account**. You must have also created your **two factor authentication** and **Access keys**

1. To verify that terraform is installed and working:

open your teminal on vscode and type ```terraform -v```

Note: You can also use powershell on windows to run this command

2. Configure AWS on your Terminal

    a.  On the terminal, type ```aws configure```

    b. Enter your **AWS Access Key ID**

    c. Enter your **AWS Secret Access Key**

    d. Enter a Default region name e.g us-east-1

    e. Press **Enter**

3. Verify your configuration using this command 

``` aws sts get-caller-identity```    


4. Create a directory, to hold all your terraform files. Choose an appropriate name e.g **terraform_file**

5. Open the directory in your VSCode. 
6. Create a new file in that directory with the name main.tf extension


7. copy the template code below from which you will edit other parameters for you EC2 instance creation

```
provider "aws" {
  region = "region"
}
resource "aws_instance" "Demo" {
  ami           = "instance_id"
  instance_type = "instance_type"
  key_name = "key_name"
  tags = {
    Name = "instance_name"
  }
}

```

8. Paste this code in the main.tf file

9. Edit the file thus:

- Rwplace **region** with your desired region. E.g ```us-east-1```
 (you can enter your own prefered region)
- Replace **instance_ID** with the ami-ID of the  of the required AMI you want to create E.g: 
```
ami-035d8ae8de3734e5a
```
-  Replace **Instance type** with the desired type E.g:

```
t2.micro
```

-  Repalce **Key_name** with the name of your **key pair**.  This can be obtained from the console by 
    
    - Search for and click on **key pair** in the services menu.
    - under **name** copy the key name there.
- Replace **Instance name** with the name name you want to give your instance E.g:

```
admin-server-1
```

10. save the file

11. open your terminal and type ```terraform init```. When you the message **terraform has been successfully initialized* then run the next step

12. Type ```terraform validate```

13. Type ```terraform apply```
14. Type ``yes``
15. When you see apply completed, go to the console and verify if the instance hasbeen completed or not

16. TO avoid extra unwanted costs, it is good todelete your unused instances. To do this, use the ``terraform destroy`` command

17. It will askforconfirmation, type **yes** 

18. Lab Done!!

