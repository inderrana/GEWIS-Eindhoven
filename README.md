

Data Description:

This dataset simulates transactions and employee information for a fictional company. It includes the following tables:

**employees.csv:** Contains information about company employees.

- Employee_ID: Unique identifier for each employee.
- Employee_Name: Name of the employee.
- Role: Role of the employee in the company (Manager, Senior Manager, Employee).

**customers.csv:** Contains information about customers.

- Customer_ID: Unique identifier for each customer.
- Customer_Name: Name of the customer.
- Related_to_Management: Indicates whether the customer is related to management.

**transactions.csv:** Contains details of transactions made by employees.

- Transaction_ID: Unique identifier for each transaction.
- Employee_ID: Identifier of the employee who made the transaction.
- Transaction_Amount: Amount of the transaction.
- Discount: Discount applied to the transaction.
- Approval_Level: Level of approval required for the transaction (Manager, Senior Manager, Employee).
- Bank_Account_Change: Indicates if there was a change in the bank account.
- Order_Receiver: Identifier of the employee who received the order.
- Customer_ID: Identifier of the customer involved in the transaction.
- Order_Status: Status of the order (Ordered, Cancelled, In Progress, Hold, Invoiced, Shipped).
- Transaction_Date: Date of the transaction.
- Order_Status_Date: Date of the order status update.
- Is_Fraudulent: Indicates if the transaction is flagged as fraudulent.
