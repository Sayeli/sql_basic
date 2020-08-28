# sql_basic
Basics of sql learned
-- Data Types 
-- NUmeric 1,2,3
-- int (1,2,3,4,5)
-- float (12.34)


-- Characters Vardaan123  
-- char 2bhk 3 10x 
-- varchar 5bhk 10 - 4

----------------------------
-- Step 1: Creating a Table 
-- Step 2: Inserting Values 
-- Step 3: Extracting or Analysing 


------------------------------ 
-- CREATE TABLE <TABLE NAME> (NAME DATA TYPE,NAME DATA TYPE,NAME DATA TYPE);
--CREATE table customers (name VARCHAR, SURNAME VARCHAR, AGE INT);

------------------------------
-- INSERT INTO <TABLE NAME> VALUES(VALUE, VALUE, VALUE);
--insert into CUSTOMERS VALUES ('Vardaan', "Sharma", 30);
--insert into CUSTOMERS VALUES ('Neeru', "Sharma", 50); 
--insert into CUSTOMERS VALUES ('Farhan', "Mohd", 26);
--insert into CUSTOMERS VALUES ('Simran', "Singh", 35);  
--insert into CUSTOMERS VALUES ('Ayush', "Jain", 40); 
--insert into CUSTOMERS VALUES ('Sambhav', "Singla", 19); 

------------------------------- 
-- Queries 

-- SELECT <WHAT> FROM <TABLENAME>; 
-- SELECT * from CUSTOMERS;
--SELECT NAME, age from CUSTOMERS;
-- = > < <= >= 
-- 10 = 11 // false 
-- 10 > 9 // true 
-- 9 > 10 //false 
-- SELECT * from CUSTOMERS where age >= 30;

/*
CREATE TABLE  AGENTS (	
   "AGENT_CODE" VARCHAR NOT NULL PRIMARY KEY,
	AGENT_NAME VARCHAR, 
	"WORKING_AREA" VARCHAR, 
	"COMMISSION" FLOAT, 
	"PHONE_NO" VARCHAR, 
	"COUNTRY" VARCHAR 
	 );
*/
--INSERT INTO AGENTS VALUES ('', 'Ramasundar', 'Bangalore', '0.15', '077-25814763', 'India'); 
--INSERT INTO AGENTS VALUES ('A003', 'Alex ', 'London', '0.13', '075-12458969', 'UK');
--INSERT INTO AGENTS VALUES ('A008', 'Alford', 'New York', '0.12', '044-25874365', 'USA');
--INSERT INTO AGENTS VALUES ('A011', 'Ravi Kumar', 'Bangalore', '0.15', '077-45625874', 'India');
--INSERT INTO AGENTS VALUES ('A004', 'Ramasundar', 'Bangalore', '0.15', '077-25814763', 'Sri Lanka'); 

---------------------------------------- 
-- SELECT * from AGENTS;
--SELECT * from agents where country = "India";
--SELECT * from agents where agent_name =  "Ramasundar";
-- AND OR 

--SELECT * from AGENTS where agent_name = "Ramasundar" AND country = "India";
--SELECT * from AGENTS where agent_name = "Ramasundar" OR agent_name = "Alex ";

-- SELECT * from AGENTS ORDER BY agent_code DESC;


--UPDATE AGENTS SET agent_code = "A006" where agent_code = "";
--DELETE from AGENTS where agent_code = "A006";
-- SELECT * from AGENTS;

-- SELECT COUNT(agent_code) from AGENTS;
--SELECT * from AGENTS;


--SELECT * from AGENTS where agent_name LIKE "Ra%";
--SELECT * from AGENTS where agent_name LIKE "%ar";
-- SELECT * from AGENTS where working_area LIKE "%or%";
