# static_flask
[Medium tutorial](https://medium.com/swlh/baking-static-sites-with-python-and-jinja-330fe29bbe08) for news aggregator in Flask created by [@mattvh](https://github.com/mattvh).

## Setup
* Install [pipenv](https://realpython.com/pipenv-guide/)
* Clone repo
* Install dependencies
```bash
# clone
git clone https://github.com/pythoninthegrass/static_flask.git
cd static_flask/

# install pipenv dependencies
pipenv install
```

## Generate HTML only
* Move `style.css` out of public and template static directories
* Run `generator.py`
```bash
pipenv shell
python generator.py
open public/index.html
```

## Generate HTML + CSS
* Leave `style.css` in-place
* Run `generator.py`
```bash
pipenv shell
python generator.py
open public/index.html
```

## TODO
* Refactor with [News API](https://newsapi.org/docs/client-libraries/python)
* Setup Flask environment for localhost
* CI/CD
* Create API to update or hard-code articles
* Database to store previous days' hits
* Redesign CSS layout
* Deploy to Digital Ocean
