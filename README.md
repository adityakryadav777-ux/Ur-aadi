
# Program to calculate bill with tip

n = int(input("Enter the number of items: "))

total = 0

for i in range(n):
    print("\nItem", i + 1)

    name = input("Enter item name: ")
    price = float(input("Enter item price: "))
    quantity = int(input("Enter quantity: "))

    amount = price * quantity
    total += amount

    print("Item:", name)
    print("Amount:", amount)

tip_percent = float(input("\nEnter tip percentage: "))

tip = total * tip_percent / 100
final_bill = total + tip

print("\n------ FINAL BILL ------")
print("Total Items:", n)
print("Total Bill:", total)
print("Tip Amount:", tip)
print("Final Bill:", final_bill)
