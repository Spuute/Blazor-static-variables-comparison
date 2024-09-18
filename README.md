## Blazor Static Variables Comparison

This repository illustrates the differences between **Blazor WebAssembly** (WASM) and **Blazor Server** in handling static variables. It provides two examples to demonstrate how static variables behave in each environment:

- **Blazor WebAssembly**: Each client (or tab) has its own isolated instance of static variables. Changes in one client do not affect others. This example highlights how data is isolated per user session.

- **Blazor Server**: Static variables are shared among all clients connected to the same server. Changes made by one user affect all other connected users in real time. This example shows how data can be shared across all users.

### Features

- **Blazor WebAssembly** Example: Demonstrates how static variables are handled in a client-side Blazor application, emphasizing isolation between different user sessions.
- **Blazor Server** Example: Shows how static variables are shared and synchronized across all users connected to the same server.

### Usage

1. **Run the Blazor WebAssembly project**: Open the example page in multiple tabs or browsers and observe the isolated behavior of static variables. Each time you hit the Save button, take a look in the console. 
You will see that the name change only happens in the current tab.

2. **Run the Blazor Server project**: Open the example page in multiple browsers and observe how changes to static variables are reflected across all users in real time. Each time you hit the Save button, take a look at the terminal window and you will see that every change is logged, no matter what tab you are saving from. And if you make a change in Tab A and refresh Tab B you will have the new name.

### Purpose

This repository is intended to provide a practical understanding of how static variables differ in behavior between client-side and server-side Blazor applications. 
