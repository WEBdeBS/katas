# Beverage machine kata
The idea of this kata is to implement the logic that govern a coffee machine controller that serves beverages like coffee, tea, chocolate when requested. It will start from simple functionality and grow to a more complex logic by adding more use cases.

Try to implement this program in TDD adding one functionality at the time. Theres no need to build the user interface, just stick to the user story.
The stories are divided in three iteration of different difficulty.

### Basic machine operation with coins and keys

* When the coffee machine starts it is ready to operate and the credit is zero.
* As a user I can insert coins of different formats (5, 10, 20 cents) and the displayed credit should grow accordingly.
* As a user I can cancel the operation and have the money back.
* As a user I can insert a prepaid key. The key can have some credit loaded and it will be displayed (sum it to actual credit).
* The user can extract the key and the credit should not be changed 
* The user can recharge the key using the coins. The eventually present credit is passed to the key.


### Making beverages
* When the credit as reached 30cents the user can get a coffee. If the credit is not enough the machine should display a message with the price of the coffee (30cents). Credit should decrease accordingly.
* The machine can deliver different types of beverages: Tea and Chocolate. Tea costs 40cents. Chocolate costs 60cents.
* As a user if I buy the beverage with the key the costs are lower than the actual prices of 0.5cents.

### Add-ons
* As a user I can set the desired level of sugar to use (1 to 5) and the machine must use it to prepare the beverage.
* As a user I can add add-ons to the beverages: super-hot beverage, sweetener, honey. Every add-ons costs 10cents and I can add more than one for a single beverage
* More add-ons are available but these can be used only with specific beverage:
	* Lemon (10cents), Milk (20cents) with Tea
	* Decaf (0cents), Milk (20cents), Cream(20cents) with coffee
	* Whipped Cream(30 cents), nuts (30 cents) with chocolate

### Extras
* The coffee machine has limited number of beverage available. 50 Tea, 50  Coffee, 50 Chocolate. When the machine runs out of one of them an Administrator must reload the beverage.
* If the users use the key to get the beverage, every 10 euros of they get a free coffee.
* The owner of the machine would like to receive a monthly report with the list of all orders (add-ons included)
