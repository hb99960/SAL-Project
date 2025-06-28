# Assignment S09

### Problem Statement:

You are building a simple vending machine that can be in three states: **Idle, Processing, and Dispensing**.

- The machine starts in the **Idle** state.
- When a user inserts a coin, it moves to the **Processing** state.
- When a selection is made, it moves to the **Dispensing** state.
- After dispensing, it returns to the **Idle** state.

Implement a basic **State Design Pattern** to model this vending machine behavior. Ensure that state transitions are correctly handled through a `VendingMachine` class.

### Submission Guidelines:

- Please submit your Masai Git repository link containing your code.

### Problem Statement:

Design a **Traffic Light System** using the **State Design Pattern**. The traffic light should have three states:

1. **Red** – Vehicles must stop.
2. **Yellow** – Vehicles should slow down.
3. **Green** – Vehicles can move.

The light transitions from **Red → Green → Yellow → Red** in a loop. Implement a `TrafficLight` class that handles these transitions appropriately.

### Submission Guidelines:

- Please submit your Masai Git repository link containing your code.

### Problem Statement:

Design a **Media Player** using the **State Pattern** that supports the following operations:

- **Play State**: If the player is in this state, it should allow playing media.
- **Pause State**: If paused, the player can either resume playing or be stopped.
- **Stop State**: If stopped, media can only be played again from the beginning.

Your implementation should have a `MediaPlayer` class with state transitions based on user actions (`play()`, `pause()`, `stop()`).

### Submission Guidelines:

- Please submit your Masai Git repository link containing your code.

### Problem Statement:

A bank's ATM is implemented using the **State Pattern**, but it's not functioning correctly. The ATM should have the following states:

1. **Idle** – Waiting for a user.
2. **Card Inserted** – Waiting for PIN entry.
3. **Authenticated** – Allowing cash withdrawal.
4. **Dispensing Cash** – Dispensing money.
5. **Idle (again)** – Returning to the starting state after a transaction.

However, in the given implementation:

- The ATM transitions directly from **Idle → Authenticated**, skipping the PIN verification step.
- It does not return to the **Idle** state after dispensing cash.

Your task is to **identify and fix** these issues in the provided code.

### Submission Guidelines:

- Please submit your Masai Git repository link containing the corrected code and a brief explanation of what you fixed.

### Problem Statement:

Design a **Smart Home Automation System** using the **State Design Pattern**. The system should manage a **Smart Light**that can be in different states based on user actions and external conditions:

1. **Off State** – The light is turned off.
2. **On State** – The light is turned on manually.
3. **Motion Detection State** – The light turns on automatically when motion is detected.
4. **Brightness Adjustment State** – If it’s daytime, brightness is reduced; at night, it’s increased.

Requirements:

- Implement state transitions for the light based on user input and environmental conditions.
- The system should be scalable, allowing future state additions like "Energy Saver Mode."

### Submission Guidelines:

- Please submit your Masai Git repository link containing your implementation and a short explanation of your design choices.