# Database-Programming-Assignment-30583-2025-ALSHEAB

Oracle PDB Administration Assignment II

​1. Assignment Overview:

​This individual practical assignment focuses on developing Oracle Database administration skills, specifically through the implementation of Oracle Multitenant Architecture and the management of Pluggable Databases (PDBs).

​2. Oracle Environment:

​- Oracle Version: Oracle AI Database 26ai Free Release 23.26.2.0.0
​- Operating System: Windows
​- Tools Used: SQL*Plus, Oracle Enterprise Manager (OEM) Express

​3. Task Documentation:

​- PDB Creation: Successfully created sh_pdb_30583_2025 using the CREATE PLUGGABLE DATABASE command with FILE_NAME_CONVERT.

​- User Configuration: Created the user sh_plsqlauca_30583_2025 and granted the necessary privileges (CONNECT, RESOURCE, DBA).

​- Temporary PDB: Created and subsequently dropped sh_to_delete_pdb_30583_2025 including its datafiles.

​- OEM Configuration: Attempted to configure and access Oracle Enterprise Manager (OEM) Express via port 5500.

​4. Challenges and Solutions:

​- Challenge: Encountered ORA-01031: insufficient privileges and ORA-65040: Operation not allowed errors.

​- Solution: Resolved by connecting as sysdba and ensuring the session container was set to CDB$ROOT before executing administrative commands.

​- Challenge: The OEM Express interface on port 5500 refused to connect (ERR_CONNECTION_REFUSED).

​- Solution: Executed EXEC DBMS_XDB_CONFIG.SETHTTPSPORT(5500); to enable the port. Despite successful execution, the connection remained unreachable due to local environment restrictions. Relevant error logs are documented in the screenshots folder.

​5. Lessons Learned:

​Through this assignment, I gained a deeper understanding of Oracle's Multitenant Architecture, the importance of container management, and the practical application of SQL commands for managing PDB lifecycles. I also improved my troubleshooting skills regarding database connectivity and privilege management.

​6. Integrity Statement:

​"I confirm that this assignment represents my own practical work, screenshots, and documentation. All external resources consulted have been properly acknowledged."
