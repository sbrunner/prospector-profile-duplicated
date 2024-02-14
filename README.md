# Prospector profile duplicate

Profile that can be used to disable the duplicated or conflict rules between Prospector tools and also
external tools like and Black, isort and docformatter.

The profile considers that you are using Pylint, pyupgrade, Black, isort, docformatter and autoflake and remove conflict or duplicate with them.

## Usage

```yaml
inherits:
  # Get All
  - duplicated
  # Get for individual tools
  - duplicated:black
  - duplicated:isort
  - duplicated:pyupgrade
  - duplicated:pylint
  - duplicated:docformatter
  - duplicated:autoflake
```

## Contributing

Install the pre-commit hooks:

```bash
pip install pre-commit
pre-commit install --allow-missing-config
```
