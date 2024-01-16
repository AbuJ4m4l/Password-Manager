# Terminal-Based Password Manager in Rust 🔐🖥️

A Rust application that provides a terminal-based interface for managing passwords. It consists of two main files: `main.rs` and `db.rs`.

## Description 📖

This project is a terminal-based password manager that allows users to store and manage their passwords securely. The application offers various modes for interacting with the password database, such as inserting, editing, deleting, and listing passwords.

## Files Overview 📄

### 1. `main.rs`

- **Functionality**:
  - Sets up the user interface using `tui` (Text User Interface) crate.
  - Handles user input and switches between different modes (e.g., Insert, Edit, Delete, List).
  - Integrates with the clipboard for copying usernames and passwords.
  - Connects to the SQLite database through the `Database` struct defined in `db.rs`.

- **Key Components**:
  - `PassMng`: A struct that manages application state and database interaction.
  - `InputMode`: An enum representing different input modes of the application.
  - `ui`: A function that renders the user interface.
  - `run_app`: The main loop that handles user input and updates the interface accordingly.

### 2. `db.rs`

- **Functionality**:
  - Manages the SQLite database operations.
  - Provides functions for creating tables, loading, inserting, updating, and deleting password records.

- **Structs and Functions**:
  - `Database`: A struct that handles database connections and operations.
  - `new`: Function to initialize a new database connection.
  - `create_table`, `load`, `insert`, `update`, `delete`: Functions for various database operations.

## Usage 🚀

1. Run the `main.rs` file to start the application.
2. Follow the on-screen instructions to interact with the password manager.
3. Use the specified key combinations to switch between different modes and perform actions.

## Dependencies 📦

- `arboard` for clipboard interaction.
- `crossterm` for handling terminal input/output.
- `rusqlite` for SQLite database management.
- `tui` for creating terminal-based user interfaces.

## Note 🚨

- Ensure to keep your passphrase safe as it's essential for accessing your stored passwords.
- This application is a demonstration and should be used with caution in real-world scenarios.

---

Developed with ❤️ in Rust by AbuJamal! 🦀
