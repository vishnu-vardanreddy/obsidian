mysql> select* from patient;
+---------+-------+------+--------------------+
| name    | p_no  | age  | issue              |
+---------+-------+------+--------------------+
| Ramadas | 10001 |   39 | diabetes           |
| Ravi    | 10002 |   42 | Stroke             |
| Sara    | 10003 |   24 | Stroke             |
| Sneha   | 10004 |   32 | HIV/AIDS           |
| Amit    | 10005 |   32 | Alzheimers disease |
| Anjali  | 10006 |   62 | Depression         |
| Vikram  | 10007 |   12 | Astama             |
| Rahul   | 10008 |   95 | Arthritis          |
| Riya    | 10009 |   66 | Cancer             |
| Arjun   | 10010 |   52 | heart disease      |
+---------+-------+------+--------------------+

mysql> select* from doctor;
+-------------------+------+-----------------+--------+
| name              | d_no | specialist      | rating |
+-------------------+------+-----------------+--------+
| Dr. Sudhansu      |  302 | Rheumatologist  |      8 |
| Dr. Ashok         |  403 | Psychiatrist    |      9 |
| Dr. S. S. Arya    |  504 |  Neurologist    |      6 |
| Dr.RaghuRam       |  605 | geriatricia     |     10 |
| Dr.RandeepGupta   |  706 | nephrologist    |      3 |
| Dr. Naresg Trehan |  807 | immunologist    |      8 |
| Dr. Devi prasad   |  908 | cardiac surgeon |      6 |
+-------------------+------+-----------------+--------+


mysql> select * from treatment;
+------+--------------------+-----------------+
| t_id | issue              | specialist      |
+------+--------------------+-----------------+
|    1 | diabetes           | nephrologist    |
|    2 | Stroke             | Neurologist     |
|    3 | HIV/AIDS           | immunologist    |
|    4 | Alzheimers disease | Neurologist     |
|    5 | Depression         | Psychiatrist    |
|    6 | Astama             | immunologist    |
|    7 | Arthritis          | Rheumatologist  |
|    8 | Cancer             | immunologist    |
|    9 | heart disease      | cardiac surgeon |
+------+--------------------+-----------------+


SELECT d.name AS doctor_name,d.d_no, d.specialist,  t.issue,  p.name AS patient_name FROM  patient p JOIN    treatment t ON p.issue = t.issue JOIN   doctor d ON t.specialist = d.specialist;




SELECT  t.issue, d.name AS doctor_name, d.d_no,  d.rating FROM 
  treatment t JOIN doctor d ON t.specialist = d.specialist WHERE  t.issue = 'Astama';



select t.issue, d.name as doctor_name, d.d_no, d.rating 
from treatment t 
join doctor d on t.specialist= d.specialist
 where d.d_no = 807;



SELECT  d.name AS doctor_name,  d.d_no,   d.specialist,  t.issue,  p.name AS patient_name FROM  patient p JOIN   treatment t ON p.issue = t.issue JOIN  doctor d ON t.specialist = d.specialist;



CREATE TABLE table1 (
    id INT AUTO_INCREMENT PRIMARY KEY,
    column1 VARCHAR(255) NOT NULL,
    column2 INT NOT NULL
);

CREATE TABLE table2 (
    id INT AUTO_INCREMENT PRIMARY KEY,
    column1 VARCHAR(255) NOT NULL,
    column2 DATE NOT NULL
);

CREATE TABLE table3 (
    id INT AUTO_INCREMENT PRIMARY KEY,
    column1 VARCHAR(255) NOT NULL,
    column2 DECIMAL(10, 2) NOT NULL
);


select title, ratings from IMDB  where title = %2;

select * from doctor order by d_no desc limit 1;

