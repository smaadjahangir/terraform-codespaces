FROM mcr.microsoft.com/vscode/devcontainers/base:buster

RUN apt-get update && \
        apt-get install -y python

RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip" && \
        unzip awscliv2.zip && \
        sudo ./aws/install

RUN wget "https://releases.hashicorp.com/terraform/1.1.9/terraform_1.1.9_linux_amd64.zip" && \
        unzip terraform_1.1.9_linux_amd64.zip && \
        mv terraform /usr/local/bin/
