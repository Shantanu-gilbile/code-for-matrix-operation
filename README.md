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
# Program to add two matrices
addition = []
for i in range(row):
    add = []
    for j in range(coloumn):
        result = Matrix1[i][j] + Matrix2[i][j]
        add.append(result)
    addition.append(add)
print("addition =",addition)

# Program to substracte two matrices 
substraction = []
for i in range(row):
    sub = []
    for j in range(coloumn):
        result = Matrix1[i][j] - Matrix2[i][j]
        sub.append(result)
    substraction.append(sub)
print("substraction =",substraction)

#Program for transpose of matrix
transpose1=[]
for i in range(row):
    trans=[]
    for j in range(coloumn):
        result=Matrix1[j][i]
        trans.append(result)
    transpose1.append(trans)
print("Transpose of matrix 1 =",transpose1)

transpose2=[]
for i in range(row):
    trans=[]
    for j in range(coloumn):
        result=Matrix2[j][i]
        trans.append(result)
    transpose2.append(trans)
print("Transpose of matrix 2 =",transpose2)








