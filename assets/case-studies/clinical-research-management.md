# Clinical Research Management

**Domain:** Healthtech / clinical research  
**Type of work:** Maintenance, document storage and application security  
**Repository:** Private  
**Role:** Full Stack Developer

## Context

This is a large enterprise application used to support clinical-research management workflows.

The platform contains many modules related to studies, documentation, participants, operational follow-up and other research processes.

My contribution has been **targeted rather than ownership of the complete system**.

## My contribution

My work has focused on:

- diagnosing and fixing bugs in document-folder organization;
- correcting behavior in document-storage workflows;
- improving reliability around file organization;
- understanding existing modules before modifying them;
- participating in application-security improvements similar to those made in other enterprise projects.

## Document-management problem

Large document-oriented systems can fail in subtle ways when folder or storage logic becomes inconsistent.

A simplified version of the workflow is:

```mermaid
flowchart LR
    U[User uploads document] --> V[Validation]
    V --> C[Determine context]
    C --> F[Resolve folder/path]
    F --> S[Object storage]
    S --> M[(Document metadata)]
    M --> UI[Application view]
```

A bug at the folder-resolution stage can make a document difficult to locate even when the file itself was uploaded successfully.

The work therefore required understanding the relationship between:

- business entities;
- folder hierarchy;
- stored objects;
- database metadata;
- application views.

## Maintenance approach

When working on an established codebase, I prefer to:

1. reproduce the problem;
2. trace the complete flow;
3. identify whether the error belongs to data, storage, business logic or presentation;
4. make the smallest safe change;
5. validate adjacent flows to avoid regressions.

This is especially important in systems with many interconnected modules.

## Security work

I also participated in application-security improvements, including review of authentication behavior, HTTP security configuration and other hardening opportunities.

The details are intentionally generalized to avoid exposing private implementation or security information.

## Technologies

`Node.js` · `Express.js` · `MongoDB` · `Mongoose` · `EJS` · `S3-compatible storage` · `REST APIs`

## What this project demonstrates

- Debugging an unfamiliar and relatively large enterprise codebase.
- Following a document from upload through storage and metadata.
- Fixing targeted problems without rewriting unrelated modules.
- Understanding the importance of regression risk in mature applications.
- Applying security improvements to an existing system.

## Confidentiality

Study information, research participants, documents, client identity, storage configuration, infrastructure details and proprietary source code are intentionally excluded.
