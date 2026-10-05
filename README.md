# django-app-template

This is a template repository for creating new Django apps.

To use, simply create a new repository
[using this repository as a template](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template),
rename the `src/app` directory to the name of your app, and edit the `pyproject.toml` file.

## Development

Set up your development environment:

1. Install [uv](https://docs.astral.sh/uv/):
   ```bash
   # On macOS/Linux:
   curl -LsSf https://astral.sh/uv/install.sh | sh
   # Or with pip:
   pip install uv
   ```

2. Create a virtual environment and install dependencies:
   ```bash
   uv sync
   ```

3. Copy `example.env` to `.env` and configure your environment variables.

4. Run migrations:
   ```bash
   uv run python manage.py migrate
   ```

5. (Optional) Install pre-commit hooks:
   ```bash
   uv run pre-commit install
   ```
