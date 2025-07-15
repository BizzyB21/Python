# Python
#Student Gradebook Analyzer
scores = []
students = {"Ally": [88, 93, 66],
            "Hector": [33, 86, 99],
            "Paula": [39, 96, 85],
            "Nikki": [90, 94, 98],
            "Andrew": [20, 49, 33],
            "Helen": [33, 23, 29],
            "Damian": [89, 87, 69],
            "Nathan": [34, 26, 41],
            "Mitch": [45, 38, 39],
            "Roger": [44, 28, 35],
            "Lily": [76, 86, 96],
            "Randy": [20, 30, 31],
            "Ethan": [24, 28, 29],
            "Adam": [74, 91, 95]
}
averages = {}
for name, scores in students.items():
    avg = sum(scores) / len(scores)
    averages[name] = avg

class_average = sum(averages.values()) / len(averages)
print(f"📊 Class Average: {class_average:.2f}\n")

print("🎉 Students Above Class Average:")
for name, avg in averages.items():
    if avg > class_average:
        print(f"{name}: {avg:.2f}")

print("\n❌ Students Who Failed (Average < 40):")
for name, avg in averages.items():
    if avg < 40:
        print(f"{name}: {avg:.2f}")

#Password
password = "August 17th"
max_attempts = 3
failed_attempt = 0
user = input("Enter the password:")
if max_attempts > failed_attempt:
    print("Account locked")
else:
        print("Welcome back!")

#Inventory Tracker for Small Business
product_items = {"Milk": 20,
                 "Bread": 100,
                 "Eggs": 100,
                 "Cereal": 60,
                 "Pasta": 40,
                 "Lotion": 250,
                 "Bananas": 80,
                 "Apples": 200,
                 "Pineapples": 150,
                 "Lemonade": 50,
                 "Jam": 70,
                 "Toothpaste": 90,
                 "Yoghurt": 60
}
stock = {}
stock_display = input("Enter product name:")
quantity_sold = input("Enter the quantity sold:")
stock_remaining = input("Enter what is remaining:")
if quantity_sold == 0:
    print("Out of stock")
    
#Bus Passenger
bus_capacity = 30
passenger_changes = [+5, -2, +4, +3, -1, +6, -3, +2]
current_passengers = 0
for i, change in enumerate(passenger_changes, start=1):
    current_passengers += change
    print(f"Stop {i}: Change = {change}, Passengers = {current_passengers}")
    
    if current_passengers > bus_capacity:
        print("Warning: Bus is over capacity!")
print(f"\nFinal number of passengers on the bus: {current_passengers}")

#Supermarket Receipt
groceries = ()
items = {"Milk": 1.99,
         "Eggs": 4.69,
         "Bread": 1.99,
         "Chicken": 28.99,
         "Furniture": 99.99,
         "Refridgerator": 199.99,
         "Pasta": 2.99,
         "Apple": 1.99,
         "Bananas": 1.99,
         "Ice cream": 5.49,
}

