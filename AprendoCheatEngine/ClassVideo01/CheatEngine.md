## Para aprender por nosotros mismos 

### Cambio de valor de vidas problema basico
PW=419482

### Sin saber el valor i9nicial

El cheat engine va a scanear toda la memoria del proceso, y luego se va filtrar
No sabemos que vida tengo, pero si sabemos que ha cambiado (ha bajado el valor)


Primero se escanea todo, y no se muestra lista, pero si se ha guardado

Luego nexto scan, para mostrar las direcciones que se van a mostra

### Tipos de valor que se puede escanear
Presionar *Memory View* parte media izquierda del programa
Direccion de memoria
Identifica unma posicion en la direccion de memoria del proceso

### Valors en memoria float y double
Podemos cambiar el tipo selecionando type y cambiarlo al que se desea
float (4 bytes)
s=1
m=23
e=8
### Representacion de lcodigo en memoria

Cuando se ejecuta un proceso en windows,caraga las instrucciones que se v a a ejecutar en la memoria de ese proceso, por el procesador GPU va ejecutando las instrucciones del proceso, esa instrucciones son el codigo interno de ese proceso.

En seccion addes esta el codigo del procesos mas un sumando en hexadecimal
(Para cambiarlo, desenmarcar viw sohw module addresses, ose no mostrar el modulo)

### Para valores aleatorios

##### Debuger
Un debugr, es una herramiento para analizar la ejecucion de un programa y monitorear la ejecucion

- hacer anticlick en el dato de memoria, luego find out writhe adrres para analizar la direcion de memoria
- show this addresses in assembler
La memoria de un proceso, son codigo almacenados en la memoria del proceso GPU, y bueno con esa idea se puede cambiar

#### Punteros 
Una direccion der memoria con otra direccion de memoriak

Entonces 
- Tienes una direccion con un valor
- hay un puntero que tiene la direccion
- Entonces busco el valor de la direccion
- Me va a buscar las direcciones que tienen la direccion que estoy buscado
- Entonces encuentro el puntero
- paso final, cambiar valor y poner un x en active(congela la direccion de memoria, de manera que el proceso no pueda sobreescribir su valor)

#### PW=013370

## Insersicon de Codigo
Primero se inserta el valor normalmente
- En address hacer anticlick(Find) out what write to this address
- Esperar que se cambie el valor y se va a mostrar la instruccion
- Hacer anticlick en la opcion show this address in this assembler
- Vamos en ventana de assemble, en toools, en auto assemble luego en templete en code injection
- cambiamos codigo y damos en execute, 
Si queremos ver e informanos 
- Click derecho en follow, nos muestra la direccion de memoria original
- Clicl en el jmp para volver y siga codigo que se esta ejecutando
- Con eso nos damos cuenta que, tu insertas el codigo pero este con la ejecucion jmp vuelve a la linea de codigo para que no haya ninguna interrupcion