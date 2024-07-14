# Java Concurrent gRPC Script

## Motivation

My company's standard backend stack uses **Java** and **gRPC**, with nearly a thousand running services as of 2024. Over the 7 years I've been there, once or twice a year there surfaces a need for a script that makes a ton of gRPC calls. It might be data migration, incident remediation, data repair, an investigation—anything that requires _doing something_ for many entities (such as **users**). {...}

In many of these cases, writing a **data pipeline** is seen as prohibitively {...}

Concurrency is _hard_. If the intent is to mutate production data, for less experienced engineers it would be the _right_ thing to do to avoid concurrency altogether. Even for experienced engineers, it's risky to proceed without 

But it's unlikely that an engineer will be given extra days just to write a concurrent version of a script that's only going to be run once. Even if some engineer _can_ write a reusable library that makes concurrency in this context easy and safe, it's unlikely a team can afford the _weeks_ of this engineer's time it would take to build something like that correctly, especially when there might not even be a payoff until a year or so later when another script is needed.

So I built this over my nights and weekends (and that's why it's not my company's).

Since no one can justify spending days (or weeks) 

CompletableFuture

Java 21 threads

## Key

Idempotency.
