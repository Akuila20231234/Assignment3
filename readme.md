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
Greetings! This is the final code I will go over and it is the longest out of the three. Its very long because it covers 5 different principles and is all incorporated into one. I am referring to the "SOLID" principle. With this final code I will share where these 5 different principles will be present and explain what each role they play. 
# Single Responsibility Principle:
With this principle it is important that each class should have only one responsibility or job. As you can see each class is seperate and focus on a single task. Firstly, we have a class named "Ticket" which helps the user create the tickets. Secondly, the next class is under "HelpDesk" and that will focus on the different functions in your ticketing system. Afterwards, the user will have the last class assigned as your main, so the code may run and view the tickets the user has created. 
# Open/Closed Principle: 
This priniciple focuses on the whether your code is open for extensions but closed for modification. This means that you should write code that can be extended with new functionality, without having to modify the existing code. Again, we refer back to the classes we talked about earlier. In the first class, the "Ticket" class, we mentioned that is was used to create the tickets, well the second class ("HelpDesk") helps modify those tickets. 
# Liskov Substitution Principle
This principle is for code such as subtypes to be substitued in place of their parent types without causing any issues. Like for instance, when submitting tickets this method creates a new Ticket within the first class with the given parameters and subs it to the tickets list.
# Interface Segregation Principle
The whole idea behind the ISP principle is to provide the smallest number of methods in a class. This leads to focused definitions, often seperating a design into mulitple classes to isolate the imapct of any changes. For example, the user must then have another class to focus on the different functions in your ticketing system and have everything run through that main class. Set that as "class HelpDesk". This class will help you represent the entire helpdesk system. This class will cover how you will create tickets, display tickets, reopen tickets, respond to tickets, as well as display the statistics of those tickets.  
# Dependency Inverion Principle
This method or principle is the last one and it focuses on the abstractions of your code and how it should not depend upon the details. Instead the details should depend upon the abstractions. So what does that mean? When displaying statistics of the users tickets we can assign "HelpDesk" instead of "stats" to provide the interface to use in your concrete classes, like so: 
def display_statistics(self):
        stats=["total tickets, resolved tickets, open tickets"]
        print("total ticket number: ", len(self.helpdesk))
# Conclusion 
That is it for all three of the codes, these principles will help ensure that your code is maintainable, extensible, and testable and it has really helped me out. So, thank you so much for coming along and viewing my readme!
