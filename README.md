# GFG_Stock_problem_vivek
Purpose:

The code aims to find the maximum number of products that can be bought with a given budget k, considering a set of n products with their respective prices.
Class and Function:

The code defines a class named Solution with a public member function buyMaximumProducts.
This function takes three parameters:
n: The number of products available.
k: The budget available for buying products.
price[]: An array containing the prices of the products.
It returns an integer representing the maximum number of products that can be bought within the budget.
Logic:

Organizing Product Information:
A vector named info is created to store pairs of (price, product index).
The prices and corresponding indices are filled into this vector.
Sorting Products by Price:
The info vector is sorted in ascending order of prices, ensuring prioritization of cheaper products.
Iterating and Buying:
A variable ans is initialized to 0 to track the total number of products bought.
The code iterates through the sorted info vector:
For each product:
It calculates the maximum quantity that can be bought with the remaining budget (k).
It ensures the quantity doesn't exceed the available stock of that product.
It updates the ans (total products bought) and k (remaining budget).
Returning the Result:
The function returns the ans variable, which holds the maximum number of products purchased.
Key Points:

The code prioritizes buying cheaper products first to maximize the total number of products bought.
It considers the available stock of each product to ensure realistic purchase quantities.
It efficiently tracks the remaining budget and updates it after each purchase.
Example:

Python
n = 5  # Number of products
k = 10  # Budget
price = [2, 3, 4, 5, 1]  # Product prices

max_products = buyMaximumProducts(n, k, price)
print(f"Maximum number of products bought: {max_products}")
Use code with caution. Learn more
Output:

Maximum number of products bought: 7
