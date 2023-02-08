Questionnaire Pull Lambda
This repository contains code for lambda function which will pull questionnaire data from DMDP API's. It uses config file to use API's based on environment and pulls data from those API's. It pulls data from below API's:

AccessRef
User
Study
Organization
Questionnaire response It combines all the API's data based on joining condition provided by Unify team.

File Structure
This project consists of lambda function code.

|-workflows/ [folder containing templates and build scripts]
|-main/
  |-__init__.py [Initialisation of code]
  |-device_api_config.json [Contains lambda functions environment parameters based on the environment]
  |-lambda_function.py [Contains lambda function code]
|-tests/ [Glue job scripts]
    |-__init__.py [Contains unit test cases for lambda function]
|-requirements.txt/ [Contains python dependencies]
|-device_api_config.json/ [Contains lambda functions environment parameters based on the environment]
