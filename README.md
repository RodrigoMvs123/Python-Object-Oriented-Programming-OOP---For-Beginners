# Python-Object-Oriented-Programming-OOP---For-Beginners

https://youtu.be/JeznW_7DlB0 

https://raw.githubusercontent.com/RodrigoMvs123/Python-Object-Oriented-Programming-OOP---For-Beginners/main/README.md



Visual Studio Code
Explorer 
OPEN EDITORS
OOP
oop0.py 

oop0.py
x = 1
print(type("hello"))

Visual Studio Code
Explorer 
OPEN EDITORS
OOP
oop1.py 

oop1.py
def hello():
    print("hello")

x = 1 
print(type("hello"))

Visual Studio Code
Explorer 
OPEN EDITORS
OOP
oop2.py 

oop2.py
x = 1
y = "hello"

print(x + y)

Visual Studio Code
Explorer 
OPEN EDITORS
OOP
oop3.py 

oop3.py
x = 1 
y = 2
x + y

Visual Studio Code
Explorer 
OPEN EDITORS
OOP
oopMethod0.py

oopMethod0.py
string = "hello"
print(string.upper())

Visual Studio Code
Explorer 
OPEN EDITORS
OOP
oopMethod1.py

oopMethod1.py
string = "hello"
x = 1
print(x.upper())

Visual Studio Code
Explorer 
OPEN EDITORS
OOP
oopMethod2.py

oopMethod2.py
class Dog:
    def bark(self):
        print("bark")

d = Dog()
print(type(d))

Visual Studio Code
Explorer 
OPEN EDITORS
OOP
oopMethod3.py

oopMethod3.py
class Dog:
    def bark(self):
        print("bark")

d = Dog()
d.bark()
print(type(d))

Visual Studio Code
Explorer 
OPEN EDITORS
OOP
oopMethod4.py

oopMethod4.py
class Dog:

    def add_one(self, x): 
        return x + 1

    def bark(self):
        print("bark")

d = Dog()
d.bark()
print(d.add_one(5))
print(type(d))

Visual Studio Code
Explorer 
OPEN EDITORS
OOP
oopMethod5.py

oopMethod5.py
class Dog:

    def __init__(self, name):
        self.name = name
        print(name)

    def add_one(self, x): 
        return x + 1

    def bark(self):
        print("bark")

d = Dog("Tim")
d2 = Dog("Bill")

Visual Studio Code
Explorer 
OPEN EDITORS
OOP
oopMethod6.py

oopMethod6.py
class Dog:

    def __init__(self, name):
        self.name = name
        
    def add_one(self, x): 
        return x + 1

    def bark(self):
        print("bark")

d = Dog("Tim")
print(d.name)
d2 = Dog("Bill")
print(d2.name)

Visual Studio Code
Explorer 
OPEN EDITORS
OOP
oopMethod7.py

oopMethod7.py
class Dog:

    def __init__(self, name, age):
        self.name = name
        self.age = age
        
    def get_name(self):
        return self.name

d = Dog("Tim", 34)
print(d.get_name)
d2 = Dog("Bill", 12)
print(d2.get_name)

Visual Studio Code
Explorer 
OPEN EDITORS
OOP
oopMethod8.py

oopMethod8.py
class Dog:

    def __init__(self, name, age):
        self.name = name
        self.age = age
        
    def get_name(self):
        return self.name

    def get_age(self):
        return self.age

d = Dog("Tim", 34)
print(d.get_age())
d2 = Dog("Bill", 12)
print(d2.get_age())

Visual Studio Code
Explorer 
OPEN EDITORS
OOP
oopMethod9.py

oopMethod9.py
class Dog:

    def __init__(self, name, age):
        self.name = name
        self.age = age
        
    def get_name(self):
        return self.name

    def get_age(self):
        return self.age
    
    def set_age(self, age):
        self.age = age 

d = Dog("Tim", 34)
d.set_age(23)
print(d.get_age())

Visual Studio Code
Explorer 
OPEN EDITORS
OOP
oopMethod10.py

oopMethod10.py
class Student:
    def __init__(self, name, age, grade):
        self.name = name
        self.age = age
        self.grade = grade # 0 - 100

    def get_grade(self):
        return self.grade
    
class Course:
    def __init__(self, name, max_students):
        self.name = name
        self.max_students = max_students
        self.students = []

    def add_student(self, student):
        if len(self.students) < self.max_students:
            self.students.append(student)
            return True
        return False 
    
    def get_avarage_grade(self):
        pass

s1 = Student("Tim", 19, 95)
s2 = Student("Bill", 19, 75)
s3 = Student("Jill", 19, 65)

course = Course("Science", 2)
course.add_student(s1)
course.add_student(s2)
print(course.students[0].name)

Visual Studio Code
Explorer 
OPEN EDITORS
OOP
oopMethod11.py

oopMethod11.py
class Student:
    def __init__(self, name, age, grade):
        self.name = name
        self.age = age
        self.grade = grade # 0 - 100

    def get_grade(self):
        return self.grade
    
