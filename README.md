##Introduction:

The following document outlines the implementation of a simple shopping application. The application utilizes the following APIs provided by https://fakestoreapi.com to retrieve information about products and users:

https://fakestoreapi.com/products
https://fakestoreapi.com/products?limit=5
https://fakestoreapi.com/products/categories
https://fakestoreapi.com/products/category/jewelery
https://fakestoreapi.com/users
https://fakestoreapi.com/auth/login

## Features:

  ##Login Screen:
 A login screen will be the first screen that the user sees when opening the app. The user will be prompted to enter their email and password.
User authentication will be done using the /auth/login API provided by https://fakestoreapi.com.
After successful login, the user will be taken to the product listing screen.

 ##Product Listing Screen:
The product listing screen will display a list of all available products from the /products API provided by https://fakestoreapi.com.
The product list will implement lazy loading, where only a certain number of products are loaded at a time. Additional products will be loaded as the user scrolls down the list.
The list will be searchable, allowing the user to filter the products based on keywords.
FilterChip class from https://api.flutter.dev will be used to provide a filter option on different categories.

  ##Product Details Screen:
The user will be able to navigate to the product details screen by tapping on a product in the product listing screen.
The product details screen will display more detailed information about the selected product, including its name, description, and image.

  ##Cart Screen:
The user will be able to add products to their cart by tapping on the "Add to Cart" button in the product details screen.
The cart will be persisted even if the user closes the app from memory, meaning that the items in the cart will still be there when the user reopens the app.
The cart screen can be accessed by tapping on the cart button in the app bar on the top of the screen.
On cart screen, user can see all the items added to the cart and the option to remove items from cart.

 ##Error Handling and Recovery:
Error handling was implemented to ensure that the app can gracefully handle any errors that occur during the loading of data from the APIs.
In case of error, proper message will be displayed to the user.

file:///Users/topgamer/Desktop/Screen%20Shot%202023-01-10%20at%2022.39.35.png

