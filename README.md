# MFC-pratical
QUESTION1:
import numpy as np
NR = int(input("Enter the number of Rows:"))
NC = int(input("Enter the number of columbs:"))
print("Enter the entries in a single line (seperated by space):")
entries = list(map(int,input().split()))
matrix= np.array(entries).reshape(NR,NC)
print("Matrix X is as follows", '\n',matrix)
print("The transpose of Matrix X is as follows:",'\n',np.transpose(matrix))    




Question2:
import numpy as np
NR = int(input("Enter the number of Rows:"))
NC = int(input("Enter the number of columbs:"))
print("Enter the entries in a single line (seperated by space):")
entries = list(map(int,input().split()))
matrix= np.array(entries).reshape(NR,NC)
print("Matrix X is as follows", '\n',matrix)
print("The rank of a matrix is :" , np.linalg.matrix_rank(matrix))


Question3:
import numpy as np
NR = int(input("Enter the number of Rows:"))
NC = int(input("Enter the number of columbs:"))
print("Enter the entries in a single line (seperated by space):")
entries = list(map(int,input().split()))
matrix= np.array(entries).reshape(NR,NC)
print("Matrix X is as follows", '\n',matrix)
matrix_Inverse = np.linalg.inv(matrix)
Transpose_of_matrix_Inverse = np.linalg.det(matrix)
Determinant_of_matrix = np.linalg.det(matrix)
Cofactor_of_matrix = np.dot(Transpose_of_matrix_Inverse,Determinant_of_matrix)
print("The cofactor of a matrix is:",'\n',Cofactor_of_matrix)
print("The Determinant of a Matrix is:"'\n',Determinant_of_matrix)



QUESTION4::
import numpy as np
print("Enter the dimension of coefficientmatrix(A):")
NR = int(input("Enter the number of rows :"))
NC =int(input("Enter the number of columns:"))
print("Enter the elements of coefficients of matrix(A) in single line(seperated by space):")
Coefficients_Entries = list(map(float,input().split()))
Coefficients_Matrix = np.array(Coefficients_Entries).reshape(NR,NC)
print("Coefficient Matrix(A)is as follows:",'\n',Coefficients_Matrix,"\n")
