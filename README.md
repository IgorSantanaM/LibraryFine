# Library Fine Calculator

## Problem Statement

This program calculates the fine for a book returned to a library based on the expected and actual return dates. The fine structure is as follows:

- **No fine**: If the book is returned on or before the expected return date.
- **Daily fine**: If the book is returned after the expected return date but within the same calendar month and year, a fine of 15 units for each day late is charged.
- **Monthly fine**: If the book is returned after the expected return month but within the same calendar year, a fine of 500 units for each month late is charged.
- **Fixed fine**: If the book is returned after the calendar year in which it was due, a fixed fine of 10,000 units is charged.

## Function Description

```python
def libraryFine(d1, m1, y1, d2, m2, y2):
```
# Parameters:
`d1, m1, y1`: Integers representing the day, month, and year when the book was returned.
`d2, m2, y2`: Integers representing the day, month, and year when the book was due.
# Returns:
An integer representing the total fine based on the return date.
# Input Format:
The first line contains three space-separated integers: d1 (day), m1 (month), y1 (year) representing the return date.
The second line contains three space-separated integers: d2 (day), m2 (month), y2 (year) representing the due date.
# Constraints:
The returned date and the due date will always be valid dates in the Gregorian calendar.
