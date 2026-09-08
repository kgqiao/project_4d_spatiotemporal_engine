{
"Virtual Environment Setup": {
    "prefix": "venv_setup",
    "body": [
        "# ⚙️ INITIAL SETUP",
        "",
        "## 🛠️ Create Virtual Environment",
        "",
        "1. **Navigate to project directory in terminal:**",
        "`H:\CODING_PROJECTS\4d_spatiotemporal_engine`",
        "",
        "2. **Create Virtual Environment:**",
        "   - `python -m venv venv_st_engine`",
        "   - OR: `py -3.12 -m venv ${2:desired_venv_name}`",
        "",
        "2.6. **If need virtual env package installation from embedded portable pi files:**",
        "   - `powershell -Command "Invoke-WebRequest -Uri 'https://bootstrap.pypa.io/virtualenv.pyz' -OutFile 'virtualenv.pyz'"`",
        "",
        "2.5. **Create the virtual environment using the portable python.exe:**",
        "   - `\python_312_portable\python.exe -m venv {desired_venv_name}`",
        "",
        "3. **Activate the virtual environment:**",
        "   *(Required every time you start working to ensure packages stay isolated)*",
        "   - Windows Command Prompt: `venv_st_engine\Scripts\activate.bat`",
        "   - Windows Git Bash: `source ${2:desired_venv_name}/Scripts/activate`",
        "",
        "4. **Select the Python Interpreter in VS Code:**",
        "   - Press `Ctrl + Shift + P` and type `Python: Select Interpreter`.",
        "   - Look for the entry pointing to your `.venv` folder.",
        "   - If missing, click `Enter interpreter path...` and browse to `${2:desired_venv_name}\\\\Scripts\\\\python.exe`.",
        "",
        "5. **Choose the Python Environment Kernel:**",
        "   - Click the Kernel name in the top-right corner of your notebook.",
        "   - Select `Python Environments...` and choose your recommended environment.",
        "",
        "6. **Install Jupyter Kernel Support:**",
        "   - `pip install ipykernel`",
        "",
        "---",
        "",
        "# 🔁 EACH TIME FILE IS OPENED",
        "",
        "### 🖥️ KQ-PC:",
        "1. **Navigate:** `cd ${3:H:\\\\CODING-GITHUB\\\\learning_machine_learning\\\\class_usc_202601_mlfordatascience}`",
        "2. **Environment Name:** `${4:dsci552_venv}`",
        "3. **Activate:** `${4:dsci552_venv}\\\\Scripts\\\\activate`",
        "",
        "### 💻 ASUS TUF Gaming A15 Laptop:",
        "1. **Navigate:** `cd ${5:C:\\\\Users\\\\kathy\\\\Documents\\\\GitHub\\\\learning_machine_learning\\\\class_usc_202601_mlfordatascience}`",
        "2. **Environment Name:** `${6:dsci552_venv_a15}`",
        "3. **Activate:** `${6:dsci552_venv_a15}\\\\Scripts\\\\activate`",
        "",
        "---",
        "",
        "### 🔍 Verify Current Jupyter Environment Path",
        "Run this snippet inside a notebook cell to see exactly where Python is executing from:",
        "```python",
        "import sys",
        "print(sys.executable)",
        "```",
        "$0"
    ],
    "description": "Inserts variable-based virtual environment and kernel setup workflow notes."
}

}


##### Python 3.12 Specific Version - Create Virtual Environment for Open3D
# cd H:\CODING_PROJECTS\project_3d_perception_pipeline
# python312_portable\python.exe -m venv depth_est_venv_312
# depth_est_venv_312\Scripts\Activate
# deactivate
#if can't find kernel, find the manual path of the folder/venv folder/Python.exe