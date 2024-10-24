# DSA-Bootcamp-Project
Real Time Messaging Queue System
Here's the updated `README.md` with the new project title:

---

Real-Time Messaging Queue System

This project simulates a real-time messaging system using a GUI built with Python's `tkinter` library. The system allows users to act as a Customer, **Restaurant**, or **Delivery Partner**, and process real-time messages about restaurant orders. Customers can create new orders or check their status, restaurants can update order preparation statuses, and delivery partners can update delivery statuses.

## Features

- **Role-Based Interaction**: 
  - **Customer**: Can create new orders or check the status of existing orders.
  - **Restaurant**: Can update the preparation status of an order.
  - **Delivery Partner**: Can update the delivery status of an order.
  
- **Message Queue**: Implements a real-time messaging queue system where messages are processed one by one.
  
- **Order Management**: 
  - Create new orders.
  - Check the status of orders, including restaurant name, delivery status, and items.
  - Sample data for restaurants and delivery partners.

- **User-Friendly GUI**: 
  - Displays messages in a chat-like interface.
  - Role selector for user type (Customer, Restaurant, Delivery Partner).
  - Text entry for sending messages, and buttons for processing and clearing messages.

## Technologies Used

- **Python**: Core programming language used for development.
- **Tkinter**: Standard Python library for creating the graphical user interface.
- **Datetime**: For adding timestamps to messages and order history.
- **JSON**: For structured storage of orders and restaurant information (used internally).

## Setup Instructions

### 1. Clone the repository:

```bash
git clone <repository-url>
cd real-time-messaging-queue-system
```

### 2. Set up a virtual environment (optional but recommended):

```bash
python -m venv venv
source venv/bin/activate   # For Linux/MacOS
venv\Scripts\activate      # For Windows
```

### 3. Install the dependencies:

Since the project uses `tkinter`, which is part of Python’s standard library, no external dependencies are required.

### 4. Run the application:

```bash
python main.py
```

This will launch the GUI, where you can start interacting as a **Customer**, **Restaurant**, or **Delivery Partner**.

## How to Use

1. Select the user role (Customer, Restaurant, Delivery Partner) from the top of the GUI.
2. Enter messages based on the role:
   - **Customer**: Type `"NEW"` to create a new order, or enter an order ID (e.g., `1001`) to check the order status.
   - **Restaurant**: Enter an order ID to mark the order as "Prepared".
   - **Delivery Partner**: Enter an order ID to mark the order as "Delivered".
3. Press **Send** to enqueue your message.
4. Press **Process Message** (or use the shortcut `Ctrl+P`) to process the next message in the queue.
5. The system will automatically provide a response based on the role and the content of the message.

## Project Structure

```plaintext
.
├── main.py                # Main entry point of the application.
├── README.md              # Project documentation.
└── requirements.txt       # List of project dependencies.
```

## Sample Data

The project comes with some pre-configured sample data:

- **Restaurants**:
  - Domino's: Menu includes Pizza, Pasta, and Garlic Bread.
  - McDonald's: Menu includes Burgers, Fries, and McFlurry.
  - Starbucks: Menu includes Coffee, Sandwiches, and Pastries.
  
- **Orders**: 
  - Sample orders with IDs `1000`, `1001`, and `1002` are pre-loaded for testing purposes.

- **Delivery Partners**: 
  - John (DP001) – Available.
  - Sarah (DP002) – Busy.

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute it as you see fit.

---

Let me know if you’d like any further changes!
