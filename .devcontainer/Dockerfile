FROM mcr.microsoft.com/devcontainers/base:resolute

RUN sudo apt update && sudo apt -y upgrade
RUN sudo apt install -y python3-pip python3-full
RUN curl -O https://raw.githubusercontent.com/Cambridge-ICCS/differentiable-programming-summer-school-2026/refs/heads/main/requirements.txt
RUN pip install -r requirements.txt
