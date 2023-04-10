# shapes_python
import math


def circle_area(radius):
    return math.pi * radius ** 2


def circle_perimeter(radius):
    return 2 * math.pi * radius


def rectangle_area(length, width):
    return length * width


def rectangle_perimeter(length, width):
    return 2 * (length + width)


def triangle_area(base, height):
    return 0.5 * base * height


def triangle_perimeter(side1, side2, side3):
    return side1 + side2 + side3


shape = input("Enter the shape (circle, rectangle, triangle): ")



if shape == "circle":
    radius = float(input("Enter the radius of the circle: "))
    area = circle_area(radius)
    perimeter = circle_perimeter(radius)
    print(f"The area of the circle is {area:.2f} and the perimeter is {perimeter:.2f}.")
elif shape == "rectangle":
    length = float(input("Enter the length of the rectangle: "))
    width = float(input("Enter the width of the rectangle: "))
    area = rectangle_area(length, width)
    perimeter = rectangle_perimeter(length, width)
    print(f"The area of the rectangle is {area:.2f} and the perimeter is {perimeter:.2f}.")
elif shape == "triangle":
    base = float(input("Enter the base of the triangle: "))
    height = float(input("Enter the height of the triangle: "))
    side1 = float(input("Enter the length of side 1 of the triangle: "))
    side2 = float(input("Enter the length of side 2 of the triangle: "))
    side3 = float(input("Enter the length of side 3 of the triangle: "))
    area = triangle_area(base, height)
    perimeter = triangle_perimeter(side1, side2, side3)
    print(f"The area of the triangle is {area:.2f} and the perimeter is {perimeter:.2f}.")
else:
    print("Invalid shape selected.")
