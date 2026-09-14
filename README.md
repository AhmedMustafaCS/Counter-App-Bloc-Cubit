# Counter App - BLoC Architecture Implementation 🚀

A foundational Flutter project demonstrating the core concepts of state management using the `flutter_bloc` library. This project serves as a practical implementation of separating business logic from the UI.

## 🧠 Core Concepts Explored

This project moves beyond a simple counter by rigorously applying BLoC architectural rules and optimizing widget rebuilds:

* **Cubit (`CounterCubit`):** Encapsulating state logic and utilizing "Early Return" principles to prevent redundant state emissions (e.g., stopping state emissions when the counter hits zero during decrement).
* **`BlocProvider`:** Handling dependency injection to make the Cubit accessible throughout the widget tree.
* **`BlocBuilder`:** Rebuilding specific UI components reactively based on state changes.
* **`BlocListener`:** Handling side effects (like triggering SnackBars) independently without causing UI rebuilds.
* **`BlocConsumer`:** Merging the responsibilities of Builder and Listener to streamline the widget tree and prevent nesting hell.
* **`listenWhen` / `buildWhen`:** Implementing conditional execution to optimize performance and filter out unnecessary state updates.

## 🛠️ Tech Stack & Tools

* **Framework:** Flutter
* **State Management:** `flutter_bloc` (Cubit)
* **Language:** Dart
* **Version Control:** Git & GitHub (Using Conventional Commits standard)

## 📈 Git History & Architecture

The commit history of this repository follows the **Conventional Commits** specification (`feat:`, `fix:`, `refactor:`, `chore:`) to ensure a clean, readable, and professional development lifecycle. 

State management transitions were implemented iteratively, starting from basic Builders to advanced Consumers, ensuring zero redundant UI rebuilds and preventing logic bugs directly at the Cubit level.

## 🚀 Getting Started

To run this project locally:

1. Clone the repository:
   ```bash
   git clone [https://github.com/AhmedMustafaCS/Counter-App-Bloc-Cubit.git](https://github.com/AhmedMustafaCS/Counter-App-Bloc-Cubit.git)
