# 1st Code: DRY Principle
Hello! Welcome to the project, this is one of the three principles I will cover. Starting first is a simple one called the "DRY Principle" and how to use it. First of all the main focus of this principle is to avoid duplication of code. It means that you should write code that can be reused, rather than copying and pasting the same thing over and over. 
# Instructions:
1. Choose a shape
2. List out the dimensions of that shape to calculate the area
3. After listing write a simple code to calculate the area
4. Add in numbers to terminal when requested
5. Print and view results in the terminal
Just a reminder you can implent all the dimensions (i.e Length, Width) in one line of code like so:
def calculate_area(length,width):
*you will most likely need to crunch in some numbers to the terminal in order to run the code
Listing it like this is tedious and unnecessary:
width=10
length=5
area=width*length

# Example of DRY Principle:
*my own code*
Oringial Code:
width=10
length=5
area=width*length
print(area)

New Code:
def calculate_area(length,width):
    return length *width

# 2nd Code: Separation of Concerns Principle
Welcome! This is another code that I will go over, this time referring to the principle "Separation of Concerns". The whole purpose of this principle is to divide your code into distinct and independent parts, each with a specific concern or responsibility. For this example, I will be using a code we used in class, with the use of the "import turtle" syntax. Its longer than the previous code but don't worry its very simple and easy to understand. 
# Instructions: 
1. Choose a shape (In this case I chose a square) *The sides of a square come at a 90 degree angle on all four corners*
2. Use OOP to classify what each class does
3. Add a function to have a color of your choosing to outline your shape
4. Create a function to draw the shpae 
5. Call the function
# Example of SoC Principle: 
*not my code* 
class Shape:
    def __init__(self, color):
        self.t = turtle.Turtle()
        self.t.color(color)

class square(Shape):
    def __init(self,color,side_length):
        super().__init__(color)
        self.side_length = side_length

    def draw(self):
        for i in range(2):
            self.t.forward(self.side_length)
            self.t.right(90)
            self.t.forward(self.side_length)
            self.t.right(90)

# 3rd Code: SOLID Principle 
