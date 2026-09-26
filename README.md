# Harness Engineering Python Template

This repository contains Cursor rules for building reliable Python coding and test harnesses.

## File location

- Cursor rules: `.cursor/rules/harness-engineering-python.mdc`

## Use with Cursor

Clone the repository, then copy the `.cursor` directory into your Python project, or copy the rule file into your project's `.cursor/rules/` directory.

```bash
git clone https://github.com/liangyuzhu888/harness-engineering-python.git
cp -R harness-engineering-python/.cursor /path/to/your-python-project/
```

The rule is written in Cursor's `.mdc` format and applies as project guidance when Cursor reads the project rules.

## Recommended project checks

```bash
python -m pip install pytest ruff mypy
ruff format --check .
ruff check .
pytest
mypy .
```

Review the rule file and adapt the checklist to your team's Python version, CI system, and hardware or service integrations.
