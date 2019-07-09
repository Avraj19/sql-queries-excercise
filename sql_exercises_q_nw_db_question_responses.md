# SQL Queering Homework :taco:

**Note to student**
Hey there :) if you found this, well done. You should use it to check your answer. If you just use it to copy that is fine.. but you are really cheating yourself :(  Not good. Do your best! I'm here to help you achieve more! :happy:
**End of note to student**

Use your sequel sever to run the queries and come to an answer.
Pay attention to detail, as there is ONE right answer and following guidelines & or instructions is an important skill for consultants.

Note we will refer to Northwind Database as NWDB
Please read on.

**Important**
Your response should always be the **SQL query** + the short answer where appropriate.

## Queries

### Q1 - How many orders in NWDB?
```
  SELECT COUNT(*) from orders
```

### Q2 - How many order that the Ship City is Rio de Janeiro?
```
  SELECT COUNT(*) from orders WHERE ShipCity = 'Rio de Janeiro'
```

### Q3 - Select all orders that the Ship City is Rio de Janeiro or Reims?

```
  SELECT * from orders WHERE ShipCity = 'Rio de Janeiro' OR ShipCity = 'Reims'
```


### Q4 - Select all of the entries where the Company name has a z or a Z in the table of Customers
```
	SELECT * from Customers Where CompanyName LIKE '%z%'
```

### Q5 - We need to update all of our FAX information! This Day and age it is a must! :) Find me the Name of All of the companies that we do not have their FAX numbers! I would also like to know with whom I need to speak with, their contact numbers and what city they are base in.
```
	SELECT CompanyName, ContactName, City, Phone from Customers WHERE Fax IS NULL;
```

### Q6 - Ahh there you are! My prize SPARTANTS! MY MARES AND MY STALLIONS! We need to re-target all of our Customers is Paris! Get me information on these clients.


### Q7 - WAIT! Where are you going? (...) These clients are hard to sell too! We need more intel.. Can you find out, from these clients from France, whom orders the most by quantity? Who are our top 5 clients?  
