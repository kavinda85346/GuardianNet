# GuardianNet

GuardianNet is a machine learning–based cybersecurity project focused on detecting and mitigating a range of digital threats. It combines anomaly detection, attack classification, and content analysis to help identify malicious activity before it causes damage.

## Table of Contents

- [Features](#features)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Project Status](#project-status)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Anomaly Detection for Cyber Threats** — Identifies unusual patterns in network/system behavior that may indicate a security incident.
- **Cyber Attack Detection** — Detects known and emerging attack patterns across monitored systems.
- **Ransomware Detection and Blocking** — Flags ransomware-like behavior and takes preventive action.
- **Email Security Issue Identification** — Scans emails for security risks and suspicious content.
- **Phishing Detection** — Classifies phishing attempts in emails, links, and messages.

## Prerequisites

- Python 3.10 or later
- Git
- Windows, macOS, or Linux (commands below are shown for Windows `cmd`; macOS/Linux equivalents are noted where they differ)

## Getting Started

Follow the steps below to set up the project environment and run GuardianNet locally.

### 1. Install Python

Download the latest stable Python version from the official Python website:

[https://www.python.org/](https://www.python.org/)

> During installation on Windows, check **"Add python.exe to PATH"** to skip the manual path configuration in Step 2.

### 2. Verify the Python Installation

Check whether the environment variables are correctly configured by running the following command in `cmd`:

```
python -V
```

If the command outputs `Python 3.X.X`, proceed to [Step 3](#3-clone-the-github-repository). If it does not, proceed to Step 2.1.

#### 2.1 Set the Python Path

Run the following command in `cmd` to configure the environment, replacing the paths with your actual Python installation directory. Alternatively, navigate to **System Properties → Advanced → Environment Variables** and add the paths there.

```
setx PATH "%PATH%;C:\Users\John\AppData\Local\Programs\Python\Python313;C:\Users\John\AppData\Local\Programs\Python\Python313\Scripts"
```

> Replace `John` and `Python313` with your username and installed Python version.

Then proceed to Step 2.2.

#### 2.2 Re-verify the Python Path

Open a **new** `cmd` window (so the updated PATH takes effect) and run:

```
python -V
```

If the command now outputs `Python 3.X.X`, proceed to Step 3. If it still doesn't, double-check the path entered in Step 2.1 before continuing.

### 3. Clone the GitHub Repository

Choose a location on your drive, create a directory, and navigate into it. Then clone the repository.

```
mkdir workspace & cd workspace
git clone https://github.com/kavinda85346/GuardianNet.git
cd GuardianNet
```

### 4. Create a Virtual Environment

```
python -m venv .playenv
```

### 5. Activate the Virtual Environment

```
.playenv\Scripts\activate
```

> On macOS/Linux, use `source .playenv/bin/activate` instead.

Once activated, you should see `(.playenv)` prefixed to your terminal prompt.

### 6. Upgrade pip

```
python -m pip install --upgrade pip
```

### 7. Install Required Libraries

Install the necessary libraries into the activated environment only.

```
python -m pip install numpy pandas
```

### 8. Verify Installed Packages

```
python -m pip list
```

### 9. Deactivate the Environment

Once you're done working, deactivate the environment.

```
deactivate
```

> Reactivate the created enviornment, use `.playenv\Scripts\activate`.

## Project Status

This is a personal pet project under active development. Features and setup instructions will be updated as the project evolves.

## Contributing

This is currently a personal project and not yet set up for external contributions. This section will be updated if that changes.

## License

This project is currently unlicensed / for personal use.
