# Compiler-Design-DFA-Implemetation

Regular Expression to DFA Converter

This project demonstrates the conversion of a Regular Expression (RE) into a Deterministic Finite Automaton (DFA) using formal automata theory techniques. The implementation is written in C++ and follows a classic compiler-style workflow involving Thompson’s Construction and the ε-closure (subset construction) algorithm.

📌 Project Overview

The goal of this project is to:

Convert a given regular expression into an ε-NFA

Transform the ε-NFA into an equivalent DFA

Use the DFA to determine whether an input string is Accepted or Rejected

🧮 Regular Expression

The core regular expression handled by this project is:

RE=b∗a[a+ba(a+b)]∗

This expression defines the language that the DFA recognizes.

⚙️ Workflow Logic

The project follows a standard automata conversion pipeline:

1. Regular Expression → ε-NFA

Uses Thompson’s Construction

Builds a non-deterministic finite automaton with ε-transitions

2. ε-NFA → DFA

Applies the ε-closure and subset construction algorithm

Eliminates non-determinism to produce a DFA

3. C++ Implementation

The resulting DFA is either hardcoded or dynamically generated

The program evaluates input strings based on the DFA’s transition table

