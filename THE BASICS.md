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

    show user;            
   (USER CREATED)


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


CREATE TABLE UniversityDataset1 ( 
    StdID int, 
    Credits int, 
    Course_id varchar(255), 
    Semester int,
    Faculty varchar(255),
    Dept varchar(255))

INSERT INTO UniversityDataset1 (STDID,CREDITS,COURSE_ID,SEMESTER,FACULTY,DEPT)
VALUES (20034,101,'CE258',4,'AJS','CE');

select 
    "STDID",
    "CREDITS",
    "COURSE_ID",
    "SEMESTER",
    "FACULTY",
    "DEPT"
from "UNIVERSITYDATASET1";
