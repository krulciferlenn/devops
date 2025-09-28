FROM python:3.11-slim

# Install Ansible + Terraform
RUN apt-get update && \
    apt-get install -y curl unzip && \
    pip install ansible && \
    curl -fsSL https://releases.hashicorp.com/terraform/1.9.8/terraform_1.9.8_linux_amd64.zip -o terraform.zip && \
    unzip terraform.zip && mv terraform /usr/local/bin/ && \
    rm terraform.zip && \
    rm -rf /var/lib/apt/lists/*
