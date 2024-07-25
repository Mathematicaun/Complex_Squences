# Complex Point Distribution on Unit Circle

This repository contains a Python script that visualizes the distribution of complex points on the unit circle. The script uses Matplotlib to plot the sequence generated by iterating a complex function \( F(z) = z^2 + c \) over the complex plane, with interactive mouse support to update the sequence dynamically.

## Files

- `Scene.py`: The main Python script that generates and visualizes the complex point distribution.

## Requirements

- Python 3.x
- Matplotlib
- NumPy

You can install the required packages using pip:

```bash
pip install matplotlib numpy
```

## Usage

To run the script, execute the following command in your terminal:

```bash
python Scene.py
```

Once the script is running, a window will open displaying the unit circle. You can move your mouse over the plot to dynamically update the sequence of complex points.

## How it Works

The script performs the following steps:

1. Sets up the plot using Matplotlib with a dark background style.
2. Defines the complex function \( F(z) = z^2 + c \), where \( c \) is a user-defined constant.
3. Plots the unit circle.
4. Defines a function `Seq` that:
    - Clears the current plot.
    - Plots the unit circle.
    - Sets up the plot limits and labels.
    - Iteratively computes and plots the sequence of points starting from an initial complex number.
5. Defines a `mouse` function to capture mouse movements and update the sequence dynamically.
6. Connects the `mouse` function to the Matplotlib plot to handle mouse events.
7. Initializes the plot with the first point at the origin.

## Customization

You can customize the script by changing the following parameters:
- `depth`: Number of divisions for the plot axes.
- `points`: Number of points in the sequence to plot.
- `a`, `b`: Real and imaginary parts of the constant \( c \).
