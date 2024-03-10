# Starter Node.js & TypeScript Setup

## Introduction to Node.js and TypeScript

- **Node.js** allows you to write server-side JavaScript.
- As codebases grow, managing JavaScript can become challenging due to its dynamic and weak typing.
- **TypeScript**, a typed super-set of JavaScript, bridges this gap by providing strong static typing, compilation, and object-oriented features.

## Prerequisites

- Ensure you have **Node.js** installed on your system.
- If not, follow the instructions in the [How to Install Node.js and Create a Local Development Environment](https://www.digitalocean.com/community/tutorials/setting-up-a-node-project-with-typescript) guide.

## Initializing the Project

1. Create a new folder (e.g., `node_project`).
2. Navigate into the folder and initialize it as an npm project using `npm init -y`.

## Configuring TypeScript

1. Install TypeScript as a development dependency: `npm install --save-dev typescript`.
2. Create a `tsconfig.json` file in the project root with the following content:

```json
{
    "compilerOptions": {
        "module": "NodeNext",
        "moduleResolution": "NodeNext",
        "target": "ES2020",
        "sourceMap": true,
        "outDir": "dist",
        },
        "include": ["src/**/*"],
}
```

- Explanation:
  - `module`: Specifies the module code generation method (Node uses commonjs).
  - `target`: Specifies the output language level.
  - `moduleResolution`: Helps the compiler resolve imports.
  - `outDir`: Defines the output directory for transpiled JavaScript files.

## Building Your Express Application

- Create an Express application using TypeScript.
- Transpile your TypeScript code to JavaScript using the TypeScript compiler.
