# JSDoc with better-docs template

Install
````bash
npm install --save-dev better-docs
````

Command line
````bash
jsdoc your-documented-file.js -t ./node_modules/better-docs
````

- [mermaid documentation](https://mermaid-js.github.io/mermaid/getting-started/theming.html)

```mermaid
sequenceDiagram
User->>CLI: Run CLI via terminal command
CLI->>User: Would you like to start: yes/no?
User-->>CLI: no
CLI-->>User: CLI exit process
User->>CLI: yes
CLI-->>FileSystem: Access Files Failure
CLI-->>User: CLI exit process
CLI-->>FileSystem: Access Files Success
loop
    FileSystem-->>FileSystem: ./package.json
end
Note right of File System: Check dependencies
loop
    FileSystem->>FileSystem: ./package.json
end
CLI-->>User: Great!
```
