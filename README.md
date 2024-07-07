## Getting Started
- Start a virtual env

### Prequisites
- Python installed

### Cloning the Repository
Command to clone the repository:
```
git clone https://github.com/xtekky/chatgpt-clone.git
```

### Setting up a Virtual Environment

-In root directory run:
```
python -m venv venv
```
-Activate the virtual environment:
```
source venv/bin/activate
```

-For Windows:
```
venv\Scripts\activate
```
-Install the required dependencies:
```
pip install -r requirements.txt
```

### Configure the Application
 Can be set either via the environment or via config.json:

| Field               | Env Variable    | config.json     | examples                                           |
|---------------------|-----------------|-----------------|----------------------------------------------------|
| The OpenAI Api Key  | OPENAI_API_KEY  | openai_key      | sk-...                                             
| The OpenAI Base URL | OPENAI_API_BASE | openai_api_base | https://api.openai.com <br> http://my-reverse-proxy/ 

Use the Base URL if you need to run your queries through a reverse proxy (like [this one](https://github.com/stulzq/azure-openai-proxy) which will run your queries through Azure's OpenAI endpoints )


### Running the Application
To run the application, make sure the virtual environment is active and run the following command:
```
python run.py
```

### Docker
The easiest way to run ChatGPT Clone is by using docker
```
docker-compose up
```

