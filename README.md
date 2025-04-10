# field-length-measurement
import math

def calculate_field_length(area, width):
    """Calculate the length of a field given its area and width."""
    if width <= 0:
        return "Width must be greater than zero!"
    return area / width

def calculate_field_diagonal(length, width):
    """Calculate the diagonal of a rectangular field."""
    return math.sqrt(length**2 + width**2)

# Example usage
area = 5000  # Square meters
width = 50  # Meters
length = calculate_field_length(area, width)
diagonal = calculate_field_diagonal(length, width)

print(f"Field Length: {length} meters")
print(f"Field Diagonal: {diagonal:.2f} meters")
