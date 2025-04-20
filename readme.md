# CPP Module 03

This repository contains the exercises for CPP Module 03, focusing on C++ inheritance.

## Overview

This module explores inheritance in C++, introducing the concept of base and derived classes. The exercises revolve around implementing a family of classes (ClapTrap, ScavTrap, and FragTrap) with inheritance relationships that demonstrate how derived classes can extend and override functionality from their base classes.

## Exercises

### Exercise 00: Aaaaand... OPEN!

An introduction to the ClapTrap class, the base class for the module.

#### Features:
- Implementation of a simple character class with basic attributes and methods
- Proper constructors and destructors with informative messages
- Member functions for attacking, taking damage, and repairing

#### Implementation Details:
- Private attributes for name, hit points, energy points, and attack damage
- Orthodox Canonical Form implementation
- Member functions to simulate character actions

### Exercise 01: Serena, my love!

Extends the previous exercise by creating a ScavTrap class that inherits from ClapTrap.

#### Features:
- Inherits from ClapTrap with different default attribute values
- Overrides the attack() method with a class-specific message
- Adds a special guardGate() member function unique to ScavTrap

#### Implementation Details:
- Proper constructors and destructors that call parent class methods
- Modified attribute values (higher hit points, energy points, and attack damage)
- Class-specific behavior while leveraging base class functionality

### Exercise 02: Repetitive work

Further extends the hierarchy by creating a FragTrap class that also inherits from ClapTrap.

#### Features:
- Another derived class from ClapTrap with its own default values
- Unique highFivesGuys() member function
- Different initial attribute values from both ClapTrap and ScavTrap

#### Implementation Details:
- Complete orthodox canonical form implementation
- Proper inheritance with constructor and destructor messages
- Demonstration of multiple derived classes from a single base class

## Class Hierarchy

```
           ClapTrap
           /      \
          /        \
     ScavTrap    FragTrap
```

## Compilation

Each exercise comes with a Makefile that supports the following commands:
- `make`: Compile the program
- `make clean`: Remove object files
- `make fclean`: Remove object files and executable
- `make re`: Recompile the entire program

## Requirements

- C++ compiler with C++98 standard support
- Linux/macOS environment
- All code must compile with the following flags:
```
c++ -Wall -Wextra -Werror -std=c++98
```

## Technical Details

### Class Inheritance

Inheritance in C++ allows a class (derived class) to inherit attributes and methods from another class (base class). Key concepts demonstrated in these exercises include:

- Access specifiers (public, protected, private)
- Method overriding
- Constructor/destructor calling sequence
- Protected class members
- Public inheritance

### Game Character Mechanics

The exercises simulate characters with the following properties:
- Hit points (HP): The character's health
- Energy points (EP): Resources for performing actions
- Attack damage: Amount of damage inflicted on attacks

Characters can:
1. Attack other targets (costs 1 energy point)
2. Take damage (reduces hit points)
3. Be repaired (restores hit points, costs 1 energy point)
4. Perform special actions (specific to each derived class)

## Notes

These exercises demonstrate essential C++ inheritance concepts such as:
- Class hierarchies and relationships
- Code reuse through inheritance
- Method overriding
- Specialized behavior in derived classes
- Proper constructor and destructor chaining