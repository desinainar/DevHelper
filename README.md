## Inspiration

As developers, we all have run into errors that leave us stumped. Whether it's trying to understand legacy code without proper documentation or debugging a new feature you're implementing, the best resources for understanding and solving your problem are often online. DevHelper aims to bridge the gap between developing code and receiving online feedback, giving developers a coherent programming experience.


## Functionality

DevHelper assists programmers in each step of the development process with understanding and fixing code. When a user is facing challenges, they can simply highlight blocks of their code, and employ DevHelper to query ChatGPT or search Google for custom feedback. Users can ask to explain, debug, and/or translate their code snippets, with the results being directly displayed in VS Code. As a result, our tool helps save valuable time and allows users to seamlessly plan their next steps without breaking their workflow.


## Installation and Usage

You need to download puppeteer and chromium with the following terminal command (note: this can take some time to complete):

```
npm i --save puppeteer
```

In order to utilize the GPT API, you will also need to install the openai packages to the package.json dependencies. Run the following command on your terminal:

```
npm i openai
```

Make sure the version is 4.0.0 or greater to ensure proper functionality.

Then, in order to run the VS Code extension, click f5 to pull up a extension development host and open the file you want to use the extension on. From there, the option to use DevHelper will be visible on the top right of the screen.


## Project Layout

- OpenAI API to process user's code through LLM (ChatGPT &rarr GPT 3.5 Turbo Model)
- Puppeteer package to process user's code through search engine (Google)
- JavaScript in the backend to select highlighted code block and open pop-up window corresponding to the requested assistance
- React.js in the frontend to build out buttons embedded into VSCode and create an intuitive UI


## Technologies Used

- JavaScript
- Node.js
- React Native
- OpenAI
- Chromium
- Yeoman


## Next Steps for DevHelper

Future plans to expand upon the functionality of DevHelper:

1. Extend the DevHelper tools to work with the terminal windows opened in VS Code.
2. Incorporate voice recognition technology to provide verbal prompts related to the highlighted code snippets, which will be parsed into GPT and Google.
