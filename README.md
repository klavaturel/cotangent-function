# cotangent-function
import math

def cotangent(angle):
    """Calculate the cotangent of an angle in radians."""
    if math.tan(angle) == 0:
        return float('inf')  # Handle division by zero
    return 1 / math.tan(angle)

# Example usage
def main():
    angles = [math.radians(30), math.radians(45), math.radians(60), math.radians(90)]
    for angle in angles:
        print(f"Cotangent of {math.degrees(angle):.0f} degrees: {cotangent(angle)}")

if __name__ == "__main__":
    main()
