# ZooLights Ticket Generator

## Project Overview
You are building a ticket generation system for ZooLights. This program will calculate ticket prices, validate eligibility for activities, and generate a formatted ticket for customers.

## Background Information

### Pricing
* **Walkthrough tickets (adults):** $16 weekdays, $25 weekends
* **Walkthrough tickets (kids):**
  * Under 2: Free
  * Ages 2-14: $8 weekdays, $12 weekends
  * Ages 15-17: $12 weekdays, $18 weekends
* **Drive-through:** $65 base price (up to 8 people), $12 per additional person over 8
  * Drive-through guests cannot access alcohol area or train ride

### Discounts
* Members receive 20% off (use code "MEMBER")

### Activity Eligibility
* **Alcohol area:** Must be 21 or older
* **Train ride:** Must be over 48 inches tall AND less than 300 lbs
* Drive-through guests are not eligible for alcohol area or train ride

## Program Requirements

Your program should:
1. Prompt the user for necessary information
2. Calculate the ticket price
3. Determine eligibility for activities
4. Generate and display a formatted ticket

### User Inputs (use Scanner)
* First and last name
* Visit date (mm/dd/yyyy format)
* Birthdate (mm/dd/yyyy format)
* Ticket type: walkthrough or drive-through
* If walkthrough:
  * Number of people in party
  * Whether they want to ride the train (if yes, get height and weight)
* If drive-through:
  * Number of people in the vehicle
* Discount code (if any)

### Ticket Output
Your ticket should display:
* Full name
* Ticket ID (5 random digits)
* Visit date and day of week
* Age on visit date
* Total cost
* Alcohol area access (Yes/No)
* Train ride access (Yes/No - N/A for drive-through)

## Required Static Methods

You must implement the following static methods. **Do not modify the method signatures.**

```java
/**
 * Calculates the day of the week from a date string
 * @param date String in format "mm/dd/yyyy"
 * @return day of week as String (e.g., "Monday", "Tuesday", etc.)
 */
public static String getDayOfWeek(String date)

/**
 * Calculates age based on birthdate and visit date
 * @param birthdate String in format "mm/dd/yyyy"
 * @param visitDate String in format "mm/dd/yyyy"
 * @return age as an integer
 */
public static int calculateAge(String birthdate, String visitDate)

/**
 * Determines if the visit date is a weekend
 * @param dayOfWeek String representing day (e.g., "Saturday")
 * @return true if weekend (Saturday or Sunday), false otherwise
 */
public static boolean isWeekend(String dayOfWeek)

/**
 * Calculates walkthrough ticket price for one person
 * @param age person's age on visit date
 * @param isWeekend whether visit is on weekend
 * @return ticket price as a double
 */
public static double calculateWalkthroughPrice(int age, boolean isWeekend)

/**
 * Calculates drive-through ticket price
 * @param numPeople number of people in vehicle
 * @return ticket price as a double
 */
public static double calculateDriveThroughPrice(int numPeople)

/**
 * Applies discount if applicable
 * @param originalPrice price before discount
 * @param discountCode discount code entered (may be empty string)
 * @return final price after discount
 */
public static double applyDiscount(double originalPrice, String discountCode)

/**
 * Determines if person can access alcohol area
 * @param age person's age on visit date
 * @param isDriveThrough whether ticket is drive-through
 * @return true if eligible, false otherwise
 */
public static boolean canAccessAlcohol(int age, boolean isDriveThrough)

/**
 * Determines if person can ride the train
 * @param heightInches height in inches
 * @param weightLbs weight in pounds
 * @param isDriveThrough whether ticket is drive-through
 * @return true if eligible, false otherwise
 */
public static boolean canRideTrain(double heightInches, double weightLbs, boolean isDriveThrough)

/**
 * Generates a random 5-digit ticket ID
 * @return 5-digit ticket ID as a String
 */
public static String generateTicketID()

/**
 * Displays formatted ticket information
 * @param name customer's full name
 * @param ticketID the generated ticket ID
 * @param visitDate the visit date string
 * @param dayOfWeek the day of week
 * @param age customer's age on visit date
 * @param totalCost final price
 * @param alcoholAccess whether they can access alcohol area
 * @param trainAccess whether they can ride train (use "N/A" for drive-through)
 */
public static void displayTicket(String name, String ticketID, String visitDate, 
                                  String dayOfWeek, int age, double totalCost, 
                                  boolean alcoholAccess, String trainAccess)
```

## Implementation Tips

### Calculating Day of Week from Date
You'll need to use the Zeller's Congruence algorithm or Java's built-in date classes. Research how to parse a date string and determine the day of week.

**Hint:** Look into `LocalDate` class and `DateTimeFormatter`

### Program Structure
Your `main` method should:
1. Create a Scanner
2. Prompt for and collect all necessary inputs
3. Call your static methods to perform calculations
4. Display the ticket using your display method

### Testing Strategy
Test your program with various scenarios:
* Different age groups (under 2, child, teen, adult, 21+)
* Weekday vs weekend visits
* With and without discounts
* Drive-through vs walkthrough
* Train eligibility edge cases (exactly 48 inches, exactly 300 lbs)

## Challenge Extensions (Optional)

Once your program works correctly:
1. **Format the ticket** - Add decorative borders using ASCII characters or emojis
2. **Input validation** - Ensure dates are valid and inputs are reasonable
3. **Multiple tickets** - Allow the user to generate multiple tickets in one run
4. **Group pricing** - For walkthrough parties, calculate individual prices and a total

## Simplified Flow (Compared to Original)

This version removes:
* Menu system for looking up tickets
* Data storage and retrieval
* Multiple ticket lookup capability

This version focuses on:
* Method decomposition
* Input/output
* Calculations and conditionals
* String manipulation
* Working with dates

## Grading Focus Areas
Your grade will be based on:
* Correct implementation of all required methods
* Proper use of parameters and return values
* Accurate calculations
* Clear, formatted output
* Code style and documentation
* Testing with various inputs
