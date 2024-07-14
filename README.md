# Java Concurrent gRPC Script

## Motivation

My company's standard backend stack uses **Java** and **gRPC**, with nearly a thousand running services as of July 2024. Over the 7 years I've been there, once or twice a year there surfaces a need for a script that makes many gRPC calls. It might be data migration, incident remediation, data repair, an investigation—anything that requires _doing something_ for many entities (such as **users**).
