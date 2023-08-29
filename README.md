# Prospector profile duplicate

Profile that can be used to disable the duplicated or conflict rules between Prospector tools and also
external tools like and Black, isort and docformatter.

The profile considers that you are using Pylint, pyupgrade, Black, isort and docformatter and remove conflict or duplicate with them.

## Usage

```yaml
inherits:
  - duplicated
```

## Contributing

Install the pre-commit hooks:

```bash
pip install pre-commit
pre-commit install --allow-missing-config
```
