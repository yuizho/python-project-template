# Getting Started
```shell
# configure project name
sed -i -e "s/my-package/your-package-name/" setup.cfg
sed -i -e "s/my-package/your-package-name/" Pipfile

# init project
pipenv install --dev

# register source dir as package for development
# same as "python setup.py develop"
# https://qiita.com/edvakf@github/items/d82cd7ab77ea2b88506c
pipenv install -e .

# run test
pipenv run pytest tests/test-main.py
```