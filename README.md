# Multi Agent DateTime Agent

A Python-based multi-agent system for handling date and time-related queries and operations using Google APIs.

## Overview

This project implements a multi-agent architecture that leverages Google APIs to provide intelligent date and time handling capabilities. The system is designed to be extensible and can be deployed on your local machine for development and testing.

## Prerequisites

- Python 3.8 or higher
- Google API credentials

## Installation

1. Clone the repository:
```bash
git clone https://github.com/Shivam5104/Mutli_Agent_DateTime_Agent.git
cd Mutli_Agent_DateTime_Agent
```

2. Install required dependencies:
```bash
pip install -r requirements.txt
```

3. Set up your Google API Key (see section below)

## Setting Up Google API Key

### Why do you need a Google API Key?

A Google API Key is required to authenticate and access Google services used by this project. Follow the steps below to obtain and configure your API key.

### Steps to Get a Google API Key

#### 1. Create a Google Cloud Project

- Visit [Google Cloud Console](https://console.cloud.google.com/)
- Sign in with your Google account (create one if you don't have it)
- Click on the project dropdown at the top
- Click "NEW PROJECT"
- Enter a project name (e.g., "DateTime Agent")
- Click "CREATE"
- Wait for the project to be created and select it

#### 2. Enable Required APIs

- In the Cloud Console, go to "APIs & Services" > "Library"
- Search for the APIs you need (e.g., Google Calendar API, Google Sheets API, etc.)
- Click on the API and click "ENABLE"
- Repeat for all required APIs

#### 3. Create API Credentials

- Go to "APIs & Services" > "Credentials"
- Click "CREATE CREDENTIALS"
- Select "API Key"
- Copy the generated API key

#### 4. Set Up Your Local Environment

- Create a `.env` file in the project root directory:
```
GOOGLE_API_KEY=your_api_key_here
```

- Or set it as an environment variable:

**On Linux/macOS:**
```bash
export GOOGLE_API_KEY=your_api_key_here
```

**On Windows (Command Prompt):**
```cmd
set GOOGLE_API_KEY=your_api_key_here
```

**On Windows (PowerShell):**
```powershell
$env:GOOGLE_API_KEY="your_api_key_here"
```

#### 5. Secure Your API Key

⚠️ **Important Security Notes:**
- Never commit your API key to version control
- Add `.env` to your `.gitignore` file
- Restrict your API key in Google Cloud Console:
  - Go to "APIs & Services" > "Credentials"
  - Click on your API key
  - Under "Application restrictions", select your application type
  - Under "API restrictions", select the specific APIs your project uses
  - Click "SAVE"

## Running the Application

Once you've set up your Google API Key:

```bash
python main.py
```

## Usage

[Add your specific usage instructions here]

## Project Structure

```
Mutli_Agent_DateTime_Agent/
├── README.md
├── requirements.txt
├── main.py
└── [other project files]
```

## Configuration

Configure the application by:
1. Setting your Google API Key as described above
2. Modifying configuration files in the config directory (if applicable)
3. Adjusting parameters in the main application file

## Troubleshooting

### API Key Issues
- Verify that your API key is correctly set in your environment
- Check that required APIs are enabled in Google Cloud Console
- Ensure API key restrictions don't block your application

### Permission Errors
- Verify your Google Cloud project has the necessary permissions
- Check that you've enabled all required APIs
- Review Google Cloud IAM settings

## Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for bugs and feature requests.

## License

This project is open source and available under the MIT License.

## Support

For issues and questions, please open an issue on the GitHub repository.

---

**Last Updated:** 2026-04-05