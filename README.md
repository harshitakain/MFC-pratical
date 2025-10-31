## MFC-pratical
# QUESTION1:
import numpy as np
NR = int(input("Enter the number of Rows:"))
NC = int(input("Enter the number of columbs:"))
print("Enter the entries in a single line (seperated by space):")
entries = list(map(int,input().split()))
matrix= np.array(entries).reshape(NR,NC)
print("Matrix X is as follows", '\n',matrix)
print("The transpose of Matrix X is as follows:",'\n',np.transpose(matrix))    




# Question2:
import numpy as np
NR = int(input("Enter the number of Rows:"))
NC = int(input("Enter the number of columbs:"))
print("Enter the entries in a single line (seperated by space):")
entries = list(map(int,input().split()))
matrix= np.array(entries).reshape(NR,NC)
print("Matrix X is as follows", '\n',matrix)
print("The rank of a matrix is :" , np.linalg.matrix_rank(matrix))


# Question3:
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



# QUESTION4::
import numpy as np
print("Enter the dimension of coefficientmatrix(A):")
NR = int(input("Enter the number of rows :"))
NC =int(input("Enter the number of columns:"))
print("Enter the elements of coefficients of matrix(A) in single line(seperated by space):")
Coefficients_Entries = list(map(float,input().split()))
Coefficients_Matrix = np.array(Coefficients_Entries).reshape(NR,NC)
print("Coefficient Matrix(A)is as follows:",'\n',Coefficients_Matrix,"\n")




##Questin5::
from numpy import linalg
import numpy as np
print("Enter the Dimension of coefficients matrix(A):")
NR=int(input("Enter the numberof rows:"))
NC=int(input("Enter the number of columns:"))
print("Enter the  elements of coefficients matrix(A) in a single line (seperated by space):")
Coefficients_of_Entries = list(map(float,input().split()))
Coefficient_Matrix = np.array(Coefficients_Entries).reshape(NR,NC)
print("Coefficient Matrix(A)is as follows",'\n',Coefficient_Matrix,"\n")
print("Enter the Elements of column matrix(B) in single line(seperated by space):")
Column_Entries = list(map(float,input().split()))
Column_Matrix = np.array(column_Entries).reshape(NR,1)
print("Column Matrix(B) is as follows:",'\n',Column_Matrix,"\n")
Inv_of_Coefficient_Matrix = linalg.inv(Coefficient_Matrix)
Solution_of_the_system_of_Equations=np.matmul(Inv_of_Cofficient_Matrix,Column_Matrix)
print("Solution of the system of Equations using GUASS JORDAN")
print(Solution_of_the_system_of_Equations)

