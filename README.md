# Java Calculator

A lightweight Java calculator library that supports both binary and unary operations. This package provides a `Calculator` class with methods for basic arithmetic, trigonometric functions, powers, logarithms, percentages, and other common calculations.

---

## Features

### Binary Operations
- Addition (`add`)
- Subtraction (`minus`)
- Multiplication (`multiply`)
- Division (`divide`)
- Power (`xpowerofy`)

### Unary Operations
- Square (`square`)
- Square root (`squareRoot`)
- Reciprocal (`oneDividedBy`)
- Cosine (`cos`)
- Sine (`sin`)
- Tangent (`tan`)
- Base-10 logarithm (`log`)
- Percentage (`rate`)
- Absolute value (`abs`)

---

## Installation

Clone or download this repository and include it in your Java project.

```bash
git clone https://github.com/yourusername/simplejavacalculator.git

Compile the package:

javac -d . src/simplejavacalculator/Calculator.java


⸻

Usage

import simplejavacalculator.Calculator;
import simplejavacalculator.Calculator.BiOperatorModes;
import simplejavacalculator.Calculator.MonoOperatorModes;

public class Main {
    public static void main(String[] args) {
        Calculator calc = new Calculator();

        // Binary operations
        Double result = calc.calculateBi(BiOperatorModes.add, 10.0);
        result = calc.calculateBi(BiOperatorModes.multiply, 5.0);
        System.out.println("Result: " + calc.calculateEqual(0.0)); // Outputs 50.0

        // Unary operations
        double square = calc.calculateMono(MonoOperatorModes.square, 7.0);
        double sinValue = calc.calculateMono(MonoOperatorModes.sin, 30.0);

        System.out.println("Square: " + square);
        System.out.println("Sine: " + sinValue);
    }
}


⸻

Methods

calculateBi(BiOperatorModes mode, Double num)

Performs binary operations. Returns NaN if starting a new operation or the result if continuing a calculation.

calculateEqual(Double num)

Completes the current binary operation and returns the result.

calculateMono(MonoOperatorModes mode, Double num)

Performs unary operations and returns the calculated value.

reset()

Resets the calculator state to initial values.

⸻

Technologies Used
	•	Language: Java
	•	Math Libraries: java.lang.Math
	•	Development Environment: IntelliJ IDEA / VS Code / Eclipse

