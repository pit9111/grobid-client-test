Ceci est un repository expérimental dédié à faire des tests

## Getting started

```bash
# 1. Create a workspace folder to keep repositories side-by-side
mkdir my-grobid-project
cd my-grobid-project

# 2. Clone both repositories
git clone [https://github.com/pit9111/grobid-client-python](https://github.com/pit9111/grobid-client-python)
git clone [https://github.com/pit9111/grobid-client-test](https://github.com/pit9111/grobid-client-test)

# 3. Enter the scripts repository
cd grobid-client-test

# 4. Setup Python environment with uv
uv venv --python 3.12

# 5. Activate environment
# On Windows:
.venv\Scripts\activate
# On Linux/Mac:
# source .venv/bin/activate

# 6. Install the sibling library in editable mode
uv pip install -e ../grobid-client-python

# 7. Prepare input folder & download a sample
mkdir input_pdf

# 8. Run the script
uv run python main.py
