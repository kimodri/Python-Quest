# Super Function

Inheritance is easy but again, Kim, when you deal with their constructors, that's when they get complicated. Let's take the first problem as an example:

`university.py`
```python
# Person must have name and age attribute 
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age
    

class Student(Person):
    def __init__(self, name, age, major, GPA):
        super().__init__(name, age)
        self.major = major
        self.GPA = GPA


# class Faculty(Person):
#     def __init__(self, name, age, department, rank):
#         super().__init__(name, age)
#         self.department = department
#         self.rank = rank
    
# class Parttimer(Student, Faculty):
#     def __init__(self, name, age,  major, GPA, department, rank):
#         super().__init__() # we need to rethink this
```