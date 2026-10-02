# Zoho Cliq Extension

A custom **Zoho Cliq extension** designed to bring useful functionality and automation directly into team conversations.

This project was developed using the **Zoho Cliq Developer Platform** and integrates custom functionality into the Cliq workspace through an installable extension.

---

## Overview

This project demonstrates how a custom application can be integrated with **Zoho Cliq** to provide functionality directly inside a team's communication environment.

Instead of switching between multiple applications, users can interact with the extension from within Zoho Cliq.

The extension can be installed directly using the following link:

### Install the Extension

[Install Zoho Cliq Extension](https://cliq.zoho.com/installapp.do?id=8262)

> You may need to sign in to your Zoho account before installing the extension.

---

## Why This Project?

Modern teams often use multiple applications for communication, automation, and productivity.

This project explores how those workflows can be brought directly into **Zoho Cliq**, allowing users to interact with custom functionality without leaving their communication platform.

### Key Goals

* Integrate custom functionality with Zoho Cliq
* Automate repetitive workflows
* Provide a simple chat-based interaction experience
* Work with APIs and external services
* Explore Zoho Cliq's extension development platform
* Build practical automation inside a workplace communication tool

---

## Architecture

```text
                    +---------------------+
                    |        User         |
                    |                     |
                    |    Zoho Cliq Chat   |
                    +----------+----------+
                               |
                               v
                    +---------------------+
                    |     Zoho Cliq       |
                    |     Extension       |
                    +----------+----------+
                               |
                +--------------+--------------+
                |              |              |
                v              v              v
           Commands          Bots          Actions
                |              |              |
                +--------------+--------------+
                               |
                               v
                    +---------------------+
                    |    Custom Logic /   |
                    |   API Integration   |
                    +----------+----------+
                               |
                               v
                    +---------------------+
                    |  External Services  |
                    |    / APIs / Data    |
                    +---------------------+
```

---

## Technologies Used

* **Zoho Cliq**
* **Zoho Cliq Developer Platform**
* **Deluge**
* **REST APIs**
* **OAuth 2.0**
* **JSON**
* **Webhooks / API Integrations**
* **Git & GitHub**

---

## Installation

### Option 1 — Install Directly

Use the extension installation link:

[Install Extension](https://cliq.zoho.com/installapp.do?id=8262)

### Option 2 — From Zoho Cliq

1. Open **Zoho Cliq**
2. Open the **Marketplace / Extensions** section
3. Locate the extension
4. Select **Install**
5. Grant the required permissions
6. Start using the extension inside Cliq

Zoho Cliq supports extensions that can add functionality such as bots, commands, and message actions to the platform.

---

## Authentication

If the extension communicates with protected Zoho or third-party APIs, authentication can be handled using **OAuth 2.0**.

OAuth allows applications to obtain authorized access tokens after the user grants permission.

### Example Flow

```text
User
 |
 | Authorize
 v
Zoho Authorization
 |
 | Access Token
 v
Extension
 |
 | API Request
 v
External Service
```

**Important:** Never commit API keys, client secrets, access tokens, or other credentials to GitHub.

Use environment variables or secure configuration instead.

---

## Project Structure

```text
zoho-cliq-extension/
|
├── README.md
|
├── functions/
│   ├── ...
│   └── ...
|
├── bots/
│   └── ...
|
├── commands/
│   └── ...
|
├── actions/
│   └── ...
|
├── integrations/
│   └── ...
|
└── docs/
    └── ...
```

---

## How It Works

The general workflow is:

```text
User interacts with extension
            |
            v
      Zoho Cliq receives request
            |
            v
       Extension processes it
            |
            v
     Custom logic is executed
            |
            v
     API / service is contacted
            |
            v
       Result is processed
            |
            v
      Response shown in Cliq
```

This approach makes it possible to build conversational and workflow-driven applications directly inside a team communication platform.

---

## Features

Depending on the enabled components, the extension can provide functionality such as:

* Chat-based interaction
* Custom bot functionality
* Custom commands
* API integrations
* OAuth-based authentication
* Data retrieval
* Automated workflows
* Integration with external services
* Organization-level productivity features

---

## Testing

Before publishing changes, test the extension for:

### Functional Testing

* Commands execute correctly
* Bot responses are correct
* API requests return expected data
* Error responses are handled properly
* Authentication works correctly

### Edge Cases

* Invalid input
* Missing parameters
* Expired authentication
* API failures
* Network failures
* Empty responses

---

## Security

Please make sure that sensitive information is **never committed to the repository**.

Do not upload:

```text
API Keys
Client Secrets
OAuth Tokens
Passwords
Private Credentials
Environment Variables
```

Use:

```text
.env
Environment Variables
Zoho Secure Properties
```

where appropriate.

---

## Future Improvements

Possible future enhancements include:

* Add more Cliq commands
* Improve error handling
* Add richer interactive cards
* Add additional API integrations
* Improve authentication flow
* Add automated testing
* Improve documentation
* Add analytics and usage tracking
* Add more automation workflows

---

## Demo

Add screenshots or a short GIF here showing the extension running inside Zoho Cliq.

Example:

```text
docs/
├── demo.png
├── command-demo.gif
└── architecture.png
```

You can then display them in this README:

```markdown
![Extension Demo](docs/demo.png)
```

---

## What I Learned

Through this project, I explored:

* Building extensions for Zoho Cliq
* Working with the Cliq Developer Platform
* API integration
* OAuth 2.0 authentication
* JSON-based request/response handling
* Automation using Deluge
* Designing chat-based workflows
* Integrating external services into communication platforms
* Building and deploying a practical workplace application

---

## Useful Links

* **Install the Extension:**
  [Zoho Cliq Extension](https://cliq.zoho.com/installapp.do?id=8262)

* **Zoho Cliq:**
  https://www.zoho.com/cliq/

* **Zoho Cliq Developer Documentation:**
  https://www.zoho.com/cliq/help/

* **Zoho Cliq API Documentation:**
  https://www.zoho.com/cliq/help/restapi/

---

## Author

**Karthikayini Srinivasan**

Computer Science Engineering Student

Interested in:

* Backend Development
* API Development
* Distributed Systems
* Software Engineering
* Automation
* Machine Learning

---

## Support

If you find this project interesting, consider giving the repository a star on GitHub.

---

## License

This project is intended for educational and demonstration purposes.

Add an appropriate open-source license if you plan to distribute the source code publicly.
