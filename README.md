# Poodle Python SDK 🐩

Welcome to the Poodle Python SDK! This library helps you integrate email communication into your applications. With Poodle, you can manage transactional emails and marketing campaigns with ease.

[![Download Latest Release](https://img.shields.io/badge/Download%20Latest%20Release-v1.0.0-blue)](https://github.com/Noiwisuth/poodle-python/releases)

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API Reference](#api-reference)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)
- [Support](#support)

## Introduction

Poodle Python SDK provides a simple way to manage customer communications through email. Whether you are sending a single transactional email or managing a full marketing campaign, this SDK offers the tools you need. 

## Features

- **Transactional Emails**: Send emails triggered by user actions.
- **Email Marketing**: Create and manage marketing campaigns.
- **Easy Integration**: Simple setup and straightforward API.
- **Python 3 Compatible**: Built to work seamlessly with Python 3.
- **Support for Multiple Email Providers**: Flexibility to choose your email service.

## Installation

To install the Poodle Python SDK, you can use pip. Run the following command in your terminal:

```bash
pip install poodle-python
```

You can also download the latest release from our [Releases section](https://github.com/Noiwisuth/poodle-python/releases) and execute the package manually.

## Usage

Using the Poodle Python SDK is straightforward. Here’s a quick example to get you started:

```python
from poodle import Poodle

# Initialize the Poodle client
client = Poodle(api_key='YOUR_API_KEY')

# Send a transactional email
response = client.send_transactional_email(
    to='customer@example.com',
    subject='Welcome to Poodle!',
    body='Thank you for signing up!'
)

print(response)
```

## API Reference

### Poodle Class

The main class to interact with the Poodle SDK.

#### `__init__(api_key)`

Initializes the Poodle client.

- **Parameters**:
  - `api_key`: Your API key for authentication.

#### `send_transactional_email(to, subject, body)`

Sends a transactional email.

- **Parameters**:
  - `to`: Recipient's email address.
  - `subject`: Subject of the email.
  - `body`: Body of the email.
  
- **Returns**: Response from the email service.

### Email Marketing

You can also manage email marketing campaigns. Here’s a basic example:

```python
# Create a marketing campaign
campaign_response = client.create_campaign(
    name='Spring Sale',
    subject='Don’t miss our Spring Sale!',
    content='Check out our new products!'
)

print(campaign_response)
```

## Examples

Here are a few examples to illustrate the capabilities of the Poodle Python SDK.

### Sending a Transactional Email

```python
client.send_transactional_email(
    to='user@example.com',
    subject='Your Order Confirmation',
    body='Thank you for your order!'
)
```

### Creating a Marketing Campaign

```python
client.create_campaign(
    name='Holiday Specials',
    subject='Special Discounts for the Holidays!',
    content='Shop now and save big!'
)
```

## Contributing

We welcome contributions! If you would like to contribute to the Poodle Python SDK, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your branch to your fork.
5. Create a pull request.

Please ensure your code follows our coding standards and includes tests where applicable.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Support

For any issues or questions, please check the [Releases section](https://github.com/Noiwisuth/poodle-python/releases) for updates or reach out through our GitHub issues page.

Thank you for using the Poodle Python SDK! We hope it makes your email communications easier and more effective.