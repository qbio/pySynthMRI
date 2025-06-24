Make sure that you have Python 3.11 or newer, then you can start like this:

```bash
uv venv
uv pip compile requirements.txt --python 3.11 --output-file uv.lock
uv pip install --requirements uv.lock
```

If you update the uv.lock
```bash
  uv pip sync uv.lock
```

Run the tool
```bash
  uv run python -m src.pySynthMRI
```