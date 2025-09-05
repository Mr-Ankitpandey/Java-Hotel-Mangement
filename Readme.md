# Hotel Management System

## Overview

This is a **Hotel Management System** written in Java. It allows hotel staff to manage room bookings, check room availability, order food for rooms, and handle customer checkouts. The system uses file serialization to save and restore hotel data between sessions.

## Features

- **Room Booking:** Book luxury/deluxe, single/double rooms for customers.
- **Room Availability:** Check the number of available rooms for each room type.
- **Room Details:** View features and charges for each room type.
- **Food Ordering:** Order food items for any booked room.
- **Billing:** Generate and display the bill for room and food charges at checkout.
- **Data Persistence:** All data is saved to a `backup` file and restored on startup.

## Room Types

1. **Luxury Double Room** (AC, Free breakfast, ₹4000/day)
2. **Deluxe Double Room** (Non-AC, Free breakfast, ₹3000/day)
3. **Luxury Single Room** (AC, Free breakfast, ₹2200/day)
4. **Deluxe Single Room** (Non-AC, Free breakfast, ₹1200/day)

## Food Menu

- 1. Sandwich - ₹50
- 2. Pasta - ₹60
- 3. Noodles - ₹70
- 4. Coke - ₹30

## How It Works

1. **Startup:**  
   On launch, the system loads previous hotel data from the `backup` file if it exists.

2. **Main Menu:**  
   The user is presented with options to:
   - Display room details
   - Display room availability
   - Book a room
   - Order food
   - Checkout (deallocate room)
   - Exit

3. **Booking:**  
   The user selects a room type and chooses an available room number. Customer details are entered for the booking.

4. **Ordering Food:**  
   The user enters the room number and selects food items and quantities to add to the room's bill.

5. **Checkout:**  
   The user enters the room number to checkout. The system displays the bill and deallocates the room.

6. **Exit:**  
   On exit, the current hotel data is saved to the `backup` file for persistence.

## How to Run

1. **Compile:**
   ```sh
   javac Main.java
   ```
2. **Run:**
   ```sh
   java Main
   ```

## File Structure

- `Main.java` - Main source code file containing all classes.

## Notes

- All data is stored locally in the `backup` file.
- The system is console-based and requires user input for all operations.

---

**Code by:**  

@nkit
