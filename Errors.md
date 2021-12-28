## ERROR 

# #1 ORACLE initialization or shutdown in progress 

i)                                  

         username - (system or c##(user)) as sysdba
         password - (Oracle#143 or cspit)

ii) 

         SELECT status, database_status from v$instance;

(output)

         STATUS       DATABASE_STATUS

         ------------ -----------------

         MOUNTED      ACTIVE

iii) 

         alter database open;
         Database altered.

iv) 

         SELCET status, database_status from v$instance;

(output)

         STATUS       DATABASE_STATUS

         ------------ -----------------

         OPEN         ACTIVE

[SOLVED]

# Reasons

- Improper shutdown of oracle/system.


