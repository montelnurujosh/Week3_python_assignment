# Discount Calculator

## Description
A Python program that calculates the final price of an item after applying a discount.  
If the discount percentage is 20% or higher, the discount is applied.  
Otherwise, the original price is returned.

## Features
- Accepts original price and discount percentage from the user.
- Applies discount only if it's 20% or more.
- Returns the final price or the original price.

## Function Definition
def calculate_discount(price, discount_percent):
    if discount_percent >= 20:
        discount_amount = price * (discount_percent / 100)
        return price - discount_amount
    else:
        return price

## Example Usage
original_price = float(input("Enter the original price: "))
discount_percent = float(input("Enter the discount percentage: "))

final_price = calculate_discount(original_price, discount_percent)

print(f"The final price is: {final_price}")

## Example Output
Enter the original price: 1000
Enter the discount percentage: 25
The final price is: 750.0


