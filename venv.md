# Python virtual environment (venv)

## 建立 Ed25519 類型的 SSH 公私鑰對

### Windows
```sh
ssh-keygen -t ed25519 -C "title"
```

### macOS / Linux
```sh
ssh-keygen -t ed25519 -C "title"
```

## Clone GitHub 儲存庫

### Windows
```sh
git clone path
```
### macOS / Linux
```sh
git clone path
```

## Create a Virtual Environment

### Windows
```sh
python -m venv .venv
```

### macOS / Linux
```sh
python3 -m venv .venv
```

## Activate the Virtual Environment

### Windows

```sh
.\.venv\Scripts\activate
```

### macOS / Linux

```sh
source .venv/bin/activate
```

## Deactivate

```sh
deactivate
```

## Install Packages

```sh
pip install package_name
```

## Uninstall Packages

```sh
pip uninstall package_name
```

## List Installed Packages

```sh
pip list
```

## Freeze Package Versions to a File
### macOS / Linux
```sh
pip freeze > requirements.txt
```

### Windows
```sh
pip freeze | Out-File -Encoding UTF8 requirements.txt
```
## Install Packages from a File

```sh
pip install -r requirements.txt
```

## Check for Outdated Packages

This will display a list of packages that have newer versions available.

```sh
pip list --outdated
```

# Specify Python Version When Creating a Virtual Environment

If you have multiple versions of Python installed, you can specify which one to use when creating the environment:

```sh
python3.9 -m venv .venv
```

# Remove all packages

```
deactivate
rm -rf .venv
```

## Upgrade pip (optional)

### Windows

```sh
python.exe -m pip install --upgrade pip
```

### macOS / Linux

```sh
python3 -m pip install --upgrade pip
```
