### Swapping
```
a = 20
b = 10
# a,b = b,a

c = a
a = b
b = c


print(" this is valu of a ",a)
print("This is value of b ",b)


```
# Take prices of three products and print total, average and remaining amount from 1000
```
prod1 = int(input("Enter the price of Pruduct1:"))
prod2 = int(input("Enter the price of Pruduct2:"))
prod3 = int(input("Enter the price of Pruduct3:"))

Total = prod1 + prod2 + prod3
Average = Total / 3
Remain = 1000 - Total

print("Your Total Amount is : ", Total)
print("Average of your price :", Average)
print("Your remain amount is :", Remain)
```
## with GST 

```
# Take prices of three products and print total, average and remaining amount from 1000

prod1 = int(input("Enter the price of Pruduct1:"))
prod2 = int(input("Enter the price of Pruduct2:"))
prod3 = int(input("Enter the price of Pruduct3:"))

Total = prod1 + prod2 + prod3 
GST = Total * 0.18
GST_Total = Total + GST
Average = GST_Total / 3
Remain = 1000 - GST_Total
print("Your Total Amount is : ", Total)
print("Your Total Amount with GST is : ", GST_Total)
print(f"Average of your price :{Average:.2f}")
print("Your remain amount is :", Remain)


```

### Loops and Cond.

```
# age = int(input("Enter Your age : "))
# has_id = True
 
# if age >= 18 and has_id:
#       print("Entry allowed")

today = input("Enter today's day : ")
workday = ["Monday","Tuesday","Thursday","Friday"]
weekend = ["Saturday","Sunday"]
holliday = ["wenesday"]

def day():
  
  for i in workday:
    if i == today:
      print(f" Today is {today} This is your workday")
    
      
  for i in weekend:
    if i == today:
      print("Today is weekend")
      
  for i in holiday:
    if i == today:
      print("Today is Holiday")
      
for i in holiday and weekend and workday:
  if i != today:
    print("check your input again")


    
# if is_weekend or is_holiday:
#     print("No office")
  
# else:
#   print("Go Regular to your work")
```
## For Loops in Funcions
```
def average(numbers):
  Total = 0
  for number in numbers:
    Total += number
    
  return Total / len(numbers)
numbers =[80,75,90,85]
print(average(numbers))
```
----
```

def calculate_average(numbers):

    total = 0

    for number in numbers:
        total += number

    # len() gives number of elements
    return total / len(numbers)


marks = [80, 75, 90, 85]

print(calculate_average(marks))
```
