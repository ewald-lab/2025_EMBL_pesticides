We use uv as a Python package manager. The environment for this module is called pesticides. To install and activate the environment:

```
# Create the uv environment (only needed the first time)
uv venv --python=3.12 pesticides

# Activate the environment
source pesticides/bin/activate  # On macOS/Linux
# pesticides\Scripts\activate   # On Windows (PowerShell or cmd)

# Install dependencies
uv pip install -r requirements.txt
```

To update the requirements.txt, run:
```
poetry export --without-hashes --format=requirements.txt > requirements.txt
```