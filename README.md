# Pattern 1: Simple Number Triangle Pattern
rows = 6
for num in range(rows):
    for i in range(num):
        print(num, end=" ") # print number
    # line after each row to display pattern correctly
    print(" ")

# Pattern 2: Inverted Pyramid of Numbers
rows = 5
b = 0
for i in range(rows, 0, -1):
    b += 1
    for j in range(1, i + 1):
        print(b, end=' ')
    print('\r')

 # Pattern #3: Half Pyramid Pattern of Numbers
 rows = 5
for row in range(1, rows+1):
    for column in range(1, row + 1):
        print(column, end=' ')
    print("")

# Pattern 4: Inverted Pyramid of the Same Digit
rows = 5
num = rows
for i in range(rows, 0, -1):
    for j in range(0, i):
        print(num, end=' ')
    print("\r")

# Pattern 5: Reverse Pyramid of Numbers
rows = 6
for row in range(1, rows):
    for column in range(row, 0, -1):
        print(column, end=' ')
    print("")

# Pattern 6: Equilateral Triangle with Stars (Asterisk Symbol)
print("Print equilateral triangle Pyramid using stars ")
size = 7
m = (2 * size) - 2
for i in range(0, size):
    for j in range(0, m):
        print(end=" ")
    m = m - 1 # decrementing m after each loop
    for j in range(0, i + 1):
        # printing full Triangle pyramid using stars
        print("* ", end=' ')
    print(" ")


# Pattern 7: Downward Triangle Pattern of Stars
rows = 5
k = 2 * rows - 2
for i in range(rows, -1, -1):
    for j in range(k, 0, -1):
        print(end=" ")
    k = k + 1
    for j in range(0, i + 1):
        print("*", end=" ")
    print("")
