# Truffle Hog

Searches through git repositories for secrets, digging deep into commit history and branches.

**Note:** Files added in the first commit of a git repository don't appear to be searched, 
see: https://github.com/dxa4481/truffleHog/issues/85

## Build

```sh
pip3 install virtualenv
virtualenv venv
source venv/bin/activate
pip install truffleHog
cp regexChecks.py venv/lib/python*/site-packages/truffleHog/defaultRegexes/regexChecks.py
#vim venv/lib/python*/site-packages/truffleHog/defaultRegexes/regexChecks.py
```

## Run

```sh
truffleHog --regex --entropy=False https://github.com/mshauneu/trufflehog
```

## Finish

```sh
deactivate
```

