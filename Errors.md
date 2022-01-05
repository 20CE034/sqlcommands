## ERROR 

# [SOLVED] #1 ORACLE initialization or shutdown in progress 

follow these steps
# i)                                  

         username - (system or c##(user)) as sysdba
         password - (Oracle#143 or cspit)

# ii) 

         SELECT status, database_status from v$instance;

(output)

         STATUS       DATABASE_STATUS

         ------------ -----------------

         MOUNTED      ACTIVE

# iii) 

         alter database open;
         Database altered.

# iv) 

         SELCET status, database_status from v$instance;

(output)

         STATUS       DATABASE_STATUS

         ------------ -----------------

         OPEN         ACTIVE


# _Reasons

- Improper shutdown of oracle/system.


# [SOLVED] #2 ORACLE not available (ORA-01034) & shared memory realm does not exist (ORA-27101)
 
# Restart service ![Image](https://cdn.discordapp.com/attachments/794818958686552145/928135228386607164/unknown.png)

# _Reasons
- Improper Shutdown/Startup
-

# [AWAITING] #3 ORACLE not available  
