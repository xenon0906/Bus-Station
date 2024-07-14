# Bus Reservation System

Welcome to the Bus Reservation System repository! This is a console-based application written in C, designed to manage bus ticket bookings, cancellations, and seat status inquiries. The system includes a secure login feature to ensure only authorized users can access the functionalities.

## Features

- **Secure Login**: Protects the system from unauthorized access.
- **View Bus List**: Displays the list of available buses.
- **Book Tickets**: Allows users to book tickets for a selected bus.
- **Cancel Booking**: Enables users to cancel an existing booking.
- **Bus Status Board**: Shows the current status of seats for a selected bus.

## Repository Structure

- `main.c`: The main source code file containing all the functions for the system.
- `tr1.txt`, `tr2.txt`, `tr3.txt`, `tr4.txt`, `tr5.txt`: Files to store seat availability for each bus.
- `status1.txt`, `status2.txt`, `status3.txt`, `status4.txt`, `status5.txt`: Files to store passenger names for each bus.
- `number1.txt`, `number2.txt`, `number3.txt`, `number4.txt`, `number5.txt`: Files to store seat numbers for each bus.

## How to Use

### Prerequisites

- A C compiler (e.g., GCC)
- A terminal or command prompt

### Getting Started

1. **Clone the Repository**:
   ```sh
   git clone https://github.com/xenon0906/Bus-Station.git
   cd bus-reservation-system
   ```

2. **Compile the Program**:
   ```sh
   gcc main.c -o bus-station
   ```

3. **Run the Program**:
   ```sh
   ./bus-station
   ```

### Usage

1. **Login**:
   - Enter the username: `sid`
   - Enter the password: `123`

2. **Navigate the Menu**:
   - **View Bus List**: Lists all available buses.
   - **Book Tickets**: Prompts to select a bus and the number of tickets, then records passenger details.
   - **Cancel Booking**: Prompts to enter bus and seat number to cancel the booking.
   - **Bus Status Board**: Displays the current status of seats for a selected bus.

## Functions Overview

### `void login()`
Manages user authentication.

### `void bus()`
Displays the list of available buses.

### `void booking()`
Handles the booking process for bus tickets.

### `void name_number(int booking, char numstr[100])`
Records passenger names and seat numbers.

### `int read_number(int trno)`
Reads seat numbers from the file for the specified bus.

### `void read_name(int trno)`
Reads passenger names from the file for the specified bus.

### `void status()`
Displays the current status of seats for a selected bus.

### `void status_1(int trno)`
Displays seat status during the booking process.

### `void cancle()`
Handles ticket cancellation and updates records accordingly.

## Notes

- Ensure the text files (`tr1.txt`, `tr2.txt`, etc.) exist in the same directory as the executable and have the correct initial values.
- The program uses `system("cls")` and `getch()` functions, which are specific to Windows. For cross-platform compatibility, these might need modification.

## Contribution

Contributions are welcome! If you have suggestions or improvements, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Enjoy using the Bus Reservation System! If you have any questions or encounter any issues, feel free to open an issue or contact me directly.

---
**Author**: Siddhanth
