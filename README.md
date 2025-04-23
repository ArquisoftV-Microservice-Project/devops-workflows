# devops-workflows

This repository is used to **store generic GitHub Actions workflows** that can be reused by multiple repositories across the organization.

## General Concept

GitHub allows workflows to be **reused** across repositories through the `workflow_call` feature.  
This means that instead of duplicating workflow definitions in every repository, you can define them once in a central place and then reference them when needed.

Repositories within the organization can **invoke** these centralized workflows, passing **input parameters** to customize their behavior depending on their specific needs.

## About This Repository

The workflows stored here are designed to be **flexible** and **parameterized**.  
For instance, some workflows expect inputs such as the namespace a project belongs to, enabling the same workflow to adapt dynamically depending on where it is used.

## Benefits

- **Centralization**: All reusable workflows are maintained in a single repository, simplifying updates and governance.
- **Consistency**: Ensures all projects adhere to the same automation standards and best practices.
- **Scalability**: New repositories can easily adopt existing workflows without creating them from scratch.
- **Flexibility**: Input parameters allow workflows to adapt their behavior based on the calling repository's context.
