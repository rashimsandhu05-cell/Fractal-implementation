# Fractal Implementation — Sierpiński Triangle

A Python implementation of the **Sierpiński triangle**, a fractal made from a
triangle that is repeatedly divided into three smaller triangles. The project
uses recursion and Python's built-in `turtle` graphics module to render the
pattern.

## Files

- `fractal.ipynb` — the main notebook containing the implementation.
- `Sierpiński Triangle.ipynb` — a placeholder notebook for related work.
- `AI_PROMPT.txt` — a summary of AI prompts used for the COMP3710 Part 3 work.

## How it works

The notebook defines three main functions:

- `draw_triangle(points, colour)` draws and fills a triangle using three points.
- `midpoint(point1, point2)` calculates the centre point of an edge.
- `sierpinski(points, degree)` recursively draws the three smaller triangles
  that form each level of the fractal.

The starting triangle has vertices at `(-300, -250)`, `(0, 300)`, and
`(300, -250)`. The recursion depth is set by the `degree` variable, which is
currently `5`.

## Requirements

- Python 3
- A desktop environment that supports Tk/Turtle graphics
- Jupyter Notebook or Visual Studio Code with Jupyter support

No third-party Python packages are required.

## Running the project

1. Open `fractal.ipynb` in Jupyter Notebook or VS Code.
2. Run the code cell.
3. A Turtle graphics window will open and draw the Sierpiński triangle.

To change the amount of detail, edit the following line in the notebook:

```python
degree = 5
```

Larger values create more detail but require more drawing time. For example,
`degree = 6` creates 729 smallest triangles.

## Notes

The Turtle window needs a graphical desktop session. It may not open when the
notebook is run on a headless server or in some browser-only notebook services.
