# Example Python Subproject Directory Structure

## Dependencies

Just [Poetry](https://python-poetry.org/).  Why not pip?  [Pep 440](https://www.python.org/dev/peps/pep-0440/#file-urls) (the "pip pep") seems to imply file urls must be absolute.  Poetry does not have that requirement.

## To Use

```sh
cd projects/project1
poetry install
poetry run python project1
```

Now:

- go into module1 and edit it's `say_hi` function.
- Re-run `poetry run python project1` from `projects/project1`.  Notice that no wheels were built, but your edit shows up in project1.

## Credits

[python-monorepo](github.com/ya-mori/python-monorepo) got most of the way here.  Just a few things that author missed in setting up his repo.
