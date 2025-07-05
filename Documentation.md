
# Environment setup before proceeding further
* UV is a package manager. A wrapper over python
## check the list of installations in the env
uv pip list
Using Python 3.13.5 environment at: /opt/homebrew/opt/python@3.13/Frameworks/Python.framework/Versions/3.13
Package Version
------- -------
pip     25.1.1
wheel   0.45.1
* Rust is faster than python

## install any package inside uv env
$ uv pip install langchain

## intiate virtual env 
$ uv venv env --python  cpython-3.13.5-macos-aarch64-none

## Activate the venv. (env) will reflect after running the script
$ zsh /Users/himansu.panigrahy/Documents/Personal_Projects/AI-Projects/AI_Trip_Planner/env/bin/activate

## List packages in the environment
uv pip list 
Using Python 3.13.5 environment at: env

## install Langchain
 uv pip install langchain

## uv pip list --> all packages with langchain

## Directories 
  * agent: agentic workflow to be written
  * config: all the config files in yaml format
  * prompt_library: prompts to be written
  * tools: all reqyired tools 
  * utils: all utilities 
  * .env file: env specific information
  * app.py: application code
  * main.py: program initiates from main.py file
  * __init__.py: inside each directory, Python treats directories containing an __init__.py file as packages. so that import is easy
  * notebook: experiments 
  * logger: for logging
  * exception: capture exceptions

## Tools:
  * currency_conversion_tool.py
  * place_search_tool.py
  * weather_info_tool.py
  * arithmatic_op_tool.py
  * calculator_tool.py
  * logger 
## Requirements Update
  * fastapi: create endpoint using fastapi
  * python-dotenv: interact with python env through python-dotenv
  * streamlit: print on ui, not on terminal
  * uvicon: running server
  * -e . --> its for all local packages
## setup.py : setup is the main function.
## Install requirements:
  * initiate venv
    uv venv env --python  cpython-3.13.5-macos-aarch64-none
  * source activate code
    source env/bin/activate
  * run activate script
    zsh /Users/himansu.panigrahy/Documents/Personal_Projects/AI-Projects/AI_Trip_Planner/env/bin/activate
  * install requirements
    uv pip install -r requirements.txt
