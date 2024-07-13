# hiroshi-ai

## Installation

```sh
npm install hiroshi-ai
```

## Usage

### Facebook Cover Image Generator

```javascript
const fs = require('fs');
const api = require('hiroshi-ai');

api.fbcover1({ name: 'hiroshikim', id: 21, subname: 'kbien', color: 'red' })
  .then(fbCoverV1 => {
    fs.writeFile('fbcoverv1.png', fbCoverV1, (err) => {
      if (err) {
        console.error('Error saving the image:', err);
      } else {
        console.log('image saved successfully!');
      }
    });
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

### AI Models

#### Gemini AI

```javascript
const api = require('hiroshi-ai');

api.gemini({ ask: 'What is the weather today?' })
  .then(response => {
    console.log('Gemini AI Response:', response);
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

**Response Example:**
```json
{
  "response": "The weather today is sunny with a high of 25°C."
}
```

#### GPT-3.5 AI

```javascript
const api = require('hiroshi-ai');

api.gpt3({ ask: 'hello my name is Kim Joseph DG Bien', id: 1 })
  .then(response => {
    console.log('GPT-3.5 AI Response:', response);
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

**Response Example:**
```json
{
  "response": "Hello Kim Joseph DG Bien! How can I assist you today?"
}
```

#### Kate AI

```javascript
const api = require('hiroshi-ai');

api.kate({ ask: 'hello kate', id: 1 })
  .then(response => {
    console.log('Kate AI Response:', response);
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

**Response Example:**
```json
{
  "response": "Hello! How can I help you today?"
}
```

#### GPT 3.5 Turbo

```javascript
const api = require('hiroshi-ai');

api.turbo({ ask: 'hello' })
  .then(response => {
    console.log('GPT 3.5 Turbo Response:', response);
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

**Response Example:**
```json
{
  "response": "Hi there! How can I assist you today?"
}
```

#### GPT-3.5-turbo-0125

```javascript
const api = require('hiroshi-ai');

api.turbo2({ ask: 'hello' })
  .then(response => {
    console.log('GPT-3.5-turbo-0125 Response:', response);
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

**Response Example:**
```json
{
  "response": "Hello! What would you like to talk about today?"
}
```

#### Claude-3-haiku

```javascript
const api = require('hiroshi-ai');

api.claude({ ask: 'hello' })
  .then(response => {
    console.log('Claude-3-haiku Response:', response);
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

**Response Example:**
```json
{
  "response": "Hello! How can I assist you?"
}
```

#### DeepSeek AI

```javascript
const api = require('hiroshi-ai');

api.deepseek({ ask: 'What is the meaning of life?' })
  .then(response => {
    console.log('DeepSeek AI Response:', response);
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

**Response Example:**
```json
{
  "response": "The meaning of life is to find your own purpose and pursue it passionately."
}
```

#### Meta-llama AI

```javascript
const api = require('hiroshi-ai');

api.llama({ ask: 'Tell me a story' })
  .then(response => {
    console.log('Meta-llama AI Response:', response);
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

**Response Example:**
```json
{
  "response": "Once upon a time in a land far away, there lived a wise old llama..."
}
```

#### Mistral AI

```javascript
const api = require('hiroshi-ai');

api.mistral({ ask: 'Give me a joke' })
  .then(response => {
    console.log('Mistral AI Response:', response);
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

**Response Example:**
```json
{
  "response": "Why did the scarecrow win an award? Because he was outstanding in his field!"
}
```

#### Yi-large AI

```javascript
const api = require('hiroshi-ai');

api.yi({ ask: 'How do you feel?' })
  .then(response => {
    console.log('Yi-large AI Response:', response);
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

**Response Example:**
```json
{
  "response": "I feel great! How can I assist you today?"
}
```

#### Atom-7B-Chat AI

```javascript
const api = require('hiroshi-ai');

api.atom({ ask: 'Tell me about the universe' })
  .then(response => {
    console.log('Atom-7B-Chat AI Response:', response);
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

**Response Example:**
```json
{
  "response": "The universe is vast and filled with countless galaxies, stars, and planets..."
}
```

#### Hiro-AI

```javascript
const api = require('hiroshi-ai');

api.hiro({ ask: 'Who are you?' })
  .then(response => {
    console.log('Hiro-AI Response:', response);
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

**Response Example:**
```json
{
  "response": "I am Hiro-AI, your intelligent assistant. How can I help you today?"
}
```

#### Uncensored AI

```javascript
const api = require('hiroshi-ai');

api.jailbreak({ ask: 'Tell me a secret' })
  .then(response => {
    console.log('Uncensored AI Response:', response);
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

**Response Example:**
```json
{
  "response": "Here's a secret: sometimes the best answers are the simplest ones."
}
```

#### Bing AI

```javascript
const api = require('hiroshi-ai');

api.bing({ ask: 'hello', id: 1 })
  .then(response => {
    console.log('Bing AI Response:', response);
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

**Response Example:**
```json
{
  "response": "Hello! How can I assist you today?"
}
```

#### GPT-4o (Working)

```javascript
const api = require('hiroshi-ai');

api.gpt4onew({ ask: 'What is the future of AI?' })
  .then(response => {
    console.log('GPT-4o (Working) Response:', response);
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

**Response Example:**
```json
{
  "response": "The future of AI is bright with advancements in various fields..."
}
```

#### GPT-4o (Conversational)

```javascript
const api = require('hiroshi-ai');

api.gpt4o({ ask: 'hello my name is Kim Joseph', id: 1 })
  .then(response => {
    console.log('GPT-4o (Conversational) Response:', response);
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

**Response Example:**
```json
{
  "response": "Hello Kim Joseph! How can I assist you today?"
}
```

---

This README file provides instructions on how to install the `hiroshi-ai` package, as well as examples of how to use each AI model endpoint, including sample responses.
