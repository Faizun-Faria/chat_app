# Python Setup for VS Code

## 1. Check Python Installation
Open **VS Code Terminal** (`Ctrl + ~` or `View > Terminal`) and run:

```sh
python --version
```
or  
```sh
python3 --version
```
If Python is not installed, [download it from python.org](https://www.python.org/downloads/).

## 2. Install Virtual Environment
Run the following in your project folder:

```sh
python -m venv venv  # Creates a virtual environment
```

Activate it:

- **Windows (CMD/Powershell):**
  ```sh
  venv\Scripts\activate
  ```
- **Mac/Linux:**
  ```sh
  source venv/bin/activate
  ```

## 3. Install VS Code Python Extension
Go to **Extensions (`Ctrl + Shift + X`)** and install **"Python" by Microsoft**.

## 4. Select the Right Python Interpreter
Press **`Ctrl + Shift + P`**, search **"Python: Select Interpreter"**, and choose the correct one.

## 5. Install Dependencies (If Required)
If your project has a `requirements.txt` file, install dependencies:

```sh
pip install -r requirements.txt
```

## 6. Check Linter & Formatter (Optional but Useful)
For clean code, install:

```sh
pip install black flake8
```
Then, in VS Code settings, set **Black** as the default formatter.

---

You're now ready to code! 🚀
