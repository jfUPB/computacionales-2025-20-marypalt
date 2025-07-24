# Unidad 1

## 🛠 Fase: Apply
## ACTIVIDAD 1
### EXPERIMENTO 1
En la dirección de memoria 16 se almacenó el número 3. Ese valor es la suma de los números 1 y 2 indicado en la instruccion 3 del contador (D=D+A).

En el ciclo Fetch se obtuvieron los valores asignados en cada instrucción. En Decode se interpretó que debían sumarse los valores indicados. En el ciclo Execute se resolvió la operacion de la suma y almacenó ese valor en la dirección de memoria 16.
### EXPERIMENTO 2
**PROGRAMA**
```asm
@5
D=A
@10
D=D+A
@20
M=D
@END
(END)
0;JMP
```
**RESULTADO NAND2TETRIS**
<img width="1073" height="630" alt="image" src="https://github.com/user-attachments/assets/df885d38-9c6d-4b58-83ca-e101ec32a64c" />

**¿Qué diferencia hay entre los datos almancenados en la memoria ROM y en la RAM?**

La ROM almacena el programa (instrucciones) y no se puede modificar durante la ejecución, mientras que la RAM guarda los datos temporales, variables y resultados que sí cambian durante la ejecución del programa. En el simulador Hack, la ROM contiene el código ensamblador traducido, y la RAM se usa para almacenar valores como el resultado de una suma o el estado de la pantalla.
## ACTIVIDAD 2
**1. Identifica una instrucción que use la ALU y explica qué hace.**

```asm
D=D-A
```
Esta instrucción usa la ALU (unidad aritmética y lógica) para restar el valor del registro A al contenido del registro D. El resultado se guarda en D. 

**2. ¿Para qué sirve el registro PC?**

El registro PC (Program Counter) guarda la dirección de la siguiente instrucción a ejecutar. Se incrementa automáticamente con cada instrucción, salvo que haya un salto (como @READKEYBOARD o D;JNE), donde se cambia a otra dirección específica.


**3. ¿Cuál es la diferencia entre @i y @READKEYBOARD?**

@i accede a una variable en RAM, generalmente usada para guardar datos (en este caso, una dirección de pantalla) y @READKEYBOARD es una etiqueta del programa, usada como marcador para saltar a una parte del código.

**4. Describe qué se necesita para leer el teclado y mostrar información en la pantalla.**

**5. Identifica un bucle en el programa y explica su funcionamiento.**

**6. Identifica una condición en el programa y explica su funcionamiento.**
