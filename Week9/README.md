# Week9 Research and Reflection Journal

## Notes:Design Patterns

### What are Design Patterns?

- They are general solutions to common programming problems
- Mainly used in object-oriented programming

### Two Main Principles

1. Program to an interface, not an implementation
2. Favor object composition over class inheritance

### Types of Design Patterns

1. Creational Patterns
   - Help create objects in a predictable way
   - Example: Singleton Pattern

2. Structural Patterns
   - Help organize classes into larger structures
   - Focus on composition

3. Behavioral Patterns
   - Help with communication between objects
   - Example: Observer Pattern

### Examples

#### Singleton Pattern

- Ensures only one instance of a class exists
- Used for shared resources (like databases)
- Makes constructor private and provides a public getInstance method
- Example: Managing a single database connection

#### Observer Pattern

- One object (subject) notifies many objects (observers) of changes
- Common in user interfaces
- Example: Like an auction where bidders (observers) watch the auctioneer (subject)

## Summary of Github Issue

- The tcconfig project is a tool that runs on Linux and simulates network impairments by wrapping Traffic Control (TC). I followed this project for years.

- The original issue: https://github.com/thombashi/tcconfig/issues/172
- The issue mentioned cannot actually be solved using tcconfig, because it cannot limit the sender's transmission rate from the receiving end.
  - For TCP protocols with congestion control, the sender can only perceive insufficient bandwidth by increasing packet loss, latency, or ECN signals. Moreover, different congestion control algorithms, such as BBR, RENO and CUBIC, have different implementations.
  - For UDP traffic, it is even more difficult to control through receiver side.
  - A feasible solution is to deploy the tcconfig tool on an intermediate node in the traffic forwarding path and control the forwarded traffic ( Need new feature support).