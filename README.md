![Python](https://img.shields.io/badge/Python-3.x-blue)
![Platform](https://img.shields.io/badge/Platform-Linux-green)
![License](https://img.shields.io/badge/License-MIT-orange)
![CLI Tool](https://img.shields.io/badge/Interface-CLI-black)
![OpenAI](https://img.shields.io/badge/API-OpenAI-purple)


# Short Introduction

`max` is a lightweight **command-line AI assistant** that allows developers to interact with an AI model directly from the terminal.
Instead of opening a browser or external application, users can simply run:

```bash
max how to restart nginx
```

and instantly receive AI-generated answers in the terminal.

The goal of this project was to create a **fast, minimal, and developer-friendly AI tool** that integrates directly into daily workflows.


# Technologies Used

* **Python**
* **OpenAI API**
* **Linux CLI**
* **Virtual Environments**
* **Shell scripting**
* **Symbolic linking**
* **Git & GitHub**


# Features

* Run AI queries directly from the terminal
* Global CLI command (`max`)
* Lightweight and fast
* Works inside a Python virtual environment
* Simple installation
* Easily extendable

Example usage:

```bash
max how to restart nginx
```


# Process: How I Built It

1. Designed a simple **Python CLI script** that accepts user input.
2. Integrated the **Cohere** and **Bytez** to process prompts and return responses.
3. Implemented argument parsing to capture user queries.
4. Configured a **Python virtual environment** to manage dependencies.
5. Added a **shebang line** so the script could run as an executable.
6. Made the script executable using:

```bash
chmod +x max
```

7. Created a **symbolic link in `/usr/local/bin`** to allow the command to run globally:

```bash
sudo ln -s ~/max-assistant/max /usr/local/bin/max
```

8. Tested the command from different directories to ensure it works system-wide.


# What I Learned

This project helped me understand several important development concepts:

* How **CLI tools work in Linux**
* How to create **executable scripts**
* Managing Python environments using **venv**
* Using **symbolic links to create global commands**
* Integrating external APIs into applications
* Designing tools that improve developer workflows


# Overall Growth

Building this project improved my understanding of:

* System-level tooling
* Automation
* Developer productivity tools
* Writing software that integrates with the operating system

It also strengthened my skills in **Python scripting, Linux environments, and API integration**.

# How This Project Can Be Improved


Potential improvements include:

* Add **config files for user preferences**
* Support **multiple AI providers**
* Add **colorized terminal output**
* Package the project as a **pip installable CLI tool**
* Support **streaming responses**


# Running the Project

### 1. Clone the repository

```bash
git clone https://github.com/astigPree/max-linux-terminal-ai.git
cd max-linux-terminal-ai
```

---

### 2. Create a virtual environment

```bash
python3 -m venv venv
source venv/bin/activate
```

---

### 3. Install dependencies

```bash
pip install requests
```

---

### 4. Make the script executable

```bash
chmod +x max
```

---

### 5. Create the global command

```bash
sudo ln -s $(pwd)/max /usr/local/bin/max
```

---

### 6. Run the assistant

```bash
max how to check disk usage
```




