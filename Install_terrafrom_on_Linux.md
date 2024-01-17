# Steps to install Terraform on Linux ubuntu 

1. Ensure that your system is up to date and you have installed the gnupg, software-properties-common, and curl packages

2. Type of copy the code below and paste in your terminal

```
sudo apt-get update && sudo apt-get install -y gnupg software-properties-common
```

3. Install the HashiCorp GPG key. using the code below

```
wget -O- https://apt.releases.hashicorp.com/gpg | \
gpg --dearmor | \
sudo tee /usr/share/keyrings/hashicorp-archive-keyring.gpg
```

4. Verify the Key's Fingerprint 

```
gpg --no-default-keyring \
--keyring /usr/share/keyrings/hashicorp-archive-keyring.gpg \
--fingerprint
```

5. Add the official HashiCorp repository to your system. The lsb_release -cs command finds the distribution release codename for your current system, such as buster, groovy, or sid.

```
echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] \
https://apt.releases.hashicorp.com $(lsb_release -cs) main" | \
sudo tee /etc/apt/sources.list.d/hashicorp.list

```

6. Download the package information from HashiCorp.

```
sudo apt update

```

7. Install Terraform from the new repository.

```
sudo apt-get install terraform

```

# Verify the installation

Verify that the installation worked by opening a new terminal session and listing Terraform's available subcommands.

```
terraform -help

```

b. 

```
terraform -help plan

```

# Enable tab completion

If you use either Bash or Zsh, you can enable tab completion for Terraform commands. To enable autocomplete, first ensure that a config file exists for your chosen shell.

- Bash 

```
touch ~/.bashrc
```

- Zsh 

```
touch ~/.zshrc
```

Then install the autocomplete package

```
terraform -install-autocomplete

```

