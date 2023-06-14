# Introduction-to-Databases-and-Information Systems
 
# Author
**Matthias Bartolo 0436103L**

## Preview:
```sql
CREATE TABLE IF NOT EXISTS public.supplier 
( 
  supplierid integer NOT NULL, 
  phonenumber integer, 
  locality text COLLATE pg_catalog."default", 
  suppliername text COLLATE pg_catalog."default", 
  employee_id integer, 
  start_date date DEFAULT CURRENT_TIMESTAMP, 
  CONSTRAINT supplier_pkey PRIMARY KEY 
  (supplierid) 
);
```

```plpgsql
CREATE OR REPLACE FUNCTION EmployeeDept(empId int) RETURNS int AS $$
DECLARE
 deptNo int;
BEGIN
 SELECT emp.deptno INTO deptNo
 FROM scott.emp AS emp
 WHERE emp.empno = empId;
 RETURN deptNo;
END;
$$ LANGUAGE plpgsql;
```

## Description of Task:
The project aimed to provide an introductory exploration of databases and DBMSs, focusing on the utilization of specialized tools falling under the umbrella term of Database Management Systems (DBMS). The project covered various topics, including the usage of **Structured Query Language (SQL)**, logical database design techniques such as top-down and bottom-up approaches, the Relational model and languages, as well as server-side programming.

The main objective of the project was to familiarize myself with the fundamental concepts of databases and DBMSs. The project emphasized the adoption of the "database approach" during the development of database-centric applications. The principal components and architecture of a DBMS were introduced, enabling me to effectively model data requirements onto a database. The significance of data modeling, prioritizing logical and physical data independence, was highlighted.

The project incorporated the use of **ER diagrams** as a means to design databases, ensuring data normalization to validate designs against redundancy. I gained practical experience in using SQL and stored procedures for designing and querying databases. The utilization of abstract design was explored, and I was able to write queries that involved accessing the data dictionary.

<p align='center'>
  <img src="https://github.com/mbar0075/Introduction-to-Databases-and-Information-Systems/assets/103250564/01826f1c-9516-4b25-9d63-3c10e7778c9c" style="display: block; margin: 0 auto; width: 50%; height: auto;">
</p>

By the conclusion of the project, I had acquired knowledge and understanding of various aspects related to databases and DBMSs. I could describe the components of a DBMS and operate them based on their functionality and interaction with data storage. I comprehended the relative merits and capabilities associated with relational data design, along with the ability to work with relational languages in both declarative and procedural forms. I utilized structural design constructs and triggers to implement database designs, and I gained an understanding of the usage and scope of server-side programming languages. The importance of roles and other management issues associated with live databases was also appraised.

Throughout the project, I utilized the **PostgreSQL** database management system as a practical tool for implementation and experimentation. The project provided me with the opportunity to apply my acquired knowledge and skills in a real-world database environment.

<p align='center'>
  <img src="https://github.com/mbar0075/Introduction-to-Databases-and-Information-Systems/assets/103250564/e9febddd-f1de-4517-b16f-50554c63502a" style="display: block; margin: 0 auto; width: 30%; height: auto;">
</p>


## Deliverables:
The repository includes:<br />
Databases Assignment Documentation<br />
