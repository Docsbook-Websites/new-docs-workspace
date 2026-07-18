---
title: Postgres Schema Typing Tool Reference Guide
description: Discover commands and parameters for the Postgres Schema Typing Tool to enhance your database interactions and ensure type safety.
---

# Postgres Schema Typing Tool Reference

This reference guide provides a comprehensive overview of the commands and parameters available in the Postgres Schema Typing Tool. Use this guide to streamline your database interactions and enhance type safety in your applications.

## Commands

| Command               | Type          | Description                                         | Example                        |
|----------------------|---------------|-----------------------------------------------------|--------------------------------|
| `generate`           | Command       | Generates typed clients from the specified schema. | `schema-typing-tool generate`  |
| `validate`           | Command       | Validates the schema against the defined types.    | `schema-typing-tool validate`  |
| `migrate`            | Command       | Applies schema changes to the database.             | `schema-typing-tool migrate`   |

## Parameters

### Generate Command Parameters

| Parameter            | Type          | Description                                         | Example                        |
|----------------------|---------------|-----------------------------------------------------|--------------------------------|
| `--schema`           | String        | Specifies the Postgres schema to generate from.    | `--schema public`              |
| `--output`           | String        | Defines the output directory for generated clients.  | `--output ./src/generated`     |
| `--language`         | String        | Sets the programming language for the generated client. | `--language TypeScript`        |

### Validate Command Parameters

| Parameter            | Type          | Description                                         | Example                        |
|----------------------|---------------|-----------------------------------------------------|--------------------------------|
| `--schema`           | String        | Specifies the Postgres schema to validate.         | `--schema public`              |
| `--strict`           | Boolean       | Enables strict validation mode.                     | `--strict true`                |

### Migrate Command Parameters

| Parameter            | Type          | Description                                         | Example                        |
|----------------------|---------------|-----------------------------------------------------|--------------------------------|
| `--schema`           | String        | Specifies the schema to migrate.                    | `--schema public`              |
| `--version`          | String        | Sets the target version for the migration.          | `--version 1.0.0`              |

## Usage Tips

- Use the `generate` command to create typed clients that match your Postgres schema, enhancing type safety in your application.
- Validate your schema regularly with the `validate` command to catch errors early in the development process.
- Apply schema changes efficiently with the `migrate` command to keep your database in sync with your application.

By leveraging the Postgres Schema Typing Tool, you can streamline your development workflow, reduce errors, and ensure that your database interactions are type-safe and efficient.