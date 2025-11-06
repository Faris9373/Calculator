1️⃣ Overall Plan for the Calculator

We’ll build it in layers:

Phase 1 – HTML (structure only)
Goal: Get the layout of the calculator on the page.

- Make a main container: .calculator

- Add a display area (where numbers & results show)

- Add buttons for:
digits: 0–9
operations: + - × ÷
clear: C
equals: =
decimal: .

Give buttons useful classes / attributes for JS later, like:

- .btn-number

- .btn-operator

- .btn-equals

- .btn-clear

- No styling, no logic yet. Just the skeleton.

Phase 2 – CSS (make it look nice)
Goal: Make it look like a clean modern calculator.

- Center the calculator on the page

- Give it a nice background, border-radius, shadow

- Use CSS Grid or Flexbox for the button layout

- Make it responsive so it doesn’t look broken on smaller screens

Phase 3 – JS (make it actually work)
Goal: Make it calculate properly.
Steps for the logic:

- Select the display and buttons with document.querySelector / querySelectorAll

- When a number button is clicked → append it to the display

- When an operator is clicked → store:

- current number

- which operator

- When = is pressed → perform the calculation and show result

- When C is pressed → clear everything

- Handle edge cases:

- Division by zero

- Pressing multiple operators

- Pressing = multiple times

- Extra: Keyboard support (numbers and + - * / Enter)