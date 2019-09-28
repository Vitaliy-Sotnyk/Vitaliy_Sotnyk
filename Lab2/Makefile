.DEFAULT_GOAL := all

all: install test run deploy

install:
	@echo "Installing pipenv and dependencies."
	@pip install pipenv
	@pipenv --python 3.7
	@pipenv install requests
	@pipenv install ntplib

test:
	@echo "Start tests."
	@pytest test.py>result.txt

run:
	@echo "Run Python app."
	@python app.py>>result.text

deploy:
	@echo "Adding and Committing results.txt to git."
	@git add -A
	@git commit - m "Lab2: ..."
	@git push