class Course:
    def __init__(self, name, max_students):
        self.name = name
        self.max_students = max_students
        self.students = []

    def add_student(self, student):
        if len(self.students) < self.max_students:
            self.students.append(student)
            return True
        return False 
    
    def get_avarage_grade(self):
        value = 0
        for student in self.students:
            value += student.get_grade()

            return value / len(self.students)

s1 = Student("Tim", 19, 95)
s2 = Student("Bill", 19, 75)
s3 = Student("Jill", 19, 65)

course = Course("Science", 2)
course.add_student(s1)
course.add_student(s2)
print(course.get_avarage_grade())

Visual Studio Code
Explorer 
OPEN EDITORS
Inheritance
Inheritance0.py

Inheritance0.py
class Cat:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def speak(self):
        print("Meow")

class Dog:
    def __init__(self, name, age):
        self.name = name
        self.age = age
    
    def speak(self):
        print("Bark")

Visual Studio Code
Explorer 
OPEN EDITORS
Inheritance
Inheritance1.py

Inheritance1.py
class Pet:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def show(self):
        print(f"I am {self.name} and I am {self.age} years old")

class Cat(Pet):
    def __init__(self, name, age):
        self.name = name
        self.age = age

class Dog(Pet):
    def __init__(self, name, age):
        self.name = name
        self.age = age

p = Pet("Tim", 19)
p.show()
c = Cat("Bill", 34)
c.show()
d = Dog("Jill", 25)
d.show()

Visual Studio Code
Explorer 
OPEN EDITORS
Inheritance
Inheritance2.py

Inheritance2.py
class Pet:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def show(self):
        print(f"I am {self.name} and I am {self.age} years old")
    
    def speak(self):
        print(" I do not know what to say")

class Cat(Pet):
    def speak(self):
        print("Meow")

class Dog(Pet):
    def speak(self):
        print("Bark")

p = Pet("Tim", 19)
p.speak()
c = Cat("Bill", 34)
c.speak()
d = Dog("Jill", 25)
d.speak()

Visual Studio Code
Explorer 
OPEN EDITORS
Inheritance
Inheritance3.py

Inheritance3.py
class Pet:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def show(self):
        print(f"I am {self.name} and I am {self.age} years old")
    
    def speak(self):
        print(" I do not know what to say")

class Cat(Pet):
    def speak(self):
        print("Meow")

class Dog(Pet):
    def speak(self):
        print("Bark")

class Fish(Pet):
    pass

p = Pet("Tim", 19)
p.speak()
c = Cat("Bill", 34)
c.speak()
d = Dog("Jill", 25)
d.speak()
f = Fish("Bubbles", 10)
f.speak()

Visual Studio Code
Explorer 
OPEN EDITORS
Inheritance
Inheritance4.py

Inheritance4.py
class Pet:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def show(self):
        print(f"I am {self.name} and I am {self.age} years old")
    
    def speak(self):
        print("I do not know what to say")

class Cat(Pet):
    def __init__(self, name, age, color):
        super().__init__(name, age)
        self.color = color

    def speak(self):
        print("Meow")
    
    def show(self):
        print(f"I am {self.name} and I am {self.age} years old and I am {self.color}")

class Dog(Pet):
    def speak(self):
        print("Bark")

p = Pet("Tim", 19)
p.speak()
c = Cat("Bill", 34, "Brown")
c.show()
d = Dog("Jill", 25)
d.speak()


Visual Studio Code
Explorer 
OPEN EDITORS
ClassAttributes
ClassAttributes0.py

ClassAttributes0.py
class Person:
    number_of_people = 0

    def __init__(self, name):
        self.name = name
    
p1 = Person("Tim")
p2 = Person("Jill")

Person.number_of_people = 8
print(p2.number_of_people)
print(p1.number_of_people)

Visual Studio Code
Explorer 
OPEN EDITORS
ClassAttributes
ClassAttributes1.py

ClassAttributes1.py
class Person:
    number_of_people = 0

    def __init__(self, name):
        self.name = name
        Person.number_of_people += 1
    
p1 = Person("Tim")
print(Person.number_of_people)
p2 = Person("Jill")
print(Person.number_of_people)

Visual Studio Code
Explorer 
OPEN EDITORS
ClassAttributes
ClassAttributes2.py

ClassAttributes2.py
class Person:
    number_of_people = 0
    GRAVITY = -9.8

    def __init__(self, name):
        self.name = name
        Person.add_person()

    @classmethod   
    def number_of_people_(cls):
        return cls.number_of_people
    
    @classmethod
    def add_person(cls):
        cls.number_of_people += 1

p1 = Person("Tim")
p2 = Person("Jill")
print(Person.number_of_people_())

Visual Studio Code
Explorer 
OPEN EDITORS
StaticMethods
StaticMethods0.py

StaticMethods0.py
class Math:

    @staticmethod
    def add5(x):
        return x + 5
    
    @staticmethod
    def add10(x):
        return x + 10
    
    @staticmethod
    def pr():
        print("run")
    
Math.pr()









   











