# SQL
SQL is a standard language for accessing and manipulating databases.

schooldb:

CREATE TABLE registration (
    student_id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    email VARCHAR(100) UNIQUE,
phone VARCHAR(100) UNIQUE,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-------------------------------------------------------------------------

CREATE TABLE payment (
    student_id INT AUTO_INCREMENT PRIMARY KEY,
    bankname VARCHAR(100) NOT NULL,
    accountname VARCHAR(100) UNIQUE,
payment_ref VARCHAR(100) UNIQUE,
date_of_payment VARCHAR(100) UNIQUE,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

----------------------------------------------------------------------------

  CREATE TABLE exam (
    student_id INT AUTO_INCREMENT PRIMARY KEY,
    exam_date VARCHAR(100) NOT NULL,
    subject VARCHAR(100) UNIQUE,
 result VARCHAR(100) UNIQUE,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP

---------------------------------------------------------------------------
----------------------------------------------------------------------------
----------------------------------------------------------------------------

HR Database:

CREATE TABLE customer (
    customer_id INT AUTO_INCREMENT PRIMARY KEY,
    customer_name VARCHAR(100) NOT NULL,
    customer_address VARCHAR(100) UNIQUE,
customer_email VARCHAR(100) UNIQUE,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-----------------------------------------------------------------------------

CREATE TABLE product (
    customer_id INT AUTO_INCREMENT PRIMARY KEY,
    product_name VARCHAR(100) NOT NULL,
    product_type VARCHAR(100) UNIQUE,
product_ref VARCHAR(100) UNIQUE,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

--------------------------------------------------------------------------------

CREATE TABLE finance (
    customer_id INT AUTO_INCREMENT PRIMARY KEY,
    payment_ref VARCHAR(100) NOT NULL,
    payment_status VARCHAR(100) UNIQUE,
amount VARCHAR(100) UNIQUE,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-----------------------------------------------------------------------------------

CREATE TABLE employee (
    staff_id INT AUTO_INCREMENT PRIMARY KEY,
    staff_name VARCHAR(100) NOT NULL,
    staff_status VARCHAR(100) UNIQUE,
staff_address VARCHAR(100) UNIQUE,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);