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
