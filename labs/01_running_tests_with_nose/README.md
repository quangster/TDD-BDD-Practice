# Lab: Running tests with nose

These are the source files for the lab **Running tests with node**

Required Python packages are:

- nose
- pinocchio
- coverage

Contents of `setup.cfg` should be:

```ini
[nosetests]
verbosity=2
with-spec=1
spec-color=1
with-coverage=1
cover-erase=1
cover-package=triangle

[coverage:report]
show_missing = True
```

## Test commands
```bash
# run tests
python3 -m unitest
# verbose mode
python3 -m unitest -v 
# nose
nosetests -v
# Nicer formatting and a colorful output
nosetests --with-spec --spec-color
# Test coverage
nosetests --with-spec --spec-color --with-coverage
# Coverage report
coverage report -m
# Save config for nosetests at setup.cfg file
nosetests
```