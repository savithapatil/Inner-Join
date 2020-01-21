# The Inner Join
- Selects records from two tables that hold **matching values**
  - Records that don’t hold matching values are excluded from the output
- The query compares each row of the first table with rows of the second table to find rows that satisfy the condition


# Example:

## Here are two tables, Orders and Customers

![Image](/orders.png)

![Image](/customers.png)


## The **SELECT** statement below shows which columns between the two tables are going to be included in the output.
```
SELECT Orders.OrderID, Customers.CustomerName, Orders.OrderDate
```

![Image](/pic1.png)

![Image](/pic2.png)


## Records from both tables that hold matching values are highlighted:
```
FROM Orders INNER JOIN Customers ON Orders.CustID=Customers.CustID;
```
![Image](/pic3.png)


## The result of the following statement...
```
SELECT Orders.OrderID, Customers.CustomerName, Orders.OrderDate 
FROM Orders INNER JOIN Customers ON Orders.CustID=Customers.CustID;
```
## ...is shown below:
![Image](/pic4.png)

