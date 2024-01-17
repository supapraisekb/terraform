# AWS Command Line Interface (CLI)

This a command line intrface provided by AWS and it provides a unified management tool for managing  AWS resources from your PC's command line

# Steps:

1. Go to your browser and search for ``download AWS CLI for windows``

![Search for aws cli download for windows](/AWS/terraform/assests/screenshots/ASW_CLI_installation/01-search_for%20_aws_cli_download.JPG)

2. click the first link and go to the official site

3. scroll down the page and click on **Windows**

4. under **Install or Update the AWS CLI** section, click on the link 

```
https://awscli.amazonaws.com/AWSCLIV2.msi
```

![click to download the CLI msi Installer](/AWS/terraform/assests/screenshots/ASW_CLI_installation/02-click_to_download.JPG)

# OR

5. open command prompt and run this code:
 ```
 msiexec.exe /i https://awscli.amazonaws.com/AWSCLIV2.msi
 ```

 6. Locate the downloadeded installer in you default download locatoion and double click to run it

 7. Click **Next** , **Accept the license agreement**, Click next then **Install**

 8. After the process in completed, **verify** that your installation is complete

 - Open command prompt on your PC
 - enter the following command
 ```
 aws --version
 ```

9. If you get the output in  the attached image then it is correctly installed:

![Verified AWS CLI installation ](/AWS/terraform/assests/screenshots/ASW_CLI_installation/08-verify_the_installation.JPG)

10. Done! 







