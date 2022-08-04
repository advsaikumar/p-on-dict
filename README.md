n=int(input("enter the number of students:"))
d={}
for i in range(n):
    name=input("enter student name:")
    marks=input("enter student marks:")
    d[name]=marks
while True:
    name=input("enter student name to get marks:")
    marks=d.get(name,-1)
    if marks==-1:
        print("student not found")
    else:
        print("the marks of",name,"are",marks)
    option=input("Do you want to find another student marks[Yes|No]")
    if option=='no':
        break
print("Thanks for using our application")
