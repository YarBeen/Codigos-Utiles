'Yarman '
from math import pow
def matriz_vacia(n,m):
   res=[]
   for i in range(n):
       fila=[]
       for j in range(m):
           fila.append(0)
       res.append(fila)
   return res
def multiplicacion_de_matrices(a,b):
   fil=len(a)
   col = len(b[0])
   resp= matriz_vacia(fil,col)
   for i in range (fil):
       for j in range(col):
           for k in range(len(b)):
               resp[i][j]+=a[i][k]*b[k][j]
   return resp

def exponenciacion_matrices(matriz,n):
   if n==1:
       return matriz
   resp=exponenciacion_matrices(matriz,n//2)
   print(resp)
   resp=multiplicacion_de_matrices(resp,resp)
   if n%2:
       resp=multiplicacion_de_matrices(matriz,resp)
   print(resp)
   return resp

def imprimirMatriz(matriz):
   for fila in matriz:
       print(fila)
   print()

def sumaFila(fila):
   suma = 0
   for valor in fila:
       suma += valor
   return suma > 0

def sumaDiagonales(tablero,posI,posJ):
   suma = 0
   for j in range(1, posJ + 1):
       if(posI - j >= 0):
           suma += tablero[posI - j][posJ - j]
       if(posI + j < len(tablero)):
           suma += tablero[posI + j][posJ - j]
   return suma > 0

def sumaColumna(matriz,posCol):
   suma = 0
   for i in range(len(matriz)):
       suma += matriz[i][posCol]
   return suma


