# Multi-Tier Architecture Analysis

## 1. The Web/Application Tier
The *Web/Application Tier* serves as the user-facing interface of the application architecture. In this deployment, the Nextcloud container operates at this layer to handle incoming HTTP requests from users via web browsers on port 8080. Its primary roles include processing user actions, serving static web assets, rendering the user interface, managing active sessions, and sending business logic requests to the backend database tier.

## 2. The Database Tier
The *Database Tier* forms the backend persistence storage layer of the architecture. Operating with the MariaDB database container, this tier stores critical relational data, including user account credentials, system configurations, file metadata, permissions, and sharing history. It isolates data handling from presentation logic, executing SQL queries safely and ensuring data persistence.

## 3. Why Separate Them?
Separating the web application and database into independent containers provides modular scalability, enhanced security, and isolated maintenance. By decoupling these components, the application tier can be scaled independently during high request traffic without replicating backend storage or state. Additionally, security is improved by preventing direct public exposure of the database layer, while system failures or updates in one container do not corrupt or take down the entire application stack.
