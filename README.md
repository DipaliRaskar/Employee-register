# Employee-register
Employee register
# Employee Register

## Overview

The Employee Register is an Angular application designed to manage a list of employees. This application allows users to view, add, edit, and delete employee records. Each employee record includes a photo and various details. The application supports sorting and maintains data integrity with robust validation mechanisms.

## Features

1. **Employee Register**: View a scrollable list of employees, with the ability to sort and view employee details.
2. **Add Employee**: Form to add new employees with validation for all input fields.
3. **Edit Employee**: Form to edit existing employee details.
4. **Delete Employee**: Confirm deletion of an employee with a pop-up dialog.

## Screens

### Screen 1: Employee Register

- **Layout**:
  - Displays employees in a grid with three employees per row, centered on the screen.
  - Each employee entry includes a photo, full name, and date of joining.
  - Employee images preserve their aspect ratio and avoid distortion.
- **Sorting**:
  - Drop-down menu at the top allows sorting by Name, Date of Joining (DoJ), or Date of Birth (DoB).
- **Navigation**:
  - Clicking on an employee's entry navigates to the edit screen for that employee.
  - A blue circle with a white plus sign at the bottom right indicates the option to add a new employee.

### Screen 2: Add Employee

- **Form Fields**:
  1. **Full Name**: Capitalized before storage/display.
  2. **Nickname**: One-word nickname.
  3. **Date of Joining**: Must be within the 21st century and not in the future.
  4. **Date of Birth**: Must be within the last 100 years; accepts various formats.
  5. **Designation**: Text field for the employee’s designation.
  6. **Current Salary**: Floating point value, greater than zero.
  7. **Photo**: JPEG file, 200x200 to 1000x1000 pixels, max 2 MB, unique.
  8. **Personal Email Address**: Valid email format.
  9. **Mobile Number**: Validated using Google’s libphonenumber.
  10. **Year of Graduation**: Four-digit integer not more than 80 years old.
- **Validation**:
  - Detailed validation for all fields, including meaningful error messages.
- **Buttons**:
  - **Discard**: Returns to the employee list without saving changes.
  - **Add**: Saves the new employee and returns to the employee list with updated records.

### Screen 3: Edit Employee

- **Form**:
  - Same as the "Add Employee" screen, with pre-filled values for editing.
- **Buttons**:
  - **Revert**: Discards changes and returns to the employee list.
  - **Save**: Saves the changes and returns to the employee list.
  - **Delete** (Red Button): Deletes the employee record and returns to the employee list.

### Screen 4: Delete Employee

- **Pop-Up Dialog**:
  - Displays details of the employee to be deleted.
  - **Cancel**: Returns to the edit screen without deleting.
  - **Delete**: Deletes the employee record and returns to the employee list.

## Installation

To set up the project locally, follow these steps:

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/yourusername/employee-register.git
    ```

2. **Navigate to Project Directory**:
    ```bash
    cd employee-register
    ```

3. **Install Dependencies**:
    ```bash
    npm install
    ```

4. **Run the Application**:
    ```bash
    ng serve
    ```

5. **Open in Browser**:
    Navigate to `http://localhost:4200` to view the application.

## Usage

- **Navigate through screens** using the UI elements.
- **Add, edit, and delete employee records** as described above.
- **Sorting options** can be used to rearrange the employee list.

## Contributing

Feel free to submit issues and pull requests. For major changes, please open an issue first to discuss the changes you propose.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Angular framework
- Google libphonenumber for mobile number validation

