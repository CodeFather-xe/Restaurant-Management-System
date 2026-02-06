# 🍔 Restaurant Management System

A desktop-based restaurant management application built with Java Swing. This system provides a user-friendly interface for both customers and administrators to manage menu items, orders, and user accounts efficiently.

## ✨ Key Features

- **🧑‍🍳 Dual User Roles:** Separate interfaces and functionalities for Administrators (Chefs) and Customers.
- **🔐 User Authentication:** Secure login and registration for both admins and customers.
- **🍽️ Menu Management (Admin):**
  - Add, edit, and remove meals from the menu.
  - Categorize meals into Appetizers, Main Meals, and Desserts.
  - Upload images for each meal item.
- **🛒 Ordering System (Customer):**
  - Browse the complete menu with meal details and images.
  - Add items to a virtual cart.
  - Place orders for delivery or internal service.
- **📈 Order Tracking:**
  - Admins can view a comprehensive list of all customer orders.
  - Customers can see a summary and bill for their own orders.
- **📝 Data Persistence:** All data, including user accounts, menu items, and orders, is saved locally using text files, acting as a simple database.
- **🎨 Custom Graphical Interface:** A unique and visually appealing UI created with custom-styled Swing components and background images.

## 📸 Screenshots

*To be added. It is recommended to add screenshots of the following frames to showcase the application's interface:*

- `MainFrame.java` (The initial welcome screen)
- `AdminLoginFrame.java` / `UserLoginFrame.java` (Login interfaces)
- `MenuFrame.java` (The customer's view of the menu)
- `EditMenuFrame.java` (The admin's menu management view)
- `BillFrame.java` (The final bill for an order)
- `ShowOrders.java` (The admin's view of current orders)

## 💻 Technologies & Libraries Used

- **Core:** Java
- **UI:** Java Swing
- **Look and Feel:** Nimbus

## 🚀 Getting Started

To run this project, you will need to have a Java Development Kit (JDK) installed on your system.

### How to Compile and Run

1.  **Clone the repository:**
    ```sh
    git clone git@github.com:CodeFather-xe/Restaurant-Management-System.git
    cd Restaurant-Management-System
    ```

2.  **Compile the source code from the root directory:**
    This command creates a new directory `out` for the compiled `.class` files.

    **On Windows:**
    ```sh
    javac -d out -cp src src\Main.java
    ```

    **On macOS/Linux:**
    ```sh
    javac -d out -cp src src/Main.java
    ```

3.  **Run the application:**
    This command executes the main class to start the application.

    **On Windows:**
    ```sh
    java -cp out Main
    ```

    **On macOS/Linux:**
    ```sh
    java -cp out Main
    ```

## 📂 Project Structure

The project is organized into several packages:

- **`src`**: The root source folder.
  - **`Main.java`**: The entry point of the application.
  - **`GUI/`**: Contains all the Java Swing frames and UI-related classes.
  - **`Logical_Class/`**: Holds the business logic classes (e.g., `AdminClass`, `CustomerClass`, `OrderClass`).
  - **`Shapes/`**: Includes custom Swing components used for styling the UI (e.g., `RoundButton`, `RoundedTextField`).
  - **`Images/`**: Contains all the visual assets like backgrounds, button icons, and meal pictures.

## 💾 Data Storage

The application uses a simple file-based system for data persistence. Data is stored in `.txt` files in the root directory of the project:

- **`Admins.txt`**: Stores administrator login credentials.
- **`Customers.txt`**: Stores customer login credentials.
- **`Appetizers.txt`**: Stores appetizer meal data.
- **`Main Meals.txt`**: Stores main course meal data.
- **`Desserts.txt`**: Stores dessert meal data.
- **`Orders.txt`**: Archives all placed orders.