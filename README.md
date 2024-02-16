# Console Navigation System with User-Friendly UI

## Overview
This GitHub project implements a console navigation system with a user-friendly UI, integrating CRUD operations with SQL Server, and incorporating a game quiz system.

## Features

### 1. Console Navigation
The project includes a `StateManager` class, managing console navigation through a stack-based system. Users can switch between states, navigate backward, and forward through the console interface.

### 2. User-Friendly UI
The console interface provides a user-friendly experience, making navigation intuitive and accessible. The `_currentState.Render()` method is responsible for rendering the current state on the console.

### 3. CRUD Operations with SQL Server
It utilizes the `IState` interface to manage states and switch between different functionalities seamlessly.

### 4. Game Quiz System
In addition to console navigation and CRUD operations, the project incorporates a game quiz system. Users can engage with quiz functionalities through the console interface.

## Usage

### Setting Up
1. Clone the repository to your local machine.
2. Configure the SQL Server connection in the project settings.
3. Build and run the application.

### Console Navigation
- Use the `SwitchState`, `PastState`, and `FutureState` methods in the `StateManager` class to navigate through different states in the console.

### CRUD Operations
- Leverage the implemented CRUD operations to interact with a SQL Server database seamlessly.

### Game Quiz System
- Engage with the quiz system by following the prompts in the console interface.

## Example Usage

```csharp
using Buutyful.Coding_Tracker.State;

class Program
{
    static void Main()
    {
        // Create an instance of StateManager
        StateManager stateManager = new StateManager();

        // Set up initial state
        IState initialState = // Your initial state implementation
        stateManager.Run(initialState);
    }
}
