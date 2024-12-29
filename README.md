# README

Here is a repo containing my preferred custom git-hooks. Starting off, this is just `prepare-commit-msg`.

## Usage

Either cp the choosen hook into `.git/hooks`

or manage it with

### pre-commit

in `.pre-commit-config.yaml`:

```yaml
repos:
  - repo: local
    hooks:
      - id: prepare-commit-msg
        name: prepare-commit-msg
        entry: python3 scripts/prepare-commit-msg
        language: system
        stages: [prepare-commit-msg]
```
