# expass2 DAT250
### Goal
The purpose of this assignment was to get to know the Java Persistence Architecture (JPA).

### Experiment 1: JPA Tutorial
I completed a [introduction to JPA tutorial](https://www.vogella.com/tutorials/JavaPersistenceAPI/article.html#installation) to get more familiar with the use of JPA. I downloaded the [starting point code](https://github.com/timKraeuter/dat250-jpa-example) from GitHub before starting the tutorial. I experienced some issues with the use of the Derby JDBC Driver. When specifying a local *jdbc.url* in the *persistence.xml* I repeatedly got an error message that the Driver couldn't be found. After some trial and error I got the program to work by changing the *jdbc.url*. I am not quite sure what was the problem in the first place, but I suspect it had something to do with the placement of the database (outside of the Maven project). 

Another issue I had, was inspecting the database tables being created. At first, I installed the Eclipse Data Tools Platform (DTP) Project to try to inspect the tables from Eclipse. After having installed the DTP, I changed to the *Database Development* perspective in Eclipse and tried to establish a connection to the database, but I couldn't get it to work. At last I was able to inspect the tables by downloading the [Derby Database Server](https://db.apache.org/derby/papers/DerbyTut/index.html) locally and using the *ij* toll in Command Prompt. 

To use the *ij* tool I followed the steps from a [Derby Tutorial](https://db.apache.org/derby/papers/DerbyTut/ij_intro.html) and from the *GoncalvesCh4.pdf* (from Canvas). In the Command Prompt I used the following commands:
- *set DERBY_INSTALL= < path to where Derby is downloaded >*
- *set CLASSPATH=%DERBY_INSTALL%\lib\derby.jar;%DERBY_INSTALL%\lib\derbytools.jar;%DERBY_INSTALL%\lib\derbyoptionaltools.jar;%DERBY_INSTALL%\lib\derbyshared.jar;*
- Changed directory to where my database was located: *cd < database location >*
- Started ij: *java org.apache.derby.tools.ij*
- Connected to database: *connect '< path to database >';*
- Inspected the schema with *show tables;* and the tables with *describe table;*

### Experiment 2: Banking/Credit Card example JPA
I implemented the [domain model](https://raw.githubusercontent.com/selabhvl/dat250public/master/expassignments/pictures/creditCard.svg) from the assignment by using JPA annotations and the starting point code for *experiment-2*. I then ran the project to create the database tables. I used the *ij* tool to inspect the tables.

#### Screenshots of the database schema 
<img width="400" alt="image" src="https://user-images.githubusercontent.com/53999377/188209843-ef475bd1-4e4f-4457-898d-eefa7913c6e1.png">

The last step, was to persist the [object diagram](https://raw.githubusercontent.com/selabhvl/dat250public/master/expassignments/pictures/object-diagram.svg) from the assignment into my database and run the test case MainTest successfully.

#### Screenshots of running the MainTest 
![image](https://user-images.githubusercontent.com/53999377/188210371-1f0281a5-69e5-477d-83b0-e0e4d9a60824.png)

Link to your code for experiment 2:
