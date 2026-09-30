# CFTC Managed Money — Net Long: CBOT Corn, SRW Wheat, Soybeans

A Jupyter notebook that pulls weekly CFTC Managed Money positions for corn, SRW wheat, and
soybeans and charts net long for 2026 (with and without WASDE release windows), the full history since 2016, and a year-by-year seasonal overlay.

## Get the code

**Just want to run it?** Clone the repo:

```bash
git clone https://github.com/<owner>/managed_money.git
cd managed_money
```

**Want to contribute?** Fork the repo on GitHub, then clone your fork:

```bash
git clone https://github.com/<your-username>/managed_money.git
cd managed_money
```

Push changes to a branch on your fork and open a pull request.

## Set up

1. Install [uv](https://docs.astral.sh/uv/getting-started/installation/) if you don't have it:

   ```bash
   curl -LsSf https://astral.sh/uv/install.sh | sh
   ```

2. Install dependencies. uv creates a `.venv` and installs Python 3.11+ if needed:

   ```bash
   uv sync
   ```

3. Register the project's Jupyter kernel (one time). The notebook runs on this kernel so it uses
   the project's `.venv` and not a global Python:

   ```bash
   uv run python -m ipykernel install --sys-prefix --name managed-money --display-name "Python (managed-money)"
   ```

4. Open the notebook:

   ```bash
   uv run jupyter lab managed_money.ipynb
   ```

   Then choose **Run → Run All Cells**. The data downloads from the CFTC public API, and no API
   key is needed.

   **VS Code:** open the notebook, click **Select Kernel** (top right), and choose
   **Python (managed-money)** or `.venv/bin/python`.
