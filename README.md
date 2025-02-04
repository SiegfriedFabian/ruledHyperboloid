# Ruled Hyperboloid Generator

Creates a hyperboloid surface using straight lines (ruled surface) in Blender.

## Parameters

- `radius` (default: 2): Radius of top and bottom rings
- `height` (default: 4): Vertical distance between rings
- `twist` (default: 0.0): Angular rotation between top and bottom connections
- `num_lines` (default: 25): Number of ruled lines
- `ring_thickness` (default: 0.1): Thickness of boundary rings
- `line_thickness` (default: 0.08): Thickness of ruled lines
- `smoothness` (default: 2): Controls subdivision and bevel quality (1-4)
- `double_ruled` (default: False): Creates crossed lines when True

## Example Usage

```python
# Simple hyperboloid with slight twist
create_hyperboloid(height=10, twist=0.5)

# Double-ruled hyperboloid with high smoothness
create_hyperboloid(
    radius=2,
    height=8,
    twist=1.0,
    smoothness=3,
    double_ruled=True
)

# Dense lattice structure
create_hyperboloid(
    num_lines=40,
    twist=0.8,
    line_thickness=0.05,
    double_ruled=True
)
```