---
title: How to Generate Typed Clients from Postgres Schemas
description: Generate typed clients directly from Postgres schemas using SchemaType to enhance productivity and reduce errors in your applications.
---

# How to Generate Typed Clients from Postgres Schemas

Follow these steps to create typed clients from your Postgres schemas using the SchemaType tool. This process enhances your development workflow and ensures type safety in your applications.

## Prerequisites

1. **Install Node.js**: Ensure you have Node.js installed on your machine. You can download it from [nodejs.org](https://nodejs.org/).
2. **Postgres Database**: Have access to a Postgres database with the schemas you want to use.
3. **SchemaType Account**: Sign up for an account at [SchemaType.com](https://schematype.com/) if you haven't already.

## Steps to Generate Typed Clients

1. **Install SchemaType CLI**  
   Open your terminal and run the following command to install the SchemaType CLI globally:
   ```bash
   npm install -g schematype-cli
   ```

2. **Authenticate with Your SchemaType Account**  
   Log in to your SchemaType account using the CLI. Run:
   ```bash
   schematype login
   ```
   Follow the prompts to enter your credentials.

3. **Connect to Your Postgres Database**  
   Create a configuration file named `schematype.config.js` in your project directory. Use the following template to connect to your Postgres database:
   ```javascript
   module.exports = {
     database: {
       type: 'postgres',
       host: 'your-database-host',
       port: 5432,
       username: 'your-username',
       password: 'your-password',
       database: 'your-database-name',
     },
   };
   ```
   Replace the placeholders with your actual database connection details.

4. **Generate Typed Clients**  
   Run the following command to generate typed clients from your Postgres schemas:
   ```bash
   schematype generate
   ```
   This command reads your database schema and creates TypeScript clients that reflect your data structure.

5. **Review Generated Clients**  
   Navigate to the `src/generated` directory in your project. Open the generated files to review the typed clients. Each table in your Postgres schema corresponds to a TypeScript class, complete with type definitions.

6. **Integrate Clients into Your Application**  
   Import the generated clients into your application code. For example:
   ```typescript
   import { UserClient } from './src/generated/UserClient';

   const userClient = new UserClient();
   const users = await userClient.findAll();
   console.log(users);
   ```

7. **Test Your Implementation**  
   Run your application and test the integration of the typed clients. Ensure that type safety is enforced and that you can interact with your Postgres database without errors.

## Conclusion

You have successfully generated typed clients from your Postgres schemas using SchemaType. This process improves your productivity and reduces the likelihood of errors in your database interactions.

## Related

- [SchemaType Features](https://schematype.com/features)
- [Getting Started with SchemaType](https://schematype.com/getting-started)
- [Comparing SchemaType with Prisma and TypeORM](https://schematype.com/comparison)