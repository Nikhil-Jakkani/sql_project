# Food delivery app Customer Analysis

This project includes SQL scripts for creating tables, inserting data, and running various analytical queries on a Zomato-like database.

## Database Schema

### Tables

1. `goldusers_signup`
   - `userid` (integer)
   - `gold_signup_date` (date)

2. `users`
   - `userid` (integer)
   - `signup_date` (date)

3. `sales`
   - `userid` (integer)
   - `created_date` (date)
   - `product_id` (integer)

4. `product`
   - `product_id` (integer)
   - `product_name` (text)
   - `price` (integer)

## Data Insertion

### Gold Users Signup
```sql
DROP TABLE IF EXISTS goldusers_signup;
CREATE TABLE goldusers_signup(
  userid INTEGER,
  gold_signup_date DATE
);

INSERT INTO goldusers_signup (userid, gold_signup_date) 
VALUES 
  (1, '2017-09-22'),
  (3, '2017-04-21');
