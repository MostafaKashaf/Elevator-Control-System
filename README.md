# Elevator-Control-System

## 📝 Overview
### This project models a Unified Elevator System using Finite State Machines (FSMs) to simulate the behavior of multiple elevators and floors within a building. The goal is to ensure efficient, conflict-free operation of elevators in response to user requests from different floors.

## 🔑 Main Concepts
- Elevator FSMs: Each elevator transitions through states like Idle, Moving, Loading/Unloading, and Assigned based on requests, current position, and turn-taking logic.

- Floor FSMs: Each floor generates requests (Up or Down) and waits for acknowledgment from an elevator. Once the request is served, the floor resets to idle.

- Request Management: The system uses shared variables (e.g., request[], ack[], turn) to manage requests and coordinate which elevator should respond.

- Turn-Based Scheduling: A turn variable ensures fair and balanced elevator assignment, preventing both elevators from responding to the same request.

- Modular and Scalable: The system can be extended to more elevators and floors due to its modular design using FSMs.
