# Simple User Application Management

This is a Java-based Login Management System that allows users to perform CRUD (Create, Read, Update, Delete) operations on user data. The application uses a graphical user interface (GUI) built with Swing and stores user data in a JSON file.

## Features

- **Add User**: Add a new user with a username and password.
- **Update User**: Update the username or password of an existing user.
- **Delete User**: Remove a user from the system.
- **Welcome Screen**: A central screen to navigate between different operations.
- **JSON Storage**: User data is stored in a `user.json` file for persistence.

## Project Structure

```
Login/
├── build/
│   ├── classes/
│   └── ...
├── nbproject/
│   ├── build-impl.xml
│   ├── project.properties
│   └── ...
├── src/
│   └── Login/
│       ├── add.java
│       ├── update.java
│       ├── delete.java
│       ├── welcome.java
│       ├── user.json
│       └── ...
├── test/
├── build.xml
└── manifest.mf
```

## Prerequisites

- Java Development Kit (JDK) 8 or higher
- Apache Ant (for building the project)
- NetBeans IDE (optional, for development)

## How to Run

1. Clone the repository or download the source code.
2. Open the project in NetBeans or any Java IDE.
3. Build the project using the `build.xml` file:
   ```sh
   ant build
   ```
4. Run the application:
   ```sh
   ant run
   ```
5. The application will open a GUI window starting with the Welcome screen.

## File Descriptions

- **`src/Login/add.java`**: Handles adding new users to the system.
- **`src/Login/update.java`**: Handles updating existing user details.
- **`src/Login/delete.java`**: Handles deleting users from the system.
- **`src/Login/welcome.java`**: The main navigation screen for the application.
- **`src/Login/user.json`**: Stores user data in JSON format.

## JSON File Structure

The `user.json` file stores user data in the following format:

```json
{
  "users": [
    {
      "username": "exampleUser",
      "password": "examplePassword"
    }
  ]
}
```

## Key Classes and Methods

- **`add`**:
  - `filecheck()`: Reads and validates the `user.json` file.
  - `btnAddActionPerformed()`: Adds a new user to the system.

- **`update`**:
  - `filecheck()`: Reads and validates the `user.json` file.
  - `updateButtonActionPerformed()`: Updates user details.

- **`delete`**:
  - `filecheck()`: Reads and validates the `user.json` file.
  - `btnDeleteActionPerformed()`: Deletes a user from the system.

- **`welcome`**:
  - Navigation buttons to access Add, Update, and Delete screens.

## Customization

- Modify the `user.json` file path in the `add`, `update`, and `delete` classes if needed.
- Update GUI components using the NetBeans Form Editor.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Author

Developed by **enfaith1**.
