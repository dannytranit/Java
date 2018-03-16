# Java
This is a reservation and billing system using Java
Required configuration steps before executing Customer Management sub system of Star Hotel
1. Mysql is used in this project.
2. Add mysql-connector-java-5.0.8-bin.jar under \lib directory to the project library.
3. Change server and database configuration details in ConnectionFactory.java.
  Below are the variables need to be changed:
  private static final String SERVER= "localhost";
	private static final String DATABASE_NAME = "star_hotel"; //Please use an existing database as the built-in script does not create a new database
	public static final String USER = "root";
	public static final String PASSWORD = "12345"; 
   ***Note: Please use an existing database as the built-in script does not create a new database. It only creates tables in an existing database.
4. Run Main.java to create Customer and Booking tables and some customer data.
   If Customer and/or Booking tables are already existing, then the built-in script will drop these two tables and create new one.
5. Run GUI.java for the main screen of Customer Management module.
6. Refer to Appendix for completed java source code. 

Star Hotel Directory Structure:
Src
   com.starhotel.mngt
             ConnectionFactory.java
             Customer.java
             CustomerManager.java
             CustomerManagerImpl.java
             DbUtil.java
             Util.java
             GUI.java
             LCPanel.java
             Main.java
             NCDialog.java
             SCDialog.java
             UCDialog.java
             VCDialog.java
lib
   mysql-connector-java-5.0.8-bin.jar
