# Alumno: Lucas Zapata
Ingenieria Informatica
## Codigo comentado para entender el funcionamiento.
    def contar_vocales(palabra):
        # Define un conjunto de vocales
        vocales = {"a", "e", "i", "o", "u"}
    
        # Inicia un diccionario para almacenar el resultado
        resultado = {}
    
        # Elimina espacios, comas y guiones, y convierte la palabra a minúsculas
        palabra = palabra.replace(" ", "").replace(",", "").replace("-", "").lower()
    
        # Itera sobre cada letra en la palabra
        for letra in palabra:
            # Verifica si la letra es una vocal
            if letra in vocales:
                # Si la vocal ya está en el diccionario, incrementa su contador
                if not resultado.get(letra):
                    resultado[letra] = 0
                resultado[letra] += 1 
    
        # Devuelve el diccionario con el conteo de vocales
        return resultado
  ## Para comprobar si funciona
    -Realizar un git clone (link con el SSH del repo) en la carpeta donde quieras almacenar el archivo.
    -Una vez con los direcctorios en su computadora los busca en la terminal usando cd (nombre de la carpeta donde se encuentra el archivo)
    -Ya en la carpeta donde se encuentra el archivo ejecutamos python3 test_contar_vocales.py
    -Luego de esto y finalmente se ejecutaran los test para comprobar si el codigo funciona correctamete.
