# 📝 SQL Data Insertion – Relational Model

This README provides the SQL `INSERT` statements to populate the relational model shown in the diagram:

- 🔗 Relational Model: [View Diagram](https://i.imgur.com/q25t2MI.png)
- 📋 Data to Insert: [View Data](https://i.imgur.com/DcLUzM5.png)

---

## 📥 Insert Statements

### ✅ `CUSTOMERS` Table

```sql
INSERT INTO Customers (CustCode, CustName, CustAddress, CustTel)
VALUES ('C01', 'Ali', 'Sfax', '74430000');

INSERT INTO Customers (CustCode, CustName, CustAddress, CustTel)
VALUES ('C02', 'Sana', 'Tunis', '75200000');
```

---

### ✅ `PRODUCTS` Table

```sql
INSERT INTO Products (ProductCode, ProductName, Price)
VALUES ('P01', 'Mouse', 50);

INSERT INTO Products (ProductCode, ProductName, Price)
VALUES ('P02', 'Keyboard', 70);
```

---

### ✅ `ORDERS` Table

```sql
INSERT INTO Orders (OrderCode, OrderDate, CustCode)
VALUES (101, TO_DATE('12/02/2021', 'DD/MM/YYYY'), 'C01');

INSERT INTO Orders (OrderCode, OrderDate, CustCode)
VALUES (102, TO_DATE('14/02/2021', 'DD/MM/YYYY'), 'C02');
```

---

### ✅ `ORDER_LINES` Table

```sql
INSERT INTO Order_Lines (OrderCode, ProductCode, Quantity)
VALUES (101, 'P01', 2);

INSERT INTO Order_Lines (OrderCode, ProductCode, Quantity)
VALUES (101, 'P02', 1);

INSERT INTO Order_Lines (OrderCode, ProductCode, Quantity)
VALUES (102, 'P01', 1);
```

---
