ARG PYTHON_VERSION=3.6

FROM mcr.microsoft.com/vscode/devcontainers/python:${PYTHON_VERSION}-buster

COPY requirements.txt tmp/requirements.txt

RUN pip install --no-cache-dir -r tmp/requirements.txt

