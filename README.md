# expass1 DAT250
### Goal
The purpose of this assignment was to ensure that my PC had a working Software Development Environment (SDE) installed. The requirements for the SDE was a Java Development Environment (JDK), an Integrated Development Environment (IDE), the Maven software management tool and a Git client installed. In additon to this a GitHub account was needed for handing in the assignment. 

### Installation of SDE
I already had several JDK versions installed on my PC, but installed a newer version, [JDK 18](https://www.oracle.com/java/technologies/downloads/). I also installed the Eclipse IDE for Java Developers using the [Eclipse Innstaller 2022-06](https://www.eclipse.org/downloads/packages/). Furthermore, I followed the instructions from [Maven](https://maven.apache.org) to download and install the Maven software management tool. I also added Maven to the *PATH* variable. 

I already had a GitHub account, and a Git client and a Heroku Command Line Interface (CLI) installed. 

To verify the installations I did the following: 
- Java and Eclipse: Opened the Eclipse IDE and ran a Java project
- Maven: mvn -version *(in Command Prompt)*
- Heroku CLI: heroku -v *(in Command Prompt)*

### Validation of SDE
I validated that the SDE was working properly, by completing the [Getting Started on Heroku with Java](https://devcenter.heroku.com/articles/getting-started-with-java). Before starting the tutorial, I also had to download and install [PostgreSQL](https://www.enterprisedb.com/downloads/postgres-postgresql-downloads) and set it up locally. I also added PostgreSQL to the *PATH* variable. 

The steps taken to validate the SDE are further described in the [tutorial](https://devcenter.heroku.com/articles/getting-started-with-java). I already had some experience with the Heroku platform and didn't encounter any major problems during the tutorial. However, I struggled a bit with getting the application to work locally when connecting to a local PostgreSQL database. The problem was that the connection string (JDBC_DATABASE_URL) in the .env file wasn't correct. I found the correct connection string and solved the problem, and got the application to work locally.           

Link to Heroku application: https://expass1-heroku.herokuapp.com
