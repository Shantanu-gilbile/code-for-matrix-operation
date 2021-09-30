# code-for-matrix-operation
row = int(input('Enter The No Of Rows: '))
coloumn = int(input('Enter The Number Of Coloumns: '))

print('Enter The Entries Rowwise:')

def mat(row, coloumn):
    x1 = []
    for i in range(row):
        a = []
        for j in range(coloumn):
            num = int(input('enter the numbers'))
            a.append(num)
        x1.append(a)

    return x1

Matrix1= mat(row, coloumn)
print(Matrix1)
print()
Matrix2= mat(row, coloumn)
print(Matrix2)

# Program to add two matrices using list 
result = [[Matrix1[i][j] + Matrix2[i][j]  for j in range(len(Matrix1[0]))] for i in range(len(Matrix1))]
print()
print('Addition of Matrix1 and Matrix2 is: ')
for r in result:
    print(r)

# Program to substracte two matrices using list 
result = [[Matrix1[i][j] - Matrix2[i][j]  for j in range(len(Matrix1[0]))] for i in range(len(Matrix1))]
print()
print('Substraction of Matrix1 and Matrix2 is: ')
for r in result:
    print(r)
    
#Program for transpose of matrix
for r in range(row):
    for c in range(coloumn):
        result[c][r] = Matrix1[r][c]
        result[c][r]=Matrix2[r][c]
print()
print("Transpose of Matrix1 is: ")
for r in result:
    print(r)
print()
print("Transpose of Matrix2 is: ")
for r1 in result:
    print(r1)





