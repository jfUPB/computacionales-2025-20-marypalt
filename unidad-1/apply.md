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
