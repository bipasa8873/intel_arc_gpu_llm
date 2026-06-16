# 🤖 intel_arc_gpu_llm - Run local artificial intelligence on Arc

![Download Releases](https://img.shields.io/badge/Download-Releases-blue)

[https://github.com/bipasa8873/intel_arc_gpu_llm/releases](https://github.com/bipasa8873/intel_arc_gpu_llm/releases)

intel_arc_gpu_llm helps you run powerful language models on your computer. You use your Intel Arc Pro B60 GPU to process text quickly. The software works like a private server on your machine. You send requests to the server, and it provides answers. Your data stays on your local hardware. You do not send your files or chats to external companies. The setup uses Docker technology to keep your system clean.

## ⚙️ Minimum System Requirements

Your computer needs specific parts to run this tool well. Check these specs before you start:

- Operating System: Windows 10 or 11 with the latest updates.
- Processor: Intel Core i5 or better.
- Memory: 32 GB of RAM.
- Graphics Card: Intel Arc Pro B60 GPU.
- Storage: 50 GB of free space on an SSD.
- Drivers: The latest Intel Arc GPU drivers from the Intel website.

Verify that your drivers are current. Old drivers cause errors during the setup process. Visit the Intel website to download the latest software for your graphics card.

## 📥 Download and Setup

Follow these steps to prepare your computer.

1. Visit the project website at [https://github.com/bipasa8873/intel_arc_gpu_llm/releases](https://github.com/bipasa8873/intel_arc_gpu_llm/releases).
2. Look for the latest version of the files.
3. Download the installation archive to your desktop.
4. Extract the folder to a location you can find easily.
5. Install Docker Desktop for Windows from the official Docker website.
6. Restart your computer after the Docker installation completes.

## 🚀 Running the Server

Open your terminal or command prompt to start the server.

1. Open the folder you extracted earlier.
2. Type `cd` followed by the folder path in your terminal.
3. Type the command `docker-compose up` and press Enter.
4. Wait for the initial download of model files. This takes time depending on your internet speed.
5. The window shows logs once the server is ready. Do not close this terminal window while you use the AI.
6. Open your web browser once the logs show the server is active.

## 🔗 Connecting to the AI

Your local server provides an address for your applications. Use this address to connect your favorite interface tools.

- Server URL: http://localhost:8000
- API Access: Point your chat software to the local endpoint.
- Model Support: The server loads the model defined in the configuration file.

If the page does not load, wait a few minutes. The GPU needs time to load the model into memory. Check the terminal window for any error messages in red text.

## 🛠️ Troubleshooting Common Issues

Errors happen sometimes. Follow these tips to resolve them.

- Docker is not running: Open Docker Desktop and wait until the green icon appears.
- Port conflict: If port 8000 is in use, change the port number in the docker-compose.yml file.
- Out of memory: Close other programs like web browsers or games to free up your GPU memory.
- Drive space: Delete old files if the download fails due to a full disk.

## 📄 Managing Models

You can change the language model inside the configuration folder. 

1. Locate the model configuration file in the project directory.
2. Edit the name of the model you want to load.
3. Save the file.
4. Stop the server by pressing Ctrl+C in the terminal.
5. Run the command `docker-compose up` again to restart with new settings.

## 🔐 Privacy and Security

This tool runs entirely on your hardware. You own the data. No external entity tracks your inputs or outputs. You can disconnect your internet once the initial download completes. The local server works without an active connection to the web. 

## ⚖️ Features

- Simple deployment with one command.
- Standard interface that works with most AI chat clients.
- Hardware acceleration using Intel XPU technology.
- Reliable performance for text creation tasks.
- Reproducible config for consistent results.

## 🎓 Tips for Best Results

Keep your system cool. Running AI models makes your GPU work hard. Ensure your computer case has good airflow. If you notice slow performance, reduce the number of concurrent requests. One request at a time allows the GPU to finish the task faster. 

Monitor your GPU usage task manager. Look for the Intel Arc section. It shows how much memory the model uses while it runs. Most models require at least 12 GB of GPU video memory to run smoothly. 

## 📦 Updating the Tool

Check the release page once per month for updates. New versions often contain speed improvements. 

1. Download the new version from the repository.
2. Replace your old file folder with the new content.
3. Keep your configuration files if you made special changes.
4. Restart the Docker container to apply the changes.

## ❓ Frequently Asked Questions

Can I use this for business? Yes, the software is free for personal and professional use.
Does it work on laptops? Yes, provided the laptop has the required graphics card and cooling.
Is internet required? Only for the first install.
Can I change the settings? Yes, all settings exist in the plain text configuration file.
What happens if the power cuts off? The server stops. You must restart it when power returns.

Follow these instructions to keep your local AI running without issues. Treat your hardware with care and allow adequate ventilation for the GPU during long sessions.