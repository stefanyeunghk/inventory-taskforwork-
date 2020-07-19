# inventory-taskforwork-
Author: Stefan Yeung

Steps to run the project

1. Install Netbeans
2.restore the database in this zip file
3.open and run the project

PS. I have uploaded two pictures which show the tables of database and the display page of the java web application. This is for a stituation where my project cannot be opened in other computer.



Day 1. First time making an complete java web application from scratch.
I am not sure if I can finish it in 3 days, but I will give it my best 

shot. 
 I decided to use netbean for application, and I will use java database 

to make the database.

A java DB is created, and it has a table (product)


Spec to remember: 
develop a light version Warehouse Inventory System
able to store product data via csv file consumption.
able to store quantities of such products in different locations via 

csv file consumption.
UI to show inventory level of given product code
able to transfer inventory from one location to another given amount of 

quantity and product code via UI


Day 2. 

Created initial database and connected it to the java web application. 

Inside product table, there are four columns. (Code, Productname, 

Weight, Location)

Read a lot of website trying to figure out how to store database's data 

into a csv file, but still can't do it. 

Day 3. 

Decided to install opencsv library into netbeans. Yes, I am able to 

write to a csv file or txt file, but I still don't know how to convert 

database data into a .csv file..

Created a class called inventorystore.java I intend to use this class 

file to get data from database, and then use this class to write to a 

csv file.

Created another .java file. Trying to connect to database and store 

data into public class inventorydao. However, not sure how to process 

as there will be error if the class is called.

in index.jsp, I am trying to store the value of user input.

            function getcode() {
            var input = document.getElementById("newcode").value;
            alert(input);
            



        <%
         String connectionURL = "jdbc:derby://localhost:1527/sun-	appserv-samples";
        //ConnectionURL, username and password should be specified in 	getConnection()
        try {
        Connection conn = DriverManager.getConnection(connectionURL, 	"", "");
        System.out.println("Connect successfully ! ");
        conn.close();
        } catch (SQLException ex) {
        System.out.println("Connect failed ! ");
        }
        
        %>
