# Data Management System in C++

A command-line data management application built in C++ to load, organize, search, and sort structured records efficiently. This project demonstrates practical software engineering skills in file handling, input validation, and data organization using a Binary Search Tree.

## Overview

This application reads structured records from an external file, validates user input, and provides a simple interface for managing and exploring that data. It is designed to show how structured information can be stored, searched, and displayed efficiently in a modular C++ program.

## Why It Matters

Data management is about turning raw information into something usable, searchable, and reliable. This project focuses on core concepts important in real-world systems, including:

- Organizing structured records from external data sources
- Improving retrieval efficiency through deliberate data structure selection
- Enforcing data integrity with validation and error handling
- Maintaining clean and adaptable code that can scale

## Key Features

- Loads structured data from a text file
- Validates and processes user input
- Stores records in a Binary Search Tree for efficient lookup and sorted traversal
- Supports search, sort, and display operations via a command-line interface
- Demonstrates modular C++ design with separation of concerns

## Technologies Used

- C++
- Binary Search Tree (BST)
- File I/O
- Command-line interface

## Data Structure Trade-Off Analysis

The BST was selected after evaluating three candidate structures for the core operations — file ingestion, individual record lookup, and sorted output:

| Structure | Lookup | Sorted Output | Notes |
| :--- | :--- | :--- | :--- |
| Vector | O(n) | O(n²) | Simple but costly to search and sort |
| Hash Table | O(1) avg | O(n log n) | Fast lookup, but requires external sort |
| **Binary Search Tree** | **O(log n)** | **O(n)** | **Best balance for search and sorted traversal** |

The BST's in-order traversal produces a naturally sorted result in linear time, avoiding the extra sorting pass required by other structures.

## What This Project Demonstrates

- Working with structured data from flat-file sources
- Building efficient record-management logic with a purpose-fit data structure
- Parsing and validating file-based input defensively
- Writing maintainable, modular C++ with clean separation between the UI, file engine, and BST core

## Project Files

- `ProjectTwo.cpp` — main C++ application (BST implementation, file parser, and user menu)
- `CS 300 Project One.docx` — design and algorithmic analysis documentation
