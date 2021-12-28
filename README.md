# sqlcommands+ by plush
 sqlplus

## (login)

username - system
password - Oracle#143

## (creating a user)

create user c##(20ce034)
2 identified by cspit;
show user; (system)
grant resource, connect to c##(20ce034);
connect c##(20ce034)/(cspit);
show user;            (USER CREATED)

## (if above method doesnt work) {
ERROR Desc- ORACLE initialization or shutdown in progress

i) username - (system or c##(user)) as sysdba
password - (Oracle#143 or cspit)

ii) SELECT status, database_status from v$instance;
(output)
STATUS       DATABASE_STATUS
------------ -----------------
MOUNTED      ACTIVE

iii) alter database open;
         Database altered.

iv) SELCET status, database_status from v$instance;
(output)
STATUS       DATABASE_STATUS
------------ -----------------
OPEN         ACTIVE
[SOLVED]
}

## (using dual table-sudo table)

SELECT sysdate FROM dual;
(returns date)
SELECT 2*2 FROM dual;
(4) (arithmetic operation)

## (creating a table)

CREATE TABLE table_name ( 
    column1 datatype constraint(not mandatory),
    column2 datatype constraint,
);

## (insert into table(rows))

INSERT INTO table_na## me (STDID,CREDITS,COURSE_ID,SEMESTER,FACULTY,DEPT)
VALUES (20034,101,'CE258',4,'AJS','CE');

## (select/display table)


select 
    "STDID",
    "CREDITS",
    "COURSE_ID",
    "SEMESTER",
    "FACULTY",
    "DEPT"
from "TABLE_NAME";
