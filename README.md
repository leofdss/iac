# iac

## Enviroment

### Install Terraform

```bash
wget -O- https://apt.releases.hashicorp.com/gpg | gpg --dearmor | sudo tee /usr/share/keyrings/hashicorp-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
sudo apt update && sudo apt install terraform
```

### Install Python3

```bash
sudo apt install python3
```

### Install Ansible

```bash
sudo apt update
sudo apt install software-properties-common
sudo add-apt-repository --yes --update ppa:ansible/ansible
sudo apt-get install ansible
```

### Install AWS CLI

```bash
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
```

### AWS configure

```bash
aws configure
```

## Build Infrastructure

```bash
terraform init
```

```bash
terraform fmt
```

```bash
terraform validate
```

```bash
terraform apply
```

```bash
terraform show
```

## Change Infrastructure

```bash
terraform init
```

```bash
terraform apply
```

## Destroy Infrastructure

```bash
terraform destroy
```
