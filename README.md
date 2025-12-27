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
```

