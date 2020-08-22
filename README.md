# TypeScript execution and REPL for Node.js
```npm install --save-dev typescript ts-node```

# Type definitions for Node.js built-in modules
```npm install --save-dev @types/node```

# Generate configuration for TypeScript compiler (tsconfig.json)
```npx tsc --init```

/* tsconfig.json */
{
  "compilerOptions": {
    // ...
    "outDir": "./dist",
    "rootDir": "./src",
    // ...
    "lib": ["ES2018"],
    "target": "ES2018",
  }
}

/* package.json */
"scripts": {
  "build": "tsc --build",
  "serve": "ts-node ./src",
  "start": "node ./dist"
}