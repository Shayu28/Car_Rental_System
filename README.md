# Car_Rental_System

Algorithm:
1. Start Program:

* Initialize the CarRentalSystem with empty lists of cars, customers, and rentals.
* Create and add predefined cars (Car objects) to the system.

2. Display Menu:

* Show the following options to the user:
* Rent a Car
* Return a Car
* Exit

3. User Selection:

* Get the user's choice:
* If the user selects 1 (Rent a Car), proceed to step 4.
* If the user selects 2 (Return a Car), proceed to step 8.
* If the user selects 3 (Exit), terminate the program.
* For any other choice, display an error message and redisplay the menu.

4. Rent a Car Process:

* Prompt the user for their name.
* Display the list of available cars (i.e., cars that are not rented).
* Ask the user to enter the carId of the car they wish to rent.
* Ask for the number of days the car will be rented.

5. Check Availability of the Car:

* Search the list of cars for the selected carId.
* If the car is available, proceed to step 6.
* If the car is not available or the carId is invalid, display an error message and go back to the menu.

6.Confirm Rental:

* Calculate the total rental price (price = basePricePerDay * rentalDays).
* Display the rental details (customer information, car model, number of rental days, and total price).
* Ask the user to confirm the rental (Y/N).

7. Rent the Car:

* If the user confirms (Y):
* Create a new Customer object with a unique customer ID and the provided name.
Add the customer to the list of customers.
Rent the car (mark it as unavailable) and add a new Rental object to the list of rentals.
Display a success message.
If the user cancels (N), display a cancellation message.
Return to the main menu.
Return a Car Process:

Ask the user for the carId of the car they want to return.
Search for the car in the list of cars:
If the car is found and it is rented, proceed to step 9.
If the car is not rented or the carId is invalid, display an error message and return to the main menu.
Return the Car:

Search the rentals for the corresponding rental that matches the car.
If found, return the car (mark it as available) and remove the rental from the system.
Display a success message indicating the car has been returned.
Return to the main menu.
Exit Program:

If the user selects "Exit," display a thank-you message and terminate the program.
