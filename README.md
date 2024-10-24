# Project Setup Guide

This guide outlines the steps to set up the development environment for a project that involves Python and C# coding in Jupyter Notebook.

## Prerequisites

Ensure that you have the following installed on your Ubuntu system:

- Python 3
- .NET SDK (C#)
- Jupyter Notebook

## Steps to Install

### 1. Install pip

Pip is the package installer for Python. You can install it by running:

```bash
sudo apt update
sudo apt install python3-pip
```

## Install .NET SDK for C#
```bash
sudo apt update
sudo apt install -y dotnet-sdk-8.0
```

## Create a Virtual Environment and install jupyter notebook
```bash
python3 -m venv myenv
pip install jupyter
dotnet tool install --global Microsoft.dotnet-interactive
dotnet interactive jupyter install
pip install -r requirements.txt
```

## Setup virtual env -> Contains dotnet path and activates myenv
```bash
source req_path.sh
```

## Check jupyter kernels
```bash
jupyter kernelspec list
```

## Run Jupyter notebook
```bash
jupyter notebook
```