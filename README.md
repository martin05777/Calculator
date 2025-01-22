#This code has a bit hungarian in it such as "kivonás, osztás, nem értelmezhető"
def kivonás(x, y):
        if y == 0:
            print("nem értelmezhető")
        else:
            return x-y

def osztás(x, y):
        if y == 0:
             print("nem értelmezhető")
        else:
            return x/y

def szorzás(x, y):
         if y == 0:
             print("nem értelmezhető")
         else:
            return x*y

def összeadás(x, y):
            if y == 0:
                 print("nem értelmezhető")
            else:
                return x+y

print("Válassz eggyet")
print("1. kivonás")
print("2. osztás")
print("3. szorzás")
print("4. összeadás")

operation = input("Enter choice (1/2/3/4): ")

if operation in ('1', '2', '3', '4'):
    num1 = float(input("Adj meg egy számot:"))
    num2 = float(input("Adj meg még egy számot:"))
     
if operation == '1':
    print(f"{num1} - {num2} = {kivonás(num1, num2)}")
elif operation == '2':
    print(f"{num1} / {num2} = {osztás(num1, num2)}")
elif operation == '3':
    print(f"{num1} * {num2} = {szorzás(num1, num2)}")
elif operation == '4':
    print(f"{num1} + {num2} = {összeadás(num1, num2)}")
else:
    print("Helytelen.Adj meg egy értelezhető operátort")
