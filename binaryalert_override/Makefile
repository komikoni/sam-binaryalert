build-LambdaFunction:
	python3 -m venv venv
	sh venv/bin/activate
	pip3 install -r requirements.txt
	python3 ./manage.py build
	unzip ./terraform/lambda_analyzer.zip -d $(ARTIFACTS_DIR)