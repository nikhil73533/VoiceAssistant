# Assistant Functionality Module

## Overview

This project implements a voice assistant application that leverages WebRTC for real-time communication between the client and the agent. The assistant, embodied by Nikhil Gupta, provides insights into his professional journey, personal attributes, and areas of growth.

**Summary of Findings and High-Level Approach**

The provided code outlines the development of a voice assistant application utilizing Python, with real-time communication facilitated through WebRTC. The core components of this implementation include:

1. **Assistant Functionality Module (`AssistantFnc` Class)**:
   - This class, inheriting from `llm.FunctionContext`, encapsulates personal information about Nikhil Gupta. It provides methods to retrieve details such as his life story, superpower, growth areas, common misconceptions, and how he pushes his limits.

2. **WebRTC Integration**:
   - The application employs WebRTC to enable real-time audio communication between the agent and the client. This is achieved using the `aiortc` library, which offers a Pythonic approach to implementing WebRTC and Object Real-Time Communications (ORTC) using asyncio. citeturn0search3

3. **Agent Initialization and Management**:
   - Within the `entrypoint` function, the application establishes a connection to a room and awaits participant interaction. An instance of `AssistantFnc` is created, and a multimodal agent is initialized using the `google.beta.realtime.RealtimeModel`. This agent is responsible for managing the communication flow, starting the interaction, and generating appropriate replies based on the user's input.

**High-Level Implementation Approach**:

- **Environment Setup**:
  - Ensure that Python 3.6 or higher is installed.
  - Install necessary dependencies, including `aiortc` for WebRTC functionalities and other packages specified in the `requirements.txt` file.

- **Signaling Mechanism**:
  - Implement a signaling server to facilitate the exchange of connection information (e.g., ICE candidates, session descriptions) between peers. This is a crucial step in establishing a WebRTC connection. citeturn0search5

- **Media Stream Handling**:
  - Utilize the `aiortc` library to manage media streams, enabling the transmission of audio data between the client and the agent. This involves capturing audio input, encoding/decoding media streams, and handling real-time communication protocols.

- **Agent Functionality**:
  - Define the `AssistantFnc` class to handle various user queries. This class should include methods that provide responses based on predefined personal information about Nikhil Gupta.

- **Application Deployment**:
  - Deploy the application on a server that supports asynchronous operations and WebRTC capabilities. Ensure that necessary ports are open and that the signaling server is accessible to clients.

## Prerequisites

- **Python Version**: Ensure Python 3.6 or higher is installed.
- **WebRTC Dependencies**: Install the `aiortc` library for WebRTC functionalities.
- **Additional Packages**: Refer to the `requirements.txt` file for other necessary Python packages.

## Installation

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/yourusername/assistant-functionality-module.git
   cd assistant-functionality-module
   ```

2. **Create a Virtual Environment** (optional but recommended):

   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. **Install Dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

```bash
python3 agent.py dev
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Video Demonstration

To get a visual overview of the product, click on the link below:

[Product Video](https://www.canva.com/design/DAGiM-g_hEA/3JiipW6Fr_DX_T3IcRX8-A/watch?utm_content=DAGiM-g_hEA&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h48467262ca)