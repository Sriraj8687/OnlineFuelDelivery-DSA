# OnlineFuelDelivery-DSA
The Online Fuel Delivery Management System is a Java-based application designed to manage fuel deliveries efficiently. The system allows customers to order fuel, specify delivery locations, choose fuel types, and make payments. Drivers are assigned to handle these fuel deliveries. The system prioritizes orders based on the payment amount using advanced Data Structures and Algorithms (DSA) concepts, ensuring efficient assignment and delivery management.

The project uses HashMap for managing driver details, PriorityQueue (Heap) for prioritizing customers based on payment amount, and other core DSA techniques like iteration and polling to efficiently assign drivers and process orders.

Features:
Customer Order Management:

Customers can input their details (name, phone number, location, fuel type, payment amount).

The system stores and processes customer orders.

Driver Management:

A set of available drivers is managed in a HashMap, where each driver can be assigned to a delivery based on availability.

Order Prioritization:

Customers are queued in a PriorityQueue based on their payment amount. The customer with the highest payment gets the highest priority for delivery.

Driver Assignment:

The system assigns available drivers to the highest-priority customer orders. If no driver is available, it notifies the system.

Efficient Delivery Assignment:

The system employs PriorityQueue for efficient order sorting and HashMap for quick lookup and driver management.

DSA Concepts Used:
HashMap:

Used for storing and managing driver details. Each driver is stored with a key (driver’s name) and value (driver object).

O(1) access time for checking if a driver is available.

PriorityQueue (Heap):

Used to store customer orders. The orders are sorted based on payment amount, with the highest-paying orders given priority.

Ensures that the system processes the most lucrative orders first.

Poll (PriorityQueue Method):

Retrieves and removes the highest-priority order (customer with the highest payment).

Iteration over HashMap:

Iterates over the driver collection to find the first available driver for the customer order.

Technologies Used:
Java (Core)

Data Structures: HashMap, PriorityQueue, Comparator

Algorithms: Sorting (for PriorityQueue), Iteration

Setup Instructions:
Clone the repository:

bash
Copy
Edit
git clone https://github.com/yourusername/online-fuel-delivery-system.git
Navigate to the project directory:

bash
Copy
Edit
cd online-fuel-delivery-system
Compile and run the Java program:

bash
Copy
Edit
javac FuelDeliverySystem.java
java FuelDeliverySystem
Follow the interactive prompt to input customer orders and manage the fuel delivery process.

Usage Example:
Add multiple drivers to the system.

Input customer details like name, phone number, location, fuel type, and payment amount.

The system assigns the highest-paying orders to available drivers.

Completed deliveries are displayed.
