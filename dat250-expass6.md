# expass6 DAT250
### Goal
The purpose of this assignment was to do initial experiments with front-end technologies for enterprise applications.

### Experiment 1
I completed the following tutorial on Spring MVC: https://spring.io/guides/gs/serving-web-content/

Link to code: https://github.com/h579699/expass6DAT250/tree/master/serving-web-content

### Experiment 2
When implementing the Angular front-end for the Todo API, I was inspired by the following tutorial: https://www.javaguides.net/2021/08/angular-crud-example.html

![image](https://user-images.githubusercontent.com/53999377/194704130-bce7d375-dd82-4c63-834a-871e87cadbe4.png)

![image](https://user-images.githubusercontent.com/53999377/194704137-2e6412f6-39c8-4d8b-add2-adbffa9dbd7b.png)

Link to code: https://github.com/h579699/Todo-Angular

### Issues
I had some issues with CORS when trying to access the Todo API from the Angular CLI application. 
I resolved the issue by modifying the Todo API with the following code:

```java
options("/*",
        (request, response) -> {

            String accessControlRequestHeaders = request
                    .headers("Access-Control-Request-Headers");
            if (accessControlRequestHeaders != null) {
                response.header("Access-Control-Allow-Headers",
                        accessControlRequestHeaders);
            }

            String accessControlRequestMethod = request
                    .headers("Access-Control-Request-Method");
            if (accessControlRequestMethod != null) {
                response.header("Access-Control-Allow-Methods",
                        accessControlRequestMethod);
            }

            return "OK";
        });

before((request, response) -> response.header("Access-Control-Allow-Origin", "*"));
```
