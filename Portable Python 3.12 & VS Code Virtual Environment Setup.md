# Portable Python 3.12 & VS Code Virtual Environment Setup

### 1. Download & Extract Portable Python
1. Download the **Windows embeddable package (64-bit)** for **Python 3.12** from the official site.
2. Create a folder inside your project directory named `python-portable`.
3. Extract the `.zip` contents directly into that `python-portable` folder.

### 2. Quick Config for Virtual EnvironmentsSince this embeddable version skips the system registry completely, you just need to tell it to look for local packages:

1. Open the file python312._pth inside your new folder using Notepad.
2. Remove the # from the very last line so it explicitly reads:

`import site`

### 3. Initialize the Virtual Environment
Open your terminal and run the following commands sequentially to create and activate the local environment:

```bash
# Navigate to project root
cd "{1:path/to/your/project}"

# Create virtual environment named .venv using the portable python build
.\python-portable\python.exe -m venv .venv

# Activate the environment (Windows CMD / PowerShell)
.\.venv\Scripts\activate
```

### 4. Configure VS Code Workspace
Create a `.vscode/settings.json` file in your root folder to force VS Code to use this specific interpreter:

```json
{
    "python.defaultInterpreterPath": "${workspaceFolder}\.venv\Scripts\python.exe",
    "python.terminal.activateEnvironment": true
}
```