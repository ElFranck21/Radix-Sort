# Radix-Sort
La idea de radix sort es ordenar los elementos digito por digito de los mas significativos a los menos significativos, ordenado por unidades luego por decenas luego por centenas 
radix sort utiliza counting sort como una sub rutina para poder ordenar 

EJEMPLO 
170 45 75 90 802 24 2 66 (vamos a ordenarlos pero solo viendo el primer digito las unidades aplicando counting sort)

Arreglo 
0 0 0 0 0 0 0 0 0 0
0 1 2 3 4 5 6 7 8 9 (contando del 0 al 9 para ver cualquier numero que pueda salir)


COUNTING SORT

Solo numeros del 0 al 9 

Ejemplo
1 4 1 2 7 5 2
se recorre el arreglo haciendo la suma de los numeros en el arreglo
Arreglo 
0 2 2 0 1 1 0 1 0 0(primer corrida)
0 1 2 3 4 5 6 7 8 9 

despues se hace una suma acumilativa del arreglo ejemplo
Arreglo
0 2+2+0+1+1+0+1+0+0
0 2 4 4 5 6 6 7 7 7
Numeros a acomodar
1 4 1 2 7 5 2
Arreglo
0 2 4 4 5 6 6 7 7 7
0 1 2 3 4 5 6 7 8 9

Final
1 4 1 2 7 5 2

0 0 2 4 4 5 6 6 7 7  (se decrementa en 1 el valor que esta en la tabla/casilla para cuando exista otra carta con el mismo valor colocarla en la posicion correcta)
0 1 2 3 4 5 6 7 8 9  

1 1 2 2 4 5 7

