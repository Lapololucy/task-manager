The application will have features like adding, updating, and deleting tasks. We will use RESTful API endpoints to communicate between the backend and frontend.

###Setting up the Environment:###

To get started with building the Full-stack Task Manager App, you'll need to have Node.js and npm installed on your machine.

You can download Node.js from the official website at https://nodejs.org, and npm will be installed automatically with Node.js.

You will also need to install MongoDB. Download and install the latest version of MongoDB from the official website here. Alternatively, you can also use a cloud-based MongoDB service like MongoDB Atlas.

Install Typescript. If you don't have Typescript already install, you can run the following command to install it globally on your system.

npm install -g typescript

Initialize the project by opening the terminal and create a new directory for the project. Name it task-manager.
Navigate to the directory and run the following command to initialize the project:
npm init -y

This will create a package.json file that will store the project configuration.

###Set up TypeScript configuration:###

Create a new file in your project directory called tsconfig.json and add the following contents:
{
    "compilerOptions": {
      "target": "es6",
      "module": "commonjs",
      "outDir": "dist/js",
      "rootDir": "src",
      "strict": true,
      "esModuleInterop": true,
      "forceConsistentCasingInFileNames": true
    },
    "include": ["src/**/*"],
    "exclude": ["src/types/*.ts", "node_modules", ".vscode"]
  }

This file specifies the configuration options for the TypeScript compiler. Here, we are telling the compiler to target ES6, use CommonJS modules, output the compiled JavaScript files to a dist folder, and use the src folder as the root directory for our TypeScript files. We also set esModuleInterop to true to enable interoperability between CommonJS and ES modules.

###Installing required packages:###
Now let's install the required packages for your project using the following command:

npm install express @types/express typescript nodemon mongoose cors @types/mongoose @types/dotenv @types/cors

Here, we are installing the express package for building our Node.js server and handling HTTP requests.
We are also installing the TypeScript types for these packages using the @types prefix. We are also installing mongoose, a Object-Document Mapping (ODM) library for Node.js and MongoDB, Nodemon, helps to automatically restart our server.
