![imagen](https://github.com/user-attachments/assets/36b2f34c-9c48-4cbd-aa8e-2e12961ebc40)![imagen](https://github.com/user-attachments/assets/eca3cdd7-d73b-4b80-adae-239f5808f840)# comandos de procesos
## ps
```bash
ps
ps a
ps au
```
![imagen](https://github.com/user-attachments/assets/f0fe0bc7-e653-48b2-8a29-182f1738e18f)

```bash
ps aux
```
![imagen](https://github.com/user-attachments/assets/ce73c4c1-e124-42ef-a55d-0e1e87c9b2b4)

### para ver un proceso en especifico
```bash
ps -C nano
```
![imagen](https://github.com/user-attachments/assets/a5e0806e-a4cf-4589-86e0-22735f25903f)


```bash
```
![imagen](https://github.com/user-attachments/assets/e720278e-dcf9-4699-aa4a-e17993166f9e)

## top
![imagen](https://github.com/user-attachments/assets/3b658a22-5322-48b7-88e6-d8683ef2e4a9)


## Opciones y atajos dentro de `top`

### `T` - Tiempo acumulado de los procesos
- Ordena los procesos según el **tiempo total de CPU acumulado** que han utilizado.
- Útil para identificar procesos que han consumido mucho tiempo de CPU durante su ejecución.

### `M` - Uso de memoria
- Ordena los procesos por la cantidad de **memoria RAM** que están utilizando.
- Ideal para localizar procesos que consumen demasiada RAM.

### `U` - Filtrar por usuario
- Permite mostrar los procesos de un **usuario específico**.
- Tras presionar `U`, se solicita el nombre de usuario.

### `p` - Ordenar por PID
- Ordena los procesos por su **ID de proceso** (PID).
- Es útil para localizar un proceso específico si conoces su PID.

### `P` - Uso de CPU
- Ordena los procesos por el **uso de la CPU** (de mayor a menor).
- Ayuda a identificar qué procesos están consumiendo más recursos de CPU.

### `N` - Orden por PID
- Igual que `p`, ordena los procesos por el **PID** en orden ascendente.

### `R` - Invertir el orden
- **Invierte el orden** de la columna seleccionada para ordenar.
- Por ejemplo, si los procesos están ordenados por PID, los muestra en orden descendente.


## puedes guardar en un archivo una instantanea de top con el siguiente comando
```bash
top -b -n 1 > top.txt
```
![imagen](https://github.com/user-attachments/assets/12bfe962-cd4d-46ea-9831-a8e6da2c4c69)


```bash
top -b -n 3 -o +%CPU | head -n 17 > topmasprocesados.txt
```
![imagen](https://github.com/user-attachments/assets/68f4d531-4e1a-4f7e-9138-e5a67fc16491)

## htop

![imagen](https://github.com/user-attachments/assets/ee819f31-9a5c-475e-849f-3d56fb0398d8)



```bash
```

```bash
```

```bash
```
