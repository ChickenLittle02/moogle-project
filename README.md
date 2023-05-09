# Moogle!

![](moogle.png)

> Proyecto de Programación I.
> Facultad de Matemática y Computación - Universidad de La Habana.

 Para incializar el buscador, copiamos los documentos de tipo .txt en la carpeta Content, y tenemos que garantizar que el nombre de la carpeta principal
 sea moogle-main e iniciamos el proyecto.
 Para ello debemos abrir la carpeta del proyecto y ejecutar en la terminal de Linux:

```bash
make dev
```

Si estás en Windows, desde la carpeta raíz del proyecto debes ejecutar el comando:

```bash
dotnet watch run --project MoogleServer
```
Y se abrirá un navegador en el cual ponemos la búsqueda que queremos realizar,
Podemos utilizar los operadores !,^,* delante de las palabras,
los cuales tendrán los siguientes efectos en los resultados de búsqueda:
SI la palabra tiene delante !, ejemplo !carro, se devolverán los documentos donde no aparezca la palabra carro
SI la palabra tiene delante ^, ejemplo ^carro, se devolverán solamente los documentos donde aparezca la palabra carro
SI la palabra tiene delante *, ejemplo *carro, los documentos que tengan la palabra carro tendrán mayor relevancia

También tenemos el operador ~ que se utilizará entre dos palabras
asiento ~carro
El cual dará una mayor relevancia a los documentos que tengan esas dos palabras, mientras más cerca mayor relevancia tendrán
