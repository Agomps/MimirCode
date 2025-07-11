# MimirCode: A Smart Code Analyzer and Documentation Utility

MimirCode is a Python-based tool that simplifies code analysis, documentation, and usage. It takes existing code projects or folders, breaks them into smaller parts, and sends them to an local instance of Ollama for a thorough analysis. 

MimirCode allows a local LLM to dive into code, determining its structure, function, and purpose. The resulting documentation is clear and easy-to-understand, explaining each component's role, interaction with other parts of the project, and usage examples. This makes it easier for developers to navigate through complex projects, learn new concepts quickly, and utilize the code effectively.

# Setting Up
To get started with this project on your local machine, follow these steps:

1. First, clone the repository containing the project files to your local computer using a command line tool like Git Bash or Terminal. For example:
   ```
   git clone https://github.com/Agomps/MimirCode.git
   ```
   Replace `[username]` with the username of the repository owner and `MimirCode` with the name of the specific repository you are cloning.

2. Navigate to the project directory:
   ```
   cd MimirCode
   ```
   Replace `MimirCode` with the name of the project directory you just cloned.

3. Create a new Python virtual environment using the venv module:
   ```
   python3 -m venv venv
   ```
   This command creates a folder called `venv` in your current directory, which will contain all the necessary files for the isolated Python environment.

4. Activate the virtual environment by running:
   ```
   source venv/bin/activate
   ```
   This step puts the virtual environment into effect, so that any packages installed or modifications made to Python during this session are local to the project and don't affect other projects on your machine.

5. With the virtual environment active, you can now install the required dependencies using pip:
   ```
   pip install -r requirements.txt
   ```
   This command will install all the packages listed in the `requirements.txt` file located in the project directory. In this case, there is only one package, requests. If you want to manually install just that package without using the `requirements.txt` file, you can run:
   ```
   pip install request
   ```

After completing these steps, your local environment should be set up and ready for developing or running the project.

# Using the MimirCode


## Examples on How to Use the Code

Here are three examples demonstrating how to use the main functionalities of this code:

**Generating Documentation using `code_documentation.py`**

   The script will then process all code files in the specified directory, read their content, split it into chunks if necessary, and use the Ollama API to generate documentation for each chunk or the whole file.


```bash
python3 code_documentation.py
Enter the path to the directory containing your program files: /path/to/your/project
```


**Generating Documentation using `deep_code_documentation.py`**

The script will read the file, call Ollama to generate summary, detailed explanation, and usage examples if needed, and save the generated Markdown documentation in the specified output directory.

   ```bash
   python3 deep_code_documentation.py
   Enter the path to the directory containing your program files: /path/to/your/project
   ```

