# Pet Name Generator App using OpenAI and Docker

This is an example pet name generator app used in the OpenAI API [quickstart tutorial](https://beta.openai.com/docs/quickstart). It uses the [Next.js](https://nextjs.org/) framework with [React](https://reactjs.org/). 

## Setup

## Prereq

- Docker Desktop 4.15


1. Clone this repository

```
git clone https://github.com/ajeetraina/openai-quickstart-node
```

2. Open app.js file and add API Keys


```
const openai = require('openai');

// Set your OpenAI API key
openai.apiKey = "YOUR_API_KEY";
```


3. Building the Chat GPT Docker Image

```
docker build -t ajeetraina/chatbot-docker .
```

4. Running the Chatbot container

```
docker run -d -p 8080:8080 ajeetraina/chatbot-docker
```

You should now be able to access the app at [http://localhost:3000](http://localhost:3000)
