# Kali Linux dev container for GitHub Codespaces
FROM mcr.microsoft.com/devcontainers/base:kalify

USER root

# Core Kali tooling (add/remove packages as you like)
RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        curl \
        git \
        wget \
        vim \
        python3 \
        python3-pip \
        nikto \
        nmap \
        whois \
        netcat-traditional \
    && rm -rf /var/lib/apt/lists/*

USER vscode
