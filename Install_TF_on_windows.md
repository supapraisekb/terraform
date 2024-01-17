# Installing Terraform on Windows

This installation is not like the usual installation of .exe and other installation packages. there are several steps to go through

1. In youe web browser search "download latest terraform for windows"

2. From the results page, choose **install Terraform**

![choosse install terraform](/AWS/terraform/assests/screenshots/terraform-installation_&_config/02_terraform_installation_search.JPG)

3. Scroll down to **binary download** and choose **AMD64**
![choose AMD64](/AWS/terraform/assests/screenshots/terraform-installation_&_config/03-choose_binary_download.JPG)


4. Go to **C drive, Windows, system32** and create a folder named **terraform**


5. Go to downloads and **extract the downloaded TF zip file** to the newly created folder in step 4.

6. **verify that the extraction is successful** 
- go to you **C drive**

- click **windows folder**
- click **system32**
- click **terraform folder** 
- ensure that the **terraform application** is present
- right click the applicaion, click on properties, **copy the location** for future use 

![Copy the location](/AWS/terraform/assests/screenshots/terraform-installation_&_config/06-terraform_properties.JPG)

# Configuring Terraform for windows

7. Search **edit** in windows and choose **edit the system environment variables** from the results

![Choose edit the system environment variable ](/AWS/terraform/assests/screenshots/terraform-installation_&_config/07-Search_edit_in_windows.jpg)

8. Selelct **Environment Variables** from the **advanced** tab
![choose environment variables](/AWS/terraform/assests/screenshots/terraform-installation_&_config/8-select_environment_variables.JPG)

9. Select **path at User variables part**  also  Select **path at the systems variable part** 
![Select path](/AWS/terraform/assests/screenshots/terraform-installation_&_config/09-Select_paths_and_click_edit.JPG)

10. click the **edit** button

11. click **new** and  ``recall tthe location copied in step 6``, 

![click new](/AWS/terraform/assests/screenshots/terraform-installation_&_config/11-click_new.JPG)

12. **Paste this location**in the textbox  

![Paste the location to the terraform](/AWS/terraform/assests/screenshots/terraform-installation_&_config/11-click_new.JPG)

13. Click Ok to all open windows


 

