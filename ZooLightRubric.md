# ZooLights Ticket Generator - Grading Rubric
## AP Computer Science A

**Student Name:** _______________________  
**Total Points: ______ / 100**

---

## Method Implementation (60 points)

### getDayOfWeek (6 points)
- [ ] 6 pts - Correctly parses date string and returns accurate day of week
- [ ] 4 pts - Returns day of week but has minor formatting issues
- [ ] 2 pts - Attempts implementation but has logical errors
- [ ] 0 pts - Not implemented or completely incorrect

**Comments:**

---

### calculateAge (8 points)
- [ ] 8 pts - Accurately calculates age accounting for month and day
- [ ] 6 pts - Calculates age but doesn't properly account for whether birthday has occurred
- [ ] 4 pts - Basic year subtraction only
- [ ] 2 pts - Attempts implementation but has errors
- [ ] 0 pts - Not implemented

**Comments:**

---

### isWeekend (4 points)
- [ ] 4 pts - Correctly identifies Saturday and Sunday
- [ ] 2 pts - Partial implementation (only checks one day or has case sensitivity issues)
- [ ] 0 pts - Not implemented or incorrect

**Comments:**

---

### calculateWalkthroughPrice (8 points)
- [ ] 8 pts - All age brackets and weekend/weekday pricing correct
- [ ] 6 pts - Minor error in one age bracket or pricing tier
- [ ] 4 pts - Logic present but multiple pricing errors
- [ ] 2 pts - Attempts conditional logic but significant errors
- [ ] 0 pts - Not implemented

**Comments:**

---

### calculateDriveThroughPrice (6 points)
- [ ] 6 pts - Correctly calculates base + per-person overage
- [ ] 4 pts - Base price correct but overage calculation has error
- [ ] 2 pts - Attempts implementation but has logical errors
- [ ] 0 pts - Not implemented

**Comments:**

---

### applyDiscount (6 points)
- [ ] 6 pts - Correctly checks code and applies 20% discount
- [ ] 4 pts - Discount logic present but calculation error
- [ ] 2 pts - Attempts string comparison but implementation flawed
- [ ] 0 pts - Not implemented

**Comments:**

---

### canAccessAlcohol (6 points)
- [ ] 6 pts - Correctly checks age >= 21 AND not drive-through
- [ ] 4 pts - Checks one condition but not both
- [ ] 2 pts - Attempts implementation but logical error
- [ ] 0 pts - Not implemented

**Comments:**

---

### canRideTrain (8 points)
- [ ] 8 pts - Correctly checks all three conditions (height > 48, weight < 300, not drive-through)
- [ ] 6 pts - Checks two of three conditions correctly
- [ ] 4 pts - Checks one condition correctly
- [ ] 2 pts - Attempts implementation but has errors
- [ ] 0 pts - Not implemented

**Comments:**

---

### generateTicketID (4 points)
- [ ] 4 pts - Generates random 5-digit number (includes leading zeros handling)
- [ ] 3 pts - Generates random number but doesn't handle leading zeros
- [ ] 2 pts - Generates some random value but incorrect format
- [ ] 0 pts - Not implemented or not random

**Comments:**

---

### displayTicket (4 points)
- [ ] 4 pts - Displays all required information clearly formatted
- [ ] 3 pts - Displays all information but minimal formatting
- [ ] 2 pts - Missing some required information
- [ ] 0 pts - Not implemented or minimal output

**Comments:**

---

## Main Method Implementation (20 points)

### Input Collection (8 points)
- [ ] 8 pts - Prompts are clear, all necessary inputs collected in logical order
- [ ] 6 pts - Collects all inputs but prompts could be clearer
- [ ] 4 pts - Missing some inputs or illogical flow
- [ ] 2 pts - Minimal input collection
- [ ] 0 pts - No effective input collection

**Comments:**

---

### Method Calls and Logic Flow (8 points)
- [ ] 8 pts - Calls all methods appropriately with correct parameters
- [ ] 6 pts - Calls most methods correctly with minor parameter issues
- [ ] 4 pts - Some method calls present but significant errors
- [ ] 2 pts - Minimal method integration
- [ ] 0 pts - Methods not properly called from main

**Comments:**

---

### Variable Usage (4 points)
- [ ] 4 pts - Appropriate variables with meaningful names, proper scope
- [ ] 3 pts - Variables used correctly but naming could improve
- [ ] 2 pts - Some variables but organization issues
- [ ] 0 pts - Poor or no variable usage

**Comments:**

---

## Code Quality (10 points)

### Style and Readability (5 points)
- [ ] 5 pts - Consistent indentation, spacing, naming conventions
- [ ] 4 pts - Mostly consistent style with minor issues
- [ ] 3 pts - Readable but inconsistent style
- [ ] 2 pts - Poor style but code works
- [ ] 0 pts - Very poor style affecting readability

**Comments:**

---

### Documentation (5 points)
- [ ] 5 pts - Class header complete, methods have clear comments explaining logic
- [ ] 4 pts - Most documentation present
- [ ] 3 pts - Basic documentation but incomplete
- [ ] 2 pts - Minimal documentation
- [ ] 0 pts - No documentation

**Comments:**

---

## Testing and Correctness (10 points)

### Program Execution (5 points)
- [ ] 5 pts - Runs without errors, handles all input types
- [ ] 4 pts - Runs with minor issues
- [ ] 3 pts - Runs but has some errors during execution
- [ ] 2 pts - Compiles but significant runtime errors
- [ ] 0 pts - Does not compile or run

**Comments:**

---

### Correctness of Output (5 points)
- [ ] 5 pts - All test cases produce correct results
- [ ] 4 pts - Most test cases correct
- [ ] 3 pts - Some test cases correct
- [ ] 2 pts - Minimal correct output
- [ ] 0 pts - Incorrect output

**Test Cases Checked:**
- [ ] Under 2 years old (free)
- [ ] Ages 2-14 (weekday and weekend)
- [ ] Ages 15-17 (weekday and weekend)
- [ ] Adult 18+ (weekday and weekend)
- [ ] Drive-through calculation (under and over 8 people)
- [ ] Discount code applied correctly
- [ ] Train eligibility (edge cases: exactly 48", exactly 300 lbs)
- [ ] Alcohol access (21+ and walkthrough only)
- [ ] Day of week calculation accurate

**Comments:**

---

## Extra Credit (up to 10 points)

### Enhancements (describe what was added):
- [ ] Enhanced ticket formatting (ASCII art, emojis, borders) - up to 2 pts
- [ ] Input validation (date format checking, reasonable values) - up to 2 pts
- [ ] Multiple ticket generation in one run - up to 2 pts
- [ ] File I/O implementation (saves tickets to text file) - up to 5 pts
  - [ ] Correctly writes to file in append mode (2 pts)
  - [ ] Proper file format with all ticket data (2 pts)
  - [ ] Proper exception handling (1 pt)
- [ ] Other creative enhancement: ___________________ - up to 2 pts

**Points Awarded: ______ / 10**

**Comments:**

---

## Overall Comments:

**Strengths:**

**Areas for Improvement:**

**Grade: ______ / 100**
