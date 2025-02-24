# BaseGPT

## Server

This application is a Flask-based server that uses the GPT-4 model from OpenAI to generate Base Web React code based on user input.

### Installation

You need to have Python 3.6 or higher installed to run this application.

Install the necessary dependencies:

```bash
pip install -r requirements.txt
```

### Usage

#### Server

Before running the server, set the `OPENAI_API_KEY` environment variable to your OpenAI API key. You can do this with the `export` command:

```bash
export OPENAI_API_KEY='your-api-key-here'
```

Then, you can start the server by running the `server.py` script:

```bash
python server.py
```

The server will start and listen for POST requests on `http://localhost:5000/`.

#### Client

You can make requests to the server by running the `client.py` script. The script takes a single command line argument, which is the prompt you want to pass to the GPT-4 model.

Here's an example of how to run the client script:

```bash
python client.py "Generate a simple table with some sample data with some simple formatting"
```

The script will print the response from the server, which will be the JSX code generated by the GPT-4 model.

## UI

```bash
npm install -g pnpm
pnpm install
pnpm dev
```
