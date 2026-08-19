# Fractal Implementation — Sierpiński Triangle

A Python implementation of the **Sierpiński Triangle**, a fractal that demonstrates self-similarity through repeated subdivision of a triangle.

This project contains two implementations of the fractal:

1. A recursive implementation using Python's built-in `turtle` graphics module.
2. A PyTorch implementation that uses vectorised tensor operations to calculate the fractal across a two-dimensional grid.

---

## Files

- `fractal.ipynb` — Recursive Sierpiński Triangle implementation using Turtle.
- `sierpinski_pytorch.ipynb` — PyTorch implementation using tensor operations and hardware acceleration where available.
- `AI_PROMPT.txt` — Summary of AI assistance used during development.
- `README.md` — Project documentation.

---

## 1. Recursive Turtle Implementation

The `fractal.ipynb` notebook demonstrates the geometric construction of the Sierpiński Triangle using recursion.

The implementation contains three main functions:

### `draw_triangle(points, colour)`

Draws and fills a triangle using three coordinate points.

### `midpoint(point1, point2)`

Calculates the midpoint between two points by averaging their x and y coordinates.

### `sierpinski(points, degree)`

Recursively divides the original triangle into three smaller corner triangles.

For each recursion level:

1. The current triangle is drawn.
2. Midpoints of the edges are calculated.
3. Three smaller triangles are created:
   - top
   - bottom-left
   - bottom-right
4. The function calls itself for each smaller triangle.
5. The recursion stops when `degree` reaches zero.

The recursion depth can be changed using:

```python
degree = 5