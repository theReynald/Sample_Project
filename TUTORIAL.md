# Simple Calculator Tutorial

This tutorial will guide you through building a simple calculator web app using HTML, CSS, and JavaScript.

## Step 1: Set up HTML structure and metadata

Create an `index.html` file and add the basic HTML5 structure with proper metadata:
- Set the document type to HTML5
- Add charset and viewport meta tags
- Set the page title to "Simple Calculator"

**File:** `index.html` (lines 1-8)

## Step 2: Style the calculator container

Add CSS to create a centered, modern-looking calculator container:
- Reset default margins and padding
- Center the calculator on the page using flexbox
- Add a gradient purple background
- Style the calculator box with white background, rounded corners, and shadow

**File:** `index.html` (lines 9-32)

## Step 3: Style the display screen

Style the calculator's display area:
- Dark background with white text
- Large font size (2.5rem)
- Right-aligned text
- Rounded corners and adequate padding
- Minimum height and word wrapping for long numbers

**File:** `index.html` (lines 34-44)

## Step 4: Create button grid layout

Set up a CSS Grid layout for the calculator buttons:
- 4 columns of equal width
- 10px gap between buttons

**File:** `index.html` (lines 46-50)

## Step 5: Style individual buttons

Add base styles for all calculator buttons:
- Padding, font size, and border-radius
- Remove default borders
- Add hover and active state animations
- Include cursor pointer and transitions

**File:** `index.html` (lines 52-67)

## Step 6: Style number and operator buttons

Create distinct visual styles for different button types:
- Number buttons: Light gray background
- Operator buttons: Orange background
- Clear button: Red background, spans 2 columns
- Equals button: Green background, spans 2 columns

**File:** `index.html` (lines 69-85)

## Step 7: Create calculator HTML structure

Build the calculator's DOM structure:
- Create a calculator container div
- Add a display div with ID "display"
- Create a buttons container div

**File:** `index.html` (lines 89-91)

## Step 8: Add clear and delete buttons

Add the first row of buttons:
- Clear button (C) that spans 2 columns
- Division operator (/)
- Multiplication operator (×)

**File:** `index.html` (lines 93-95)

## Step 9: Add number buttons (7-9)

Add the second row with numbers 7, 8, 9 and the subtraction operator.

**File:** `index.html` (lines 97-101)

## Step 10: Add number buttons (4-6)

Add the third row with numbers 4, 5, 6 and the addition operator.

**File:** `index.html` (lines 103-107)

## Step 11: Add number buttons (1-3)

Add the fourth row with numbers 1, 2, 3.

**File:** `index.html` (lines 109-112)

## Step 12: Add zero, decimal, and equals buttons

Add the final row:
- Zero button
- Decimal point button
- Equals button (spans 2 columns)

**File:** `index.html` (lines 114-118)

## Step 13: Initialize calculator variables

Set up JavaScript variables to track calculator state:
- `display`: Reference to the display element
- `currentInput`: Current number being entered (starts at '0')
- `operator`: Current operator (+, -, *, /)
- `previousValue`: Previous value for calculations
- `shouldResetDisplay`: Flag to reset display after operation

**File:** `index.html` (lines 123-127)

## Step 14: Function to update display

Create a function to update the display element with the current input value.

**File:** `index.html` (lines 129-131)

## Step 15: Function to append numbers

Create the `appendNumber()` function to handle number button clicks:
- Reset display if needed (after calculation)
- Replace '0' with first digit entered
- Prevent multiple decimal points
- Append the number to current input
- Update the display

**File:** `index.html` (lines 133-146)

## Step 16: Function to handle operators

Create the `appendOperator()` function to handle operator button clicks:
- If an operator already exists and user hasn't entered new number, calculate first
- Store the current value as previous value
- Store the selected operator
- Set flag to reset display on next number entry

**File:** `index.html` (lines 148-154)

## Step 17: Function to perform calculations

Create the `calculate()` function to compute results:
- Check if operation is ready to calculate
- Parse the current value as a number
- Use switch statement to perform appropriate operation
- Handle division by zero error
- Update display with result
- Reset operator and previous value
- Set flag to reset display for next calculation

**File:** `index.html` (lines 156-182)

## Step 18: Function to clear display

Create the `clearDisplay()` function to reset the calculator:
- Reset current input to '0'
- Clear operator and previous value
- Reset display flag
- Update the display

**File:** `index.html` (lines 184-191)

## Step 19: Add keyboard support

Add keyboard event listener for better user experience:
- Numbers and decimal point: Append to display
- Operators (+, -, *, /): Set operator
- Enter or =: Calculate result
- Escape or C: Clear display

**File:** `index.html` (lines 193-206)

---

## How to Run

1. Open `index.html` in any modern web browser
2. Click buttons or use your keyboard to perform calculations
3. Use 'C' or Escape to clear, Enter or '=' to calculate

## Features

- Basic arithmetic operations (addition, subtraction, multiplication, division)
- Decimal number support
- Keyboard input support
- Modern, responsive design
- Visual feedback on button interactions
- Error handling for division by zero

---

## Step-to-Code Map

- **Step 1**: `index.html` (HTML structure setup)
- **Step 2**: `index.html` (CSS: body and .calculator styles)
- **Step 3**: `index.html` (CSS: .display styles)
- **Step 4**: `index.html` (CSS: .buttons grid layout)
- **Step 5**: `index.html` (CSS: button base styles)
- **Step 6**: `index.html` (CSS: .btn-number, .btn-operator, .btn-clear, .btn-equals)
- **Step 7**: `index.html` (HTML: calculator structure)
- **Step 8**: `index.html` (HTML: clear and operator buttons)
- **Step 9**: `index.html` (HTML: number buttons 7-9)
- **Step 10**: `index.html` (HTML: number buttons 4-6)
- **Step 11**: `index.html` (HTML: number buttons 1-3)
- **Step 12**: `index.html` (HTML: 0, decimal, equals buttons)
- **Step 13**: `index.html` (JS: variable initialization)
- **Step 14**: `index.html` (JS: `updateDisplay()` function)
- **Step 15**: `index.html` (JS: `appendNumber()` function)
- **Step 16**: `index.html` (JS: `appendOperator()` function)
- **Step 17**: `index.html` (JS: `calculate()` function)
- **Step 18**: `index.html` (JS: `clearDisplay()` function)
- **Step 19**: `index.html` (JS: keyboard event listener)
