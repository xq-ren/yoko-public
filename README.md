# Yoko Public (WIP)
This is the public repository for the Yoko Discord bot.

## What is Yoko?
Yoko is a Discord bot developed as a personal software engineering project.

The project focuses on automating Discord server management tasks while providing an environment for experimenting with different technologies and software development concepts.

Yoko is currently in active development, with new functionality being added over time.

## Features

### Vanity Repping

Yoko automatically manages vanity roles based on a user's Discord custom status.

When a member adds the configured server vanity to their custom status, Yoko automatically assigns the corresponding role. If the vanity is removed, the role is removed as well.

## How it works
Yoko uses Discord presence updates to detect changes to a member's custom status.

When a presence update is received:

1. Yoko retrieves the member's current activities.
2. The custom status is identified and its content is checked.
3. Yoko determines whether the configured vanity is present.
4. The vanity role is added or removed accordingly.

### Activity Diagramm


## Architecture
Yoko is built as an event-driven Java application using JDA to communicate with Discord.

Discord events are received through JDA and processed by dedicated event listeners. Business logic is separated from Discord-specific event handling where possible, allowing individual features to remain modular and easier to maintain.

### Architecture Diagramm


## Technologies
- **Java 17** — Core application development
- **JDA (Java Discord API)** — Discord API integration and event handling
- **Apache Maven** — Dependency management and build automation
- **Git / GitHub** — Version control and project documentation

Yoko is packaged as an executable JAR for deployment.

## Source Code
Yoko's source code is maintained in a private repository and is not publicly available.

This repository serves as the public documentation of the project and contains information about its features, architecture and technical implementation.

Source code access is only provided for review purposes in connection with job applications or professional inquiries.
