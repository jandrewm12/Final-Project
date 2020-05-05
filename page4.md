# INFOTC 1000 Final Project
## Page 4
![mountain banner](https://cdn.pixabay.com/photo/2017/03/31/16/11/banner-2191712_960_720.jpg)

I also *love* food! My favorite place to eat is [Shake Shack](https://www.shakeshack.com/)!
![Shake Shack](shakeshack.jpg)

Their burgers and fries (and shakes!) are **delicious**!

I also like to eat at other fast food places, like:
- McDonald's
- Chick-Fil-A
- Burger King


---

Here's yet *another* snippet of code from class:

```
# gradebook.py

# Display the average of each student's grade.
# Display tthe average for each assignment.

gradebook = [[61, 74, 69, 62, 72, 66, 73, 65, 60, 63, 69, 63, 62, 61, 64],
             [73, 80, 78, 76, 76, 79, 75, 73, 76, 74, 77, 79, 76, 78, 72],
             [90, 92, 93, 92, 88, 93, 90, 95, 100, 99, 100, 91, 95, 99, 96],
             [96, 89, 94, 88, 100, 96, 93, 92, 94, 98, 90, 90, 92, 91, 94],
             [76, 76, 82, 78, 82, 76, 84, 82, 80, 82, 76, 86, 82, 84, 78],
             [93, 92, 89, 84, 91, 86, 84, 90, 95, 86, 88, 95, 88, 84, 89],
             [63, 66, 55, 67, 66, 68, 66, 56, 55, 62, 59, 67, 60, 70, 67],
             [86, 92, 93, 88, 90, 90, 91, 94, 90, 86, 93, 89, 94, 94, 92],
             [89, 80, 81, 89, 86, 86, 85, 80, 79, 90, 83, 85, 90, 79, 80],
             [99, 73, 86, 77, 87, 99, 71, 96, 81, 83, 71, 75, 91, 74, 72]]

#determines number of assignments
num_of_assignments = len(gradebook[0])

#main function
def main():
    try:
        print("Assignment Averages: ")
        all_averages()

        print("")


        print("Student Averages: ")
        
        all_student_averages()
    except:
        #displays if an error occurs
        print("An error has occurred. Please try again.")

#gets grades for an individual assignment
def get_assignment_grades(n):
    column = []
    for row in gradebook:
        element_in_column = row[n]
        column.append(element_in_column)

    return column

#averages grades for single assignment
def assignment_average(a):
    column = get_assignment_grades(a)
    total = 0

    for grade in column:
        total += grade

    average = total / len(column)

    return average

    
#displays averages for all assignments
def all_averages():
    for num in range(num_of_assignments):
        average = assignment_average(num)
        
        print("Assignment " + str(num + 1) + ": {:0.2f}".format(average))
        
#gets single student's grades
def student_grades(n):
    grades = gradebook[n]

    return grades
    

#averages student's grades
def student_average(a):
    row = student_grades(a)
    total = 0

    for grade in row:
        total += grade

    average = total / len(row)

    return average

#displays all students' averages
def all_student_averages():
    for num in range(len(gradebook)):
        average = student_average(num)

        print("Student " + str(num + 1) + ": {:0.2f}".format(average))



#main
main()
```
This program sorts and provides information about student's grades on particular assignments.

---

Navigate between pages:
- [Page One](page1.md)
- [Page Two](page2.md)
- [Page Three](page3.md)
- Page Four
- [Page Five](page5.md)

