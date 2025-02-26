# Reto_11

### Ejercicio 1:

- Endswith:

Endswith() es una herramienta de Python para comprobar si una cadena termina con cierta cadena determinada, se realzan comprobaciones sencillas y se evaluan rangos específicos dentro de la cadena.

- Startswith:

Startswith() es una herramiena que verifica si la cadena inicia con una cadena especifica, sirve para filtrar las cadenas.

- Isalpha:

Isalpha() es una herramienta que comprueba si una cadena contiene caracteres numericos, espacios o caracteres especiales, dando como resultado el boleano False se lo tiene.

- Isalnum:

Isalnum() es una herramienta para verificar si todos los caracteres de la cadena son alphanumericos.

- Isdigit:

Isdigit() es una herramienta para verificar si todos los caracteres de la cadena son digitos, valores numericos del 0-9.

- Istitle:

Istitle() es una herramienta para verificar si cada palabra de la cadena de caracteres inicia con mayuscula y las demas letras son minusculas.

- Islower:

Islower() es una herramienta que comprueba si todos los carcteres de la cadena estan en minuscula.

- Isupper:

Isupper() es una herramienta que comprueba si todos los carcteres de la cadena estan en mayuscula.

Referencia:
[https://www.geeksforgeeks.org/]

### Ejercicio 2:

Text esta adjunto en el repo en el Archivo_a_contar

Primero:
```python
from Archivo_a_contar import texto

Cuenta_de_vocales_m= texto.count("a") + texto.count("e") + texto.count("i") + texto.count("o") + texto.count("u")
print(f"El numero de apariciones de las vocales minusculas  en Text es = {Cuenta_de_vocales_m}")

Cuenta_de_vocales_M = texto.count("A") + texto.count("E") + texto.count("I") + texto.count("O") + texto.count("U")
print(f"El numero de apariciones de las vocales mayusculas en Text es = {Cuenta_de_vocales_M}")

Numero_total = Cuenta_de_vocales_M + Cuenta_de_vocales_m
print(f"El numero total de vocales es = {Numero_total}")
```

Segundo:
```python
#Se importa el string texto
from Archivo_a_contar import texto

#Se define la función para poder contar las consonantes en texto
def Cuenta_de_consonantes(texto_1):
  #Valor al que se le suma si hay una consonate
  Suma = 0
  #Se definen las consonantes
  Consonantes="bcdfghjklmnpqrstvwxyzBCDFGHJKLMNPQRSTVWXYZ"
  #Se evaluan todas las letras de text_1
  for i in texto_1:
    #Si i esta en consonantes se suma 1
    if i in Consonantes:
      Suma+=1

  return Suma

if __name__ == "__main__":
  Num_consonantes = Cuenta_de_consonantes(texto)
  #Se imprime el numero de consonates
  print(f"El numero de consonantes en texto es = {Num_consonantes}")
```

