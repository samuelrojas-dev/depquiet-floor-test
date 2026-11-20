# depquiet-floor-test

A minimal uv project to see what Dependabot says when the fix for a vulnerable dependency
needs a newer Python than `requires-python` allows.

- `requires-python = ">=3.10"`
- `soupsieve` 2.8.3 is locked (through `beautifulsoup4`). Every fixed soupsieve release
  needs Python 3.11.5.
- `pillow` 12.2.0 is locked. The fixed pillow releases need Python 3.11.

Nothing here is meant to run: it only exists for Dependabot and
[depquiet](https://github.com/samuelrojas-dev/depquiet) to look at.
