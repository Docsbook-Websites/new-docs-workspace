---
title: Getting Started with Postgres Schema Typing Tool
description: Learn to create typed clients from Postgres schemas using SchemaType. Enhance your productivity and reduce errors in your applications.
---

## What You'll Learn
In this tutorial, you will learn how to set up the Postgres Schema Typing Tool, connect it to your Postgres database, and generate typed clients that improve type safety in your applications.

## Prerequisites
- **Node.js**: Version 14.x or higher
- **Postgres**: Version 12.x or higher
- **SchemaType**: Version 1.0.0 or higher
- Basic knowledge of JavaScript and SQL

## Steps to Get Started

1. **Install SchemaType**  
   Open your terminal and run the following command to install the SchemaType package globally:
   ```bash
   npm install -g schematype
   ```

2. **Create a New Project**  
   Navigate to your desired directory and create a new project folder:
   ```bash
   mkdir my-schema-project
   cd my-schema-project
   ```

3. **Initialize Your Project**  
   Initialize a new Node.js project by running:
   ```bash
   npm init -y
   ```

4. **Set Up Your Postgres Database**  
   Ensure your Postgres database is running. Create a new database for this tutorial:
   ```sql
   CREATE DATABASE my_database;
   ```

5. **Connect SchemaType to Your Database**  
   Create a configuration file named `schema.config.js` in your project folder. Add the following code, replacing the placeholders with your actual database credentials:
   ```javascript
   module.exports = {
       database: {
           host: 'localhost',
           port: 5432,
           user: 'your_username',
           password: 'your_password',
           database: 'my_database',
       },
   };
   ```

6. **Generate Typed Clients**  
   Run the SchemaType command to generate typed clients based on your Postgres schema:
   ```bash
   schematype generate
   ```

7. **Verify Generated Clients**  
   Check the `generated` folder created in your project directory. Open the generated files to see the typed clients based on your database schema.

8. **Integrate Typed Clients into Your Application**  
   Import the generated clients into your application code. Use them to interact with your Postgres database with type safety:
   ```javascript
   const { User } = require('./generated/User');
   ```

## Next Steps
- Explore the core concepts of SchemaType in [Concepts](concepts.md).
- Get a quick overview of advanced features in [Quick Start Guide](guides/quick-start.md).