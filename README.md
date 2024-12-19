# Blog Website


### A Backend Project of Node.JS Express.JS, Mongoose and using TypeScript
### Goal of this Project
- Create a User schema
- Make a blog  schema

**User:**
```typescript
user{
    name
    email
    isDeleted
}
```

**Blog:**
```typescript
order {
    title
    content 
    user 
}
```

### **Folder Structure**

```typescript
src
---app.ts
---service.ts
-->module
-----user
       user.interface.ts
       user.model.ts
       user.controller.ts
       user.service.ts
       user.router.ts
-----blog
       blog.interface.ts
       blog.model.ts
       blog.controller.ts
       blog.service.ts
       blog.router.ts
```

### npm run command
``` typescript
"scripts": {
    "dev": "ts-node-dev --respawn --transpile-only src/server.ts",
    "build":"tsc",
    "lint": "npx eslint --ignore-pattern '.js,.ts'",
    "lint:fix": "npx eslint . --fix",
    "format": "npx prettier --ignore-path .prettierignore --write \"**/*.{js,ts,json}\"",
    "test": "echo \"Error: no test specified\" && exit 1"
  },
```

