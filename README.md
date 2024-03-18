<span style="color:green;">Data Description:</span>

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

<span style="color:green;">Internal Controls</span>


Segregation of Duties (SOD):
The Segregation of Duties (SOD) check ensures that critical tasks are divided among different individuals to prevent fraud and errors.

For every transaction:
- The approver cannot be the creator if there is a bank account change.
- The order receiver cannot be the creator.

Approval Matrix:

The Approval Matrix ensures that appropriate approval levels are followed based on transaction characteristics.

Approval Matrix:
- If the discount is less than 10%, no approval is required.
- If the discount is between 10% and 19%, a manager or higher approval is required.
- If the discount is 20% or more, a senior manager or higher approval is needed.

Sales Reversals :

The Sales Reversals are the transactions that may indicate potential sales reversals, where an order is created towards the end of the month and then cancelled shortly after (for example: to achieve sales targets).
