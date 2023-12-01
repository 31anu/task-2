#Approach

The code can be divided into the following main sections:
Cart Data:

*Defines an empty cart array to store cart items.
*Initializes a variable cartTotal to track the total cart amount.
*Retrieves DOM elements for the cart container (cartDom) and add-to-cart buttons (addtocartbtnDom).

Adding Items to Cart:

*Attaches a click event listener to each add-to-cart button.
*Within the event listener, extracts product information from the button's parent element.
*Creates a product object with product details (image URL, name, price, and quantity).
*Checks if the product already exists in the cart. If not, adds it to the cart array.
*Updates the cart UI by dynamically creating a cart item element and appending it to the cart container.
*Updates the add-to-cart button's text to "In cart" and disables it to prevent duplicate additions.

Cart Item Management:

*Attaches event listeners to cart item elements for increasing, decreasing, and removing items.
*For the increase button, increments the product quantity in the cart and updates the cart item UI accordingly.
*For the decrease button, decrements the product quantity in the cart and updates the cart item UI accordingly.
*If the quantity reaches zero, removes the product from the cart and updates the cart item UI.
*For the remove button, removes the product from the cart and updates the cart item UI.
*Additionally, checks if the cart is empty and removes the cart footer if necessary.

Clear Cart and Checkout:

*Attaches an event listener to the "Clear Cart" button.
*Upon clicking the button, removes all cart items from the cart array and updates the cart UI.
*Resets the cart total to zero and removes the cart footer if it exists.
*Enables all add-to-cart buttons.