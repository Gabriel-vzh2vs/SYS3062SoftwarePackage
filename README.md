A UV project for SYS3062 at the University of Virginia! (An Easy Install, I hope...)

## Getting Started

Follow these steps to set up the project and run the software package.

### 1. Install `uv`
This project uses `uv` to manage Python dependencies automatically. If you don't have it, install it first:

* **macOS / Linux:**
    ```bash
    curl -LsSf [https://astral.sh/uv/install.sh](https://astral.sh/uv/install.sh) | sh
    ```
* **Windows:**
    ```powershell
    powershell -c "irm [https://astral.sh/uv/install.ps1](https://astral.sh/uv/install.ps1) | iex"
    ```
*(You may need to restart your terminal after installing)*

### 2. Clone and Run
You do not need to manually install libraries. Just clone the repo and tell `uv` to run the main script.

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/username/repository-name.git](https://github.com/username/repository-name.git)
    cd repository-name
    ```

2.  **Run the application:**
    ```bash
    uv run main.py
    ```

**Note:** The first time you run this command, `uv` will automatically create a virtual environment and download all necessary dependencies. Subsequent runs will be instant.


## 💻 Developing in VS Code

To get features like auto-complete and error checking, you need to tell VS Code to use the environment managed by `uv`.

### 1. Open the Project
Open VS Code, go to **File > Open Folder...**, and select the `repository-name` folder you just cloned.

### 2. Install the Python Extension
If you haven't already, click the **Extensions** icon (boxes on the left) and install the **Python** extension by Microsoft.

### 3. Select the Correct Interpreter
VS Code needs to know where your installed libraries (like numpy or pandas) are.

1.  Press `Ctrl + Shift + P` (Windows/Linux) or `Cmd + Shift + P` (Mac) to open the Command Palette.
2.  Type and select: **Python: Select Interpreter**.
3.  Look for the option marked **Recommended** or that contains `.venv` in the path. It usually looks like this:
    * `Python 3.x.x ('.venv': venv) .venv/bin/python`
4.  If you don't see it, ensure you have run `uv run main.py` at least once (this creates the `.venv` folder).

### 4. Verify Setup
* Open any Python file (e.g., `main.py`).
* Look at the bottom-right corner of the VS Code window. You should see the Python version followed by `('.venv')`.
* If you open a new Terminal in VS Code (**Terminal > New Terminal**), you should see `(.venv)` appear at the start of the command prompt line.

---
### ⚡️ Pro Tip: Running Your Code
You now have two ways to run your code:

1.  **The "Official" Way:** Type `uv run main.py` in the terminal. This is 100% reliable and ensures dependencies are synced.
2.  **The "VS Code" Way:** Click the **Play Button** (▶) in the top right. This works great for quick testing *if* you completed Step 3 correctly.
```
