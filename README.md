# AI-Powered Virtual Assistant

## Overview

The **AI-Powered Virtual Assistant** is a project that integrates voice and video capabilities to create a fully interactive virtual assistant. The assistant can **see** and **hear** using APIs like **LiveKit** for video/audio processing and **Deepgram** for speech recognition, combined with **OpenAI** for generating intelligent responses. The project uses Python and can be easily set up by following the steps below.

## Features
- **Multimodal Interactions**: The assistant can process both voice (via microphone) and visual input (via webcam).
- **Real-time Conversations**: The assistant responds in real time using advanced AI models.
- **Seamless Setup**: Simple configuration using environment variables and Python's virtual environment tools.
  
## Requirements
- **Python** (3.7 or higher)
- **Virtual Environment**: Created using `venv` or `conda`.
- **API keys** from LiveKit, Deepgram, and OpenAI.

## Setup Instructions

### Step 1: Clone the Project

To clone the project repository, use the following command:

```bash
git clone https://github.com/AaftabAalam/AI-Powered-Virtual-Assistant.git
```

This will download the complete code to your local machine.

### Step 2: Create a Virtual Environment

Before running the project, it is essential to create a virtual environment to manage dependencies. You can do this using `venv` or `conda`.

#### Using `venv`:

```bash
python3 -m venv venv
source venv/bin/activate  # For macOS/Linux
venv\Scripts\activate  # For Windows
```

#### Using `conda`:

```bash
conda create --name ai_virtual_assistant python=3.8
conda activate ai_virtual_assistant
```

### Step 3: Install Dependencies

Once the virtual environment is active, install the required dependencies using the `requirements.txt` file:

```bash
pip install -r requirements.txt
```

This command installs all the libraries and modules necessary to run the project.

### Step 4: Configure the Environment Variables

Within your project directory, create a `.env` file to store the required API keys. The `.env` file should contain the following keys:

```plaintext
livekit_url=<your-livekit-url>
livekit_api_key=<your-livekit-api-key>
livekit_api_secret_key=<your-livekit-api-secret-key>
deepgram_api_key=<your-deepgram-api-key>
openai_api_key=<your-openai-api-key>
```

#### How to get the API keys:
1. **LiveKit**: Visit the LiveKit web app and generate an API key. You will receive three pieces of information:
   - `livekit_url`
   - `livekit_api_key`
   - `livekit_api_secret_key`

2. **Deepgram**: Sign up at [Deepgram](https://deepgram.com) and create an API key for speech recognition.

3. **OpenAI**: Sign up at [OpenAI](https://openai.com) to generate an API key for intelligent response generation.

Make sure to store these keys securely in the `.env` file.

### Step 5: Download Required Files

Once the environment is set up and the necessary API keys are configured, you need to download additional files required for the `bot1.py` script. Run the following command in the terminal:

```bash
python3 bot1.py download-files
```

This will download any resources required by the virtual assistant, such as language models or other dependencies.

### Step 6: Start the Project

Once everything is ready, run the virtual assistant by executing the following command in your terminal:

```bash
python3 bot1.py start
```

This will launch the assistant.

### Step 7: Connect to the LiveKit App

After the project is running, visit the following website to connect to the LiveKit application:

[https://agents-playground.livekit.io/](https://agents-playground.livekit.io/)

Once connected, the virtual assistant will be able to interact via the LiveKit platform, responding to queries using both video and audio capabilities.

## Troubleshooting

- Ensure that your `.env` file is correctly configured with all the required API keys.
- Make sure the virtual environment is active when running commands.
- If dependencies are missing, re-run `pip install -r requirements.txt`.

## Contributing

Feel free to fork the project and submit pull requests for any new features, improvements, or bug fixes.
