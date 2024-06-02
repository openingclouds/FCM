# FCM Script

Welcome to the FCM Script repository! This repository contains a powerful PowerShell script designed to help you port your phone system out of Microsoft Teams Phone to another provider using various APIs.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The FCM Script is a tool developed to facilitate the transition of your phone system from Microsoft Teams Phone to a different telecommunication provider. By leveraging multiple APIs, this script automates the porting process, ensuring a smooth and efficient migration.

## Features

- **Automated Porting**: Streamlines the process of transferring phone numbers from Teams Phone to another provider.
- **API Integration**: Supports integration with various telecommunication provider APIs for seamless porting.
- **Error Handling**: Comprehensive error handling to manage and log issues during the porting process.
- **Customizable**: Easy to configure and extend according to your specific requirements.

## Requirements

- PowerShell 5.1 or later
- Required PowerShell modules (listed in `requirements.psd1`)
- API credentials for Microsoft Teams Phone and your target telecommunication provider

## Installation

1. Clone this repository to your local machine:
    ```bash
    git clone https://github.com/yourusername/fcm-script.git
    cd fcm-script
    ```

2. Install the required PowerShell modules:
    ```powershell
    Import-Module .\requirements.psd1
    ```

## Usage

1. Ensure you have configured the script with the necessary API credentials (see [Configuration](#configuration)).

2. Run the script:
    ```powershell
    .\fcm_script.ps1
    ```

3. Follow the on-screen instructions to complete the porting process.

## Configuration

Before running the script, you need to configure it with the necessary API credentials and settings. Create a configuration file (`config.json`) in the root directory of the repository with the following structure:

```json
{
    "teams_api": {
        "client_id": "your_teams_client_id",
        "client_secret": "your_teams_client_secret",
        "tenant_id": "your_teams_tenant_id"
    },
    "provider_api": {
        "api_key": "your_provider_api_key",
        "api_secret": "your_provider_api_secret"
    }
}
```

Replace the placeholder values with your actual API credentials.

## Contributing

We welcome contributions from the community! If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature-name`).
3. Commit your changes (`git commit -am 'Add some feature'`).
4. Push to the branch (`git push origin feature/your-feature-name`).
5. Create a new Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to open an issue if you have any questions or run into any problems!
