# Cadena de Caracteres

Las cadenas de caracteres en python es la forma en que se manipula la informacion textual, es decir todo tipo de caracteres alfanumericos, que puede ser un texto, un libro, articulos cientificos, una carta etc. Y estos son representados en python como un objeto str, el cual tiene sus propios metodos y funciones externas para su manipulacion.

`#` Como es definida una cadena de caracteres

    Las cadenas se pueden definir de diferentes maneras:
      - Comillas simples: 'permite incluir comillas "dobles"'
      - Comillas dobles: "permite incluir comillas 'simples'"
      - Triples comillas: ya sea con comillas simples  o dobles.
    
Las cadenas definidas con comillas tripes pueden incluir varias líneas - todos los espacios en blancos incluidos se incorporan a la cadena de forma literal.

 Veamos ejemplos:
    
            dato1 =  "secuencia1"
            dato2 =  'secuencia2'
            
    A la variable text le hemos asignado una cadena de texto, esto es asi ya que el texto secuencia1, lo hemos incluido dentro de comillas dobles, la cual es fundamental para definir una cadena de texto en python, como asi tambien es posible definir una cadena de texto con comillas simples, esto lo podemos comprobar viendo el tipo de dato de dato1 y dato2 de la siugiente manera:
    
            dato1 = 'secuencia1'
            dato2 = "secuencia2"
            dato3 = 12345

            print(type(dato1))
            print(type(dato2))
            print(type(dato3))

            print(type(dato1) == type(dato2))
            print(type(dato1) == type(dato3))
            
            Resultado:
                <type 'str'>
                <type 'str'>
                <type 'int'>
                True
                False
                
    Hemos definido tres variabes, una con un valor dentro de comisllas simples, otra con comillas dobles y la tercera sin comillas, verificamos el tipo de datos dando como resultado que el primero y el segundo son del tipo 'str', y el tercero de tipo entero, luego verificamos tanto el primero definido con comillas simples como el segundo definido con comillas dobles son del mismo tipo, posteriormete realizamos la comparacion con el tercero arrojandonos un False, es decir no son del mismo tipo.


`#` Cadena de Caracteres como secuencia inmutable

    Las cadenas de caracteres en python son secuencia de caractres inmutables, por lo tanto de esto extraemos que las cadenas de caracteres son:
    
    1 - Secuencia: la secuencia consiste en una serie de elementos que se suceden unos a otros y guardan relacion entre si, por lo tanto cada caracter
    dentro de un texto tendrian un orden y ocuparian una posicion determianda dentro del mismo. 
    
    
        Veamos un ejemplo del porque los caractres son secuenciales:

                texto = 'secuencia'
                print(texto) Resultado: secuencia
                
        Aqui lo que hicimos fue asignar a la variable texto una cadena de caracteres, luego imprimimos en en la terminal ( secuencia ), vemos que cada elemento de la cadena
        de caracteres se suceden unos a otro para formar una palabra, cada uno de estos elementos ordenados tienen un indice que determian su posicion, es decir a cada elemento le corresponde un indice
        determinado al cual podemos acceder, el primer elemento de la palabra secuencia 's', tiene la posicion 0, luego el elemento 'e' tiene la posicion 1 y asi hasta llegar al ultimo elemento que cuenta con un indice.
        
        Cual es la forma en que podemos acceder a dichos elementos?. Podemos acceder a cada elemento de una cadena de caractres colocando la variable que contiene la cadena inmediatemente seguido
        de un corchete dentro del cual, asignamos el indice del elemento que queremos acceder.
        
            texto = 'secuencia'
            print(texto[0]) # Resultado = s
            print(texto[1]) # Resultado = e
            print(texto[7]) # Resultaod = i 
        
        Vemos como podemos acceder a cada elemento de una cadena de caractres a traves de su indice, por lo tanto esto comprueba la secuencialidad del mismo.
        
        
    2 - Inmutables: la inmutabilidad de las cadenas de caractes consiste en que una vez creada una cadena de caracteres no puede ser modificada. 
    
            texto = 'secuencia'
            texto[0] = 'S'
        
        Lo que intentamos hacer es, colocar en mayuscula el elemento s ubicado en la posicion [0], lo que nos arroja un error ya que estas son inmutables, si bien es cierto
        que las cadenas de caractres cuentan con sus metodos propios para colocar una palabra en mayuscula o minuscua, estos no son modificadas sino que crear una nueva palabra 
        que se puede incorporar a una variable.
        
            texto = 'secuencia'
            textoMayuscula = texto.capitalize()
            print(texto) # Resultado: secuencia
            print(textoMayuscula) # Resultado: Secuencia
        
        Vemos que el metodo no modifica la variable texto, sino que solamente retorna un nuevo texto modificado.
             
