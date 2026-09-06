# Growing Code - Python Fundamentals Through Garden Data

## Overview
**Growing Code** is an introductory Python module designed to cover core programming syntax, control flow, functions, and basic type annotations using community garden data as a context.

The goal of this project is to build a foundational understanding of Python 3.10+, adhering to clean code standards and strict functional structures without relying on standalone script execution blocks.

---

## Technical Requirements & Guidelines

* **Language:** Python 3.10+
* **Code Style:** Must strictly follow the `flake8` linter standard.
* **Type Hinting:** Mandatory for Exercise 07 (`mypy` compliant). Optional for Exercises 00 to 06.
* **Execution Rules:** 
  * Write **only** the requested functions.
  * No `if __name__ == "__main__":` blocks or global code execution outside functions.
  * Inputs and outputs are handled directly within the specified functions using `input()` and `print()`.

---

## Exercises Summary

| Exercise | Directory | Submitted File(s) | Function Name | Description |
| :--- | :--- | :--- | :--- | :--- |
| **Ex 00** | `ex00/` | `ft_hello_garden.py` | `ft_hello_garden()` | Displays a basic welcome message to the community. |
| **Ex 01** | `ex01/` | `ft_garden_name.py` | `ft_garden_name()` | Takes a garden name input and outputs it with status. |
| **Ex 02** | `ex02/` | `ft_plot_area.py` | `ft_plot_area()` | Calculates plot area based on length and width inputs. |
| **Ex 03** | `ex03/` | `ft_harvest_total.py` | `ft_harvest_total()` | Sums three daily harvest input values. |
| **Ex 04** | `ex04/` | `ft_plant_age.py` | `ft_plant_age()` | Checks if a plant is ready to harvest based on days. |
| **Ex 05** | `ex05/` | `ft_water_reminder.py` | `ft_water_reminder()` | Determines watering status based on elapsed days. |
| **Ex 06** | `ex06/` | `ft_count_harvest_iterative.py`<br>`ft_count_harvest_recursive.py` | `ft_count_harvest_iterative()`<br>`ft_count_harvest_recursive()` | Countdown to harvest using iterative and recursive approaches. |
| **Ex 07** | `ex07/` | `ft_seed_inventory.py` | `ft_seed_inventory(...)` | Manages inventory displays using strict Python type annotations. |

---

## Exercise Details

### Exercise 00: Hello Garden
* **Concepts:** Basic function definition, standard output (`print`).
* **Details:** Prints `"Hello, Garden Community!"`. Takes no arguments and handles output directly.

### Exercise 01: Garden Name
* **Concepts:** Basic I/O (`input`, `print`), string formatting.
* **Details:** Prompts for a garden name, then prints the entered name along with a static status message: `"Status: Growing well!"`.

### Exercise 02: Garden Plot Area
* **Concepts:** Type conversion (`str` to `int`), basic arithmetic.
* **Details:** Prompts for length and width as integers, multiplies them, and displays the total rectangular plot area.

### Exercise 03: Harvest Total
* **Concepts:** Accumulation, multi-input handling.
* **Details:** Prompts for daily harvest quantities over 3 separate days, sums them up, and prints the total weight.

### Exercise 04: Plant Age Check
* **Concepts:** Conditional statements (`if`/`else`), strict relational operator (`>`).
* **Details:** Prompts for plant age in days. Prints `"Plant is ready to harvest!"` if age is strictly greater than 60, otherwise prints `"Plant needs more time to grow."`.

### Exercise 05: Water Reminder
* **Concepts:** Conditional logic, threshold checking.
* **Details:** Prompts for days since last watering. Prints `"Water the plants!"` if strictly more than 2 days have passed, otherwise prints `"Plants are fine"`.

### Exercise 06: Count to Harvest
* **Concepts:** Iteration (`range`), Recursion call stacks, base cases.
* **Details:** Takes target days until harvest and counts up from `1` to $N$, printing `"Day X"` for each step, ending with `"Harvest time!"`. Implemented separately via iteration and recursion.

### Exercise 07: Seed Inventory with Type Annotations
* **Concepts:** Static type hints (`mypy`), string methods (`capitalize`), parameter handling.
* **Details:** Accepts arguments `(seed_type: str, quantity: int, unit: str) -> None`. Formats output based on unit (`"packets"`, `"grams"`, `"area"`). Prints `"Unknown unit type"` for unsupported units.

---

## Testing & Quality

### Testing with `main.py`
Run the helper test script in your project environment:
```bash
python3 main.py
