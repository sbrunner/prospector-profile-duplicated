# Prospector profile duplicate

Profile that can be used to disable the duplicated or conflict rules between Prospector tools and also
external tools like and Black, isort and docformatter.

The profile considers that you are using pyupgrade, Black, isort, docformatter and autoflake or Ruff and remove conflict or duplicate with them.

## Usage

```yaml
inherits:
  # Get Black / isort
  - duplicated
  # Get for individual tools
  - duplicated:black
  - duplicated:isort
  - duplicated:pyupgrade
  - duplicated:docformatter
  - duplicated:pydocstyle
```

## Contributing

Install the pre-commit hooks:

```bash
pip install pre-commit
pre-commit install --allow-missing-config
```
