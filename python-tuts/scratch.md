# Classes

    class Rectangle:
        def __init__(self, width, height):
            self.width = width
            self.height = height

        def area(self):
            return self.width * self.height

        def perimeter(self):
            return 2 * (self.width + self.height)

        def to_string(self):
            return 'Rectangle: width={0}, height={1}'.format(self.width, self.height)

        def __str__(self):
            """string version of object"""
            return 'Rectangle: width={0}, height={1}'.format(self.width, self.height)

        def __repr__(self):
            """Represent how object was built"""
            return 'Rectangle({0}, {1}'.format(self.width, self.height)

        def __eq__(self, other):
            """If equal?"""
            return self.width = other.width and self.height = other.height

    r1 = Rectangle(10, 20)
    r1.area()
    r1.to_string()
    str(r1)



