Discount Calculator 🏷️
Description

This Python program calculates the final price of an item after applying a discount.
If the discount percentage is 20% or higher, the discount will be applied; otherwise, the original price will be returned.

Features

Takes original price and discount percentage as inputs.

Applies the discount only if it is 20% or higher.

Returns the original price if the discount is below the threshold.

Function Definition
def calculate_discount(price, discount_percent):
    if discount_percent >= 20:
        discount_amount = price * (discount_percent / 100)
        return price - discount_amount
    else:
        return price

How It Works

Prompt the user to enter the original price.

Prompt the user to enter the discount percentage.

Call calculate_discount(price, discount_percent) to get the final price.

Display the final price.

Example Usage
# User Input
original_price = float(input("Enter the original price: "))
discount_percent = float(input("Enter the discount percentage: "))

# Function Call
final_price = calculate_discount(original_price, discount_percent)

# Output
print(f"The final price is: {final_price}")

Example Output
Enter the original price: 1000
Enter the discount percentage: 25
The final price is: 750.0
