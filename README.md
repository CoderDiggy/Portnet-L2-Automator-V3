# Portnet L2 Automator V3

Short guide to get this project running locally.

## Requirements
- Python 3.11 is required. Make sure your `python` binary is Python 3.11.
  - Check with:
  ```bash
  python3.11 --version
  # or, if you use `python`:
  python --version
  ```
- Recommended: virtual environment for isolation (venv).

## Quick start (recommended)
1. Clone the repository (if you haven't already):
   ```bash
   git clone https://github.com/CoderDiggy/Portnet-L2-Automator-V3.git
   cd Portnet-L2-Automator-V3
   ```

2. Create and activate a virtual environment using Python 3.11:
   - macOS / Linux:
     ```bash
     python3.11 -m venv .venv
     source .venv/bin/activate
     ```
   - Windows (PowerShell):
     ```powershell
     python3.11 -m venv .venv
     .\.venv\Scripts\Activate.ps1
     ```
   - Windows (cmd.exe):
     ```
     python3.11 -m venv .venv
     .\.venv\Scripts\activate
     ```

3. Install dependencies
   - If there's a requirements file inside the AI_Assistant_Python folder:
     ```bash
     pip install -r AI_Assistant_Python/requirements.txt
     ```
   - If requirements are at repo root:
     ```bash
     pip install -r requirements.txt
     ```
   - If no requirements file exists, install packages as directed by project documentation or the maintainers.

4. Change into the AI_Assistant_Python folder and run simple_main
   ```bash
   cd AI_Assistant_Python
   # If simple_main is a script file named simple_main.py:
   python simple_main.py

   # OR if it is a module:
   python -m simple_main
   ```

   Note: The explicit instruction is to run `simple_main` after `cd "AI_Assistant_Python"`. Use the invocation that matches the repository layout (`simple_main.py` vs. module).

## Common issues & troubleshooting
- "python: command not found" or wrong version:
  - Ensure Python 3.11 is installed and accessible as `python3.11` or update your PATH.
- Dependency installation errors:
  - Upgrade pip: `pip install --upgrade pip`
  - Re-run install: `pip install -r AI_Assistant_Python/requirements.txt`
- Virtual environment not activated:
  - Make sure you activated the venv before running the app so dependencies resolve correctly.
- If `simple_main` is not found:
  - List the files in `AI_Assistant_Python` to confirm its name:
    ```bash
    ls AI_Assistant_Python
    ```
  - Look for `simple_main.py` or a package with `__main__.py` or a module named `simple_main`.

## Development tips
- Use git branches for features and fixes.
- Run linters / formatters if present in repo (e.g., `ruff`, `black`) before committing.
- Add tests for new features where applicable.

## Contributing
Please open an issue or pull request with a clear description of the change, reasoning, and any testing steps.

## License
Check the repository for a LICENSE file. If none is present, contact the repository owner for licensing details.
