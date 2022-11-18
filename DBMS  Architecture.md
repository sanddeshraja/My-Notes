
1. <u>One tier Architecture</u>!
      - DB directly available to user
      - Required components like the interface, middle wave  and backend data, all on one server or platform
      - any changes done here will be directly done on the database itself. Doesnt provide handy tool for end users.
      - 1 tier architecture is used for development of the local Application. When programmer can directly communicate with Db for quick response

 2. <u> Two Tier Architecture</u>
        - Basic  Client-Server
        - ![[download 1.svg]]

 Intersection between both using API 's like ODBC,JDBC
 Query Processing transaction management in server

3.  Three Tier Architecture
      - Large Web Application
      - Client doesnt directly communicate with the server
      - The application of the client end interacts with an application server which further communicate with DB system
      - End user -- no idea -- existence of DB beyond  Application server --vice versa.
  
![[DBMS  Architecture 2022-10-16 16.30.57.excalidraw]]