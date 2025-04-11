# TypeScript Project Starter

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Node.js](https://img.shields.io/badge/Node.js-339933?logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![ESLint](https://img.shields.io/badge/ESLint-4B32C3?logo=eslint&logoColor=white)](https://eslint.org/)

A comprehensive, production-ready TypeScript development environment for building web servers, CLI tools, and Node.js libraries.

##### ⚠️ Please run `npm install` to ensure all required ESLint plugins and devDependencies are properly installed.

## Features

- 🚀 Modern TypeScript configuration with strict type checking

- ⚡️ Optimized ESLint setup with industry-standard rules

- 📦 Full ESM (ECMAScript Modules) support

- 🔄 Path aliases for clean imports (`@/` for src directory)

- 🔍 Comprehensive linting with specialized plugins:

- TypeScript-specific rules

- Promise handling

- Import organization

- Security best practices

- Code quality via SonarJS

## Getting Started

### Prerequisites

- Node.js 18.0 or higher

- npm or yarn

### Installation

##### Clone the repository (or use as template)

```bash
git  clone  https://github.com/yourusername/typescript-project-starter.git  my-project

cd  my-project
```

###### Install dependencies

```bash
npm  install
```

### Project Structure

```

your-project/

├── src/ # Source files

│ └── index.ts # Main entry point

├── dist/ # Compiled output (generated)

├── .eslintrc.json # ESLint configuration

├── package.json # Project metadata and scripts

├── tsconfig.json # TypeScript configuration

└── README.md # Project documentation

```

## Available Scripts

```bash

🚧 Development

npm run dev           # Run the project in development mode
npm run build:watch   # Watch for changes and rebuild

🛠️ Building

npm run build         # Build the project
npm run build:prod    # Build for production with type declarations
npm run clean         # Clean the build directory

🧹 Linting

npm run lint          # Check for linting issues
npm run lint:fix      # Fix linting issues automatically

🚀 Deployment

npm start             # Run the compiled application
npm run start:prod    # Run the app in production mode

```

## TypeScript Configuration

The project uses a carefully optimized TypeScript configuration (`tsconfig.json`) that includes:

- Target ES2022 for modern JavaScript features

- NodeNext module system for compatibility

- Strict type checking for reliable code

- Path aliases for cleaner imports

- Source maps for better debugging

- Declaration file generation for libraries

## ESLint Configuration

The ESLint configuration (`eslint.config.mjs`) is designed to enforce best practices:

- TypeScript-specific rules for type safety

- Promise handling to prevent common async/await issues

- Import sorting and organization

- Security vulnerability detection

- Code quality metrics

## Customization

### Adding Dependencies

```bash

npm  install  --save  your-dependency

```

### Modifying TypeScript Config

Edit `tsconfig.json` to adjust compiler options, include/exclude patterns, or other settings.

### Adjusting ESLint Rules

The ESLint configuration can be modified in `eslint.config.mjs`.

## Extending the Project

### For Web Servers

```bash

# Add Express.js

npm  install  express

npm  install  --save-dev  @types/express

```

### For CLI Tools

```bash

# Add Commander for CLI argument parsing

npm  install  commander

```

### For Libraries

Modify `package.json` to include:

```json

"files": ["dist"],

"publishConfig": {

"access": "public"

}

```
