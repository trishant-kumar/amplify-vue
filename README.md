# Vue 3 + TypeScript + Vite + Amplify Boilerplate

This boilerplate is starting point of any project that uses Amplify and Vite with all batteries included. you can directly start development without spending time on project setup, you just have to configure amplify according to you requirements.

The stack of this boilerplate is focused on web app front end, therefore I’ll keep it simple and mainly focuses on following technologies - Vue 3, Amplify, Vite

# Things to update before start

- update readme file to remove/add project related documenation.
- update `name` key in `package.json` file
- update git remote using `git remote set-url origin new.git.url/here` command
- [Demo](https://dev.d4mpru5o2tc5l.amplifyapp.com/) section from this file
- remove unnecessary files.


## Recommended IDE Setup

- [VS Code](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur) + [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin).

## Tech Stack

**Client:** [Vue3](https://vuejs.org/), [Typescript](https://www.typescriptlang.org/), [Vite](https://vitejs.dev/),
[Amplify](https://docs.amplify.aws/start/q/integration/vue/)

**Code Formatter** [Eslint](https://eslint.org/)

## Type Support For `.vue` Imports in TS

TypeScript cannot handle type information for `.vue` imports by default, so we replace the `tsc` CLI with `vue-tsc` for type checking. In editors, we need [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin) to make the TypeScript language service aware of `.vue` types.

If the standalone TypeScript plugin doesn't feel fast enough to you, Volar has also implemented a [Take Over Mode](https://github.com/johnsoncodehk/volar/discussions/471#discussioncomment-1361669) that is more performant. You can enable it by the following steps:

1. Disable the built-in TypeScript Extension
   1. Run `Extensions: Show Built-in Extensions` from VSCode's command palette
   2. Find `TypeScript and JavaScript Language Features`, right click and select `Disable (Workspace)`
2. Reload the VSCode window by running `Developer: Reload Window` from the command palette.

### Project Setup

`Clone URL : https://github.com/vue-simform/amplify-vue.git`

Clone repo using HTTP or SSH method.

To use SSH method, please [Follow this tutorial](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)

To use HTTP method, developer has to pass username in git clone url like this `https://{username}@github.com:vue-simform/amplify-vue.git`
It will promte for application password that you can generate from [here](https://github.com/settings/tokens)

run `npm i` command

copy `.env.example` to `.env`. update `.env` file variables. make sure in this process you don't rename/delete `.env.example` file.

run `npm run dev` command to start development server.

## Setup Amplify with Vue
Before starting with ampify you need to setup a aws account, after follow these steps:

1. Create a new Vue 3 project:
   
   **vue create amplifyUI-vue**

2. Install Amplify CLI:
   
   **npm install -g @aws-amplify/cli**

3. Initialize Amplify in your Vue project:
   
   **amplify init**

4. Add authentication to your Amplify project:
   
   **amplify add auth**

5. Push the Amplify project changes:
   
   **amplify push**

6. Integrate Amplify in your Vue app:
   
   **npm install aws-amplify @aws-amplify/ui-vue**

7. Last, add changes in your main file and add authenticator in you component [https://ui.docs.amplify.aws/vue/connected-components/authenticator](https://ui.docs.amplify.aws/vue/connected-components/authenticator)

## Customize configuration

See [Vite Configuration Reference](https://vitejs.dev/config/).

## Author
Trishant Kumar (trishant.k@simformsolutions.com)
