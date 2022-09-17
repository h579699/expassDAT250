# expass3 DAT250
### Goal
The purpose of this assignment was to get familiar with MongoDB.

### Installation
Validation of installation package:
![image](https://user-images.githubusercontent.com/53999377/190858555-0f9a7744-3edc-4c5b-a939-0985e4451243.png)


### Experiment 1: MongoDB CRUD operations
##### CREATE ([insert](https://docs.mongodb.com/manual/tutorial/insert-documents/))
![image](https://user-images.githubusercontent.com/53999377/190858821-c393b265-0408-479b-8866-7fecfdfe8666.png)

##### READ ([query](https://docs.mongodb.com/manual/tutorial/query-documents/))
![image](https://user-images.githubusercontent.com/53999377/190858835-5b18c7b0-6344-47ab-97a7-a9bf39cc066f.png)
*Used the MongoDB Compass, an example using the find method from Mongo Shell is shown in experiment 2.

##### UPDATE ([update](https://docs.mongodb.com/manual/tutorial/update-documents/))
![image](https://user-images.githubusercontent.com/53999377/190858848-0b8ef899-cfb2-44c5-905b-e1fa451fd1af.png)

##### DELETE ([remove](https://docs.mongodb.com/manual/tutorial/remove-documents/))
Before deleting:
![image](https://user-images.githubusercontent.com/53999377/190858855-3152c0a9-f5dd-49e1-b96d-e941b9c62344.png)
After deleting:
![image](https://user-images.githubusercontent.com/53999377/190858866-fa649da3-a523-48f7-a82e-144fd17b720a.png)

##### BULK WRITE ([bulk write](https://docs.mongodb.com/manual/core/bulk-write-operations/))
![image](https://user-images.githubusercontent.com/53999377/190858877-f7ac4a71-a554-411e-b2d3-b415d1420a05.png)

### Experiment 2: Aggregation
##### Example 1
![image](https://user-images.githubusercontent.com/53999377/190858927-83e3f568-dd16-457c-8525-3bc755e0ba0d.png)

##### Example 2
<img width="400" alt="image" src="https://user-images.githubusercontent.com/53999377/190858979-89fa9239-7c69-4dfa-8b99-62d223308ff9.png">

![image](https://user-images.githubusercontent.com/53999377/190859022-44ac207f-e976-4946-a48f-9e2a62427348.png)

![image](https://user-images.githubusercontent.com/53999377/190859027-a21bd3c3-7855-4ce8-ae3c-591ccc18eb96.png)

##### Own example
![image](https://user-images.githubusercontent.com/53999377/190859036-52c8a264-9aef-4296-be9b-b0607576534b.png)
My map-reduce operation shows the average price for the total quantity of items in an order, for orders with a price greater or equal to 50. The result may be useful for analysing if orders contain mostly cheap or mostly expensive items, or a mix of the two. 

### Issues
I encountered some problems with the Mongo Shell. I wasn't able to copy paste the examples from the tutorial into the Mongo Shell, and therefore I had to use a lot of time copying the examples by hand. The MongoDB Compass was easier to use. 
