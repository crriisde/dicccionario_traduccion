print (" ") #Esta linea define el espacio para el nombre 
print ("Cristian David Sals De la O 3.w") #Esta linea muestra el nombre 
print (" ") #Esta linea define el espacio para el nombre 
def crear_diccionario(traducciones): #Esta linea define la funcion 

    diccionario = {} #Esta linea da el valor a diccionario 
    pares = traducciones.split(", ") #Esta linea define los pares a la traduccion 
    for par in pares: #Esta linea define le for 
        espanol, ingles = par.split(":") #Esta linea deifne la traducion con los dos puntos 
        diccionario[espanol.strip()] = ingles.strip() #Esta linea define la traducion 
    return diccionario #Esta linea concluye la funcion 

def traducir_frase(frase, diccionario): #Esta linea deifne la funcion 
    palabras = frase.split() #Esta linea las palabras en las frases
    traduccion = [] #Esta linea define la traduccion 
    for palabra in palabras: #Esta linea define el for 
        traduccion.append(diccionario.get(palabra, palabra)) #Esta linea define la traduccion 
    return " ".join(traduccion)#Esta linea concluye la funcion 

traducciones = input("Introduce las traducciones en el formato 'palabra:traducción', con el los dos puntos ") #Esta linea indica como traudcir

diccionario = crear_diccionario(traducciones) #Esta linea deifne le diccionario 

frase = input("Introduce una frase en español para traducir: ") #Esta linea pide la frase a ttraducir 

frase_traducida = traducir_frase(frase, diccionario) #Esta linea deifne la traduccion
![image](https://github.com/user-attachments/assets/0a081d41-7e42-42b9-b668-aa42bc5e36d7)
![image](https://github.com/user-attachments/assets/09491deb-9fce-4cb7-8684-d391208395b8)
