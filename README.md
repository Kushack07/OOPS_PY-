# OOPS-

oops -object oriented programming
#student detail 

#using the list
stud_1 = ['madav', 10]   # name, age
stud_2 = ['vishnaka', 12]
stud_3 = 'kush'

stud_1.append('A')
print(stud_1)

# Using OOPs - creating student records

# Class = blueprint/template
class Student:
    name = 'kush'
    grade = 10

# Object = instance of class
student1 = Student()

print(student1.name, student1.grade)

# Now we will use functions inside class

class Student: #student class
        def __init__(self, full_name, c_grade, percentage,age): #method
        self.name = full_name   #attributes 
        self.grade = c_grade    #attribute
        self.percentage = percentage
        self.age = age
        

    # Method
    def stud_details(self):
        print(f"{self.name} is in class {self.grade}")

# Create objects
student_1 = Student('Kush', 11, 99,21)
print(student_1.name, student_1.grade,student_1.age)

student_2 = Student('Luv', 11, 96,21)
print(student_2.name, student_2.grade,student_2.age)

student_3 = Student('Dilip', 13, 97,56)
print(student_3.name, student_3.grade, student_3.percentage,student_3.age)

# Calling method
student_1.stud_details()
student_3.stud_details()
student_2.stud_details()


# Modify object property
student_1.percentage = 89
print(student_1.percentage)

# Object dictionary
print(student_1.__dict__)

# Delete object
del student_1

# print(student_1)  # This will give error because object is deleted 
