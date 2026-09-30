# CFTC Managed Money — Net Long: CBOT Corn, SRW Wheat, Soybeans

A Jupyter notebook that pulls weekly CFTC Managed Money positions for corn, SRW wheat, and
soybeans and charts net long for 2026 (with and without WASDE release windows), the full history since 2016, and a year-by-year seasonal overlay.

## Get the code

Fork [tlayers21/coins-ags-managed-money](https://github.com/tlayers21/coins-ags-managed-money)
on GitHub (**Fork** button, top right), then clone your fork:

```bash
git clone https://github.com/<your-username>/coins-ags-managed-money.git
cd coins-ags-managed-money
```

## Set up

1. Install [uv](https://docs.astral.sh/uv/getting-started/installation/) if you don't have it:

   ```bash
   curl -LsSf https://astral.sh/uv/install.sh | sh
   ```

2. Install dependencies. uv creates a `.venv` and installs Python 3.11+ if needed:

   ```bash
   uv sync
   ```

   Then choose **Run → Run All Cells**. The data downloads from the CFTC public API, and no API
   key is needed.

   **VS Code:** open the notebook, click **Select Kernel**, and look for your virtual environment.
