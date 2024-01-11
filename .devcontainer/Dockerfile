ARG PYTHON_VERSION=3.6

FROM mcr.microsoft.com/vscode/devcontainers/python:${PYTHON_VERSION}-buster

COPY requirements.txt requirements.txt

RUN pip install --no-cache-dir -r requirements.txt

WORKDIR /app

COPY . .

