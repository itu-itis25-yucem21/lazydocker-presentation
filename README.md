# Lazydocker Presentation - YZV 322E

## 1. What is this tool?
Lazydocker is an open-source terminal UI (TUI) for managing Docker and Docker Compose environments, written in Go.It provides a single-pane dashboard to monitor container logs, view real-time performance stats, and manage images or volumes without memorizing complex CLI flags.

## 2. Prerequisites
To run this project and the tool, ensure you have the following installed:

* **Operating System:** Linux, macOS, or Windows (WSL2 recommended).
* **Docker:** v20.10.0 or higher.
* **Docker Compose:** v2.0.0 or higher.
* **Lazydocker:** See the installation section below.

## 3. Installation
To install Lazydocker on Linux/WSL, use the official installation script:
```bash
curl [https://raw.githubusercontent.com/jesseduffield/lazydocker/master/scripts/install_update_linux.sh](https://raw.githubusercontent.com/jesseduffield/lazydocker/master/scripts/install_update_linux.sh) | bash
```

(Note: For macOS users, you can use:
```bash
brew install jesseduffield/lazydocker/lazydocker
```)
## 4. Running the Example
Follow these steps to launch the demo environment and monitor it with Lazydocker:  
1. Clone this repository and navigate to the folder.
2. Start the sample containers in detached mode:
```bash
docker-compose up -d
``` 
3. Launch the Lazydocker interface:
```bash
lazydocker
```
(Note: If the command is not found, you can run it via ```bash ~/.local/bin/lazydocker ```)
## 5. Expected Output
Once executed, you should see an interactive terminal interface with the following sections:
* **Containers:** List of running services (`yzv322e-log-generator`, `yzv322e-redis-cache`, `yzv322e-web-server`).
* **Logs:** Real-time log stream of the selected container.
* **Stats:** CPU and Memory usage graphs.
> **Note:** Please refer to the `screenshot.png` file in this repository for the visual output.

## 6. AI Usage Disclosure
This project utilized Gemini 3 Flash (AI) for planning the presentation structure, drafting the README documentation according to the course criteria, and designing the sample docker-compose.yml scenario. All AI-generated suggestions were reviewed and verified for technical accuracy.
      
