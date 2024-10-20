# Rule Engine with Abstract Syntax Tree (AST)
This project implements a simple 3-tier rule engine application that dynamically determines user eligibility based on multiple attributes (such as age, department, income, and spend). The system utilizes an Abstract Syntax Tree (AST) to represent conditional rules, allowing for easy creation, combination, and modification of these rules.

The architecture follows a basic three-tier approach:

**UI:** Simple interface for interacting with the rule engine.
**API:** Core logic for rule creation, combination, and evaluation.
**Backend**: Handles rule storage and management using a database.

# Key Features
Create complex eligibility rules dynamically using an AST representation.
modify existing rules efficiently.
Evaluate user attributes against the combined rules to determine eligibility.
Error handling for invalid rule syntax and user-defined attributes.
Extendable to support custom functions in rules.

# Data Structure
The core data structure used for the AST is a Node with the following attributes:

**type:** A string indicating the type of the node (e.g., "operator" for logical operations like AND/OR, or "operand" for conditions).
**left:** Reference to the left child node (used for logical operations).
**right:** Reference to the right child node (used for logical operations).
**value:** Optional value for operand nodes (e.g., a number or a string for comparisons).
