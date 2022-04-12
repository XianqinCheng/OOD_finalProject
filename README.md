# OOD_finalProject
This is OOD_finalProject by team 9

Operating environment:

1. MySQL. You can download this online installer: https://dev.mysql.com/downloads/windows/installer/8.0.html to install MySQL Community Edition.
2. Redis. Download address: https://github.com/servicestack/redis-windows/tree/master/downloads, download the latest version of redis-latest.zip, and unzip it. You can see the redis-server.exe file in the decompressed root directory, and double-click to start the redis server.
3. Nginx. Download address: http://nginx.org/en/download.html. The downloaded zip package, after decompression, has the nginx.exe file in the root directory, double-click to start the nginx server.
4. IDEA. Download address: https://www.jetbrains.com/idea/download/#section=windows
5. JDK1.8+, maven, IDEA.

Note: IDEA does not download the Community version, download the Ultimate version. The MySQL database I use is version 5.7.21. The table building statement in this project seems to be incompatible with version 5.6. It is recommended to install versions above 5.7. We recommend a relatively easy-to-use MySQL client: Navicat for MySQL. Redis client graphical interface: Redis Desktop Manager. It is best to change the Maven remote warehouse to Alibaba Cloud warehouse. There is an introduction to the modification method on the Internet, which is very simple.

Operation mode:

1. Use the command git clone https://github.com/XianqinCheng/OOD_finalProject.git to clone the project locally.
2. Import the project into IDEA. In IDEA, File->open..., then select the project folder (springboot-project). If you are using spring boot for the first time, this process may take a while, and you need to download many dependent jar packages.
3. Install lombok plugin for IDEA. In IDEA, File->Settings...->Plugin, search for lombok, and install it. When the project wiki introduces the log, it mentions why this plugin is installed.
4. The configuration file of the project is in the resources directory, the application.yml file. Modify MySQL database connection information. My database account password is root, 123456, you can change it to yours.
5. Run the sql script of the table building statement on the MySQL database terminal (or use the Navicat for MySQL graphical tool you just downloaded). The table building statement in this project is sqmax.sql under the project root path.
6. Start redis. In the Redis root directory you just decompressed, double-click redis-server.exe to run the redis service.
7. Finally, the project can be started. Run the main class SellApplication in the way of Spring Boot in IDEA. It can be seen that this is different from the way our traditional web projects are started. We have not configured servers such as tomcat, etc., because Spring Boot has introduced the server into the starting dependencies.
8. After the above steps, our project should be ready to start. Visit: http://127.0.0.1:8080/sell/seller/product/list, you can come to the merchant management system interface of our seller side. 
