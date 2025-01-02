# Microsoft Active Directory Scripts

Welcome to the **Microsoft Active Directory Scripts** repository! This collection of PowerShell scripts is designed to streamline and enhance the management of Microsoft Active Directory environments.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Requirements](#requirements)
- [Getting Started](#getting-started)
- [Available Scripts](#available-scripts)
- [Examples](#examples)
- [Customization](#customization)
- [Contributing](#contributing)
- [License](#license)

## Overview

This repository provides a set of PowerShell scripts aimed at simplifying common Active Directory tasks, automating repetitive processes, and improving efficiency for IT administrators.

## Features

- Automated user and group management
- Simplified Active Directory reporting
- Tools for managing GPOs, OU structures, and permissions
- Scripts for auditing and security management
- Modular design for ease of customization

## Requirements

- **PowerShell**: Version 5.1 or higher (Windows PowerShell or PowerShell Core)
- **Active Directory PowerShell Module**
- Administrator privileges for certain scripts

## Getting Started

1. Clone this repository:

   ```bash
   git clone https://github.com/Idanada/MS-Active-Directory.git
   ```

2. Navigate to the cloned directory:

   ```bash
   cd MS-Active-Directory
   ```

3. Review the prerequisites for each script in the `scripts/` folder.

4. Run the desired script using PowerShell:

   ```bash
   .\ScriptName.ps1
   ```

## Available Scripts

### Domain Maintenance

- **`DC - Win Domain Maintenance.ps1`**:
  - **Purpose**: Performs routine maintenance on a Windows Domain Controller. This includes health checks, log cleanup, and event log analysis.
  - **Key Features**:
    - Identifies replication issues.
    - Validates Active Directory services.
    - Cleans up temporary files.
  - **Usage Example**:
    ```powershell
    .\"DC - Win Domain Maintenance.ps1" -HealthCheckOnly
    ```

### DNS Management

- **`FetchDNSRecords.ps1`**:
  - **Purpose**: Retrieves DNS records for a specific domain or zone, helping administrators troubleshoot and manage DNS configurations.
  - **Key Features**:
    - Supports A, AAAA, CNAME, MX, and TXT record types.
    - Outputs results in a user-friendly format.
  - **Usage Example**:
    ```powershell
    .\"FetchDNSRecords.ps1" -ZoneName "example.com"
    ```

## Examples

### Running `DC - Win Domain Maintenance.ps1`

This script helps perform various maintenance tasks on your domain controller. For example, to run the script and check domain health:

```powershell
."DC - Win Domain Maintenance.ps1" -HealthCheckOnly
```

### Running `FetchDNSRecords.ps1`

Use this script to fetch DNS records for a specific zone. For example:

```powershell
."FetchDNSRecords.ps1" -ZoneName "example.com"
```

This will output all DNS records for the zone `example.com`.

For detailed usage of parameters, refer to the inline comments within each script.

## Customization

Each script is modular and customizable. Modify the parameters and logic in the scripts to suit your organization's specific needs. Scripts include detailed comments and instructions for easy editing.

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.

2. Create a new branch:

   ```bash
   git checkout -b feature/your-feature-name
   ```

3. Commit your changes and push the branch:

   ```bash
   git commit -m "Add your message here"
   git push origin feature/your-feature-name
   ```

4. Open a Pull Request.

## License

This repository is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute these scripts.

---

Got feedback or questions? [Open an Issue](https://github.com/Idanada/MS-Active-Directory/issues).

