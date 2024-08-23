Pet Simulation Program

Overview

The Pet Simulation Program is a simple console-based application that simulates the basic activities of a pet, such as feeding, playing, and resting. The user can interact with the pet by performing these activities, monitoring the pet's status (hunger, happiness, energy, and age), and saving progress to continue in future sessions.

Features

Create a Pet: Users can create a new pet by providing a name. The pet's initial attributes (hunger, happiness, energy, and age) are randomly generated.

Load Existing Pet: If a pet with the same name already exists, users can choose to continue with the existing pet or create a new one.

Interactive Operations: Users can:

Feed the pet.

Play with the pet.

Let the pet rest.

Query the pet's current status.

Save Progress: Users can save the current state of the pet to a file, allowing them to resume the simulation later.

Multiple Pets: The program supports managing multiple pets in one session.

How to Run the Program

Compile the Program:

Use a C++ compiler to compile the program. For example, using g++:

bash

g++ -o pet_simulation pet_simulation.cpp

Run the Program:

Run the compiled executable:

bash

./pet_simulation

Interact with the Program:

Follow the on-screen prompts to create a pet, interact with it, and manage its attributes.

Program Structure

Class pet: Represents the pet, encapsulating its attributes (name, hunger, happiness, energy, age) and methods for interacting with the pet.

feed(): Feeds the pet, affecting its hunger, happiness, and energy levels.

play(): Plays with the pet, affecting its hunger, happiness, and energy levels.

rest(): Lets the pet rest, affecting its happiness, energy, and age.

query(): Displays the current status of the pet.

save(): Saves the current state of the pet to a file.

Function operations(pet& m): Manages the user's interactions with the pet through a menu-driven interface, allowing them to choose various operations.

Main Function:

Handles the creation or loading of pets and allows users to manage multiple pets in one session.

Input/Output

Input:

Pet name (alphabetical characters only).

Choices for operations (feed, play, rest, query).

Option to save progress or not.

Option to manage another pet or exit the simulation.

Output:

Updates on the pet's activities and current status.

Confirmation messages for saved progress.

Important Notes

Randomness: The initial attributes of the pet (hunger, happiness, energy) are randomly generated within a range.

Validation: The program includes basic input validation to ensure correct data entry (e.g., pet names must contain only alphabetical characters).

File Handling: Pet states are saved to and loaded from text files, named after the pet (e.g., petname.txt).

Dependencies

C++ Standard Library: The program uses standard libraries like <iostream>, <cstdlib>, <fstream>, <string>, and <algorithm>.

Future Improvements

Implement a graphical user interface (GUI) for a more user-friendly experience.

Add more activities and attributes to make the simulation more dynamic.

Introduce different pet types with unique characteristics.
