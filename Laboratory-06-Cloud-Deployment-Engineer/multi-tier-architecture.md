# Multi-Tier Architecture

## Two-Tier Architecture

A two-tier architecture is a system that has two main parts: the application tier and the database tier. These two parts work together so users can access an application and its stored information.

## Web/Application Tier

The web/application tier is responsible for displaying the application and handling user requests. In our project, Nextcloud serves as the application where users can access and manage their files through a web browser.

## Database Tier

The database tier stores and manages the information needed by the application. In our project, MariaDB acts as the database and stores information such as user accounts and file metadata.

## Why Separate Them

Separating the application and database into different containers makes the system easier to manage and troubleshoot. It also allows each component to be maintained or updated independently without combining everything into one container. This setup helps organize the application and makes it easier to manage its services.
