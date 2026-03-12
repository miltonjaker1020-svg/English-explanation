# Inventory system
## good afternoon or morning (depends when you see this). Here I am going to explain how my Pyhton Program works
### this program is a simple inventory script that asks the users a  few information about the product:
1. what its name is??
2. what its price is??
3. what its amount is??
### then ask the users if they want to know just the final price or the complete purchase details,so if the users chose "just the final price" the system printed your have to pay.... but it the choose the other opcion, it prints the full infomation

#### example:
```
what its the name of the product, you want to buy??
Apples
```
```
What is price its??
$5.40
```
```
what is amount its???
3 
```
```
what do you want to view???
1. the final price 
        or
2. the complete purchase detail

2 
```
```
Producto: Apples
Precio: $5.40
Cantidad: 3
Costo total: 16.2
```

### How it works??
#### firts, the program begins with a ```while true``` loop, which means the program will keep running until a specific condition stops it
#### the first thing the program asks is what is the _name of the product_??. the user introduces the name of the product and the program verifies if the name is valid using the function ```isalpha()```.This function checks the input and if this one only has letters. If the name is invalid, the program asks the name of the product again.
















#### Next, the program asks the _price of the product_(the product selected ). this process is into a ```try-except```block. The try block attempts to convert the input on a float,so if the user enters an invalid value like string(text), the program catches the error and asks the price of the product again. also verifies that the price is not a negative value.






#### After that, the program asks _the quantity of the product_(using a similar procces validation),changes the input for an integer number and checks if it is not a negative number


#### once the program has price and quantity, it calculates the final cost by multiplying the previous price and quantity.

#### Finally, the program asks the user what infomation they want to see. They can choose between just watch the final cost or the complete purchase detail, depending on the user's choice, the program shows the result of the previous choice
