# comandos de procesos
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


## Opcionesde top


### M - Uso de memoria
### N - Orden por PID
### R - Invertir el orden
### T - Tiempo acumulado de los procesos
### U - Filtrar por usuario
### p - Ordenar por PID
### C - Uso de CPU


## puedes hacer en un archivo una instantanea de top 
```bash
top -b -n 1 > toppp.txt
```
![imagen](https://github.com/user-attachments/assets/12bfe962-cd4d-46ea-9831-a8e6da2c4c69)


```bash
top -b -n 3 -o +%CPU | head -n 11 > topmasprocesados.txt
```
![imagen](https://github.com/user-attachments/assets/68f4d531-4e1a-4f7e-9138-e5a67fc16491)

## htop
### no suele venir por defecto instalado

```bash
apt install htop
```

![imagen](https://github.com/user-attachments/assets/ee819f31-9a5c-475e-849f-3d56fb0398d8)

---

## Atajos de Teclado Más Interesantes

- **`F2 (Setup)`**: Personaliza columnas, colores y oculta procesos según preferencias.  
- **`F3 (Search)`**: Encuentra procesos rápidamente por nombre o ID.  
- **`F4 (Filter)`**: Muestra procesos que coincidan con un filtro específico.  
- **`F5 (Tree)`**: Presenta procesos en formato jerárquico para ver relaciones entre ellos.  
- **`F6 (Sort)`**: Cambia el orden de los procesos por CPU, memoria, tiempo de CPU o PID.  
- **`F9 (Kill)`**: Finaliza procesos enviando señales directamente desde la interfaz.  


### `F9 (Kill)` - Terminar un Proceso
- Enviar señales para finalizar procesos directamente desde la interfaz.

---

## Opciones de Línea de Comandos

- **`htop -u <usuario>`**: Muestra solo los procesos de un usuario específico.
- **`htop --tree`**: Inicia `htop` directamente en modo árbol.
- **`htop -p <PID1,PID2>`**: Muestra información solo de los procesos con los PIDs especificados.

---
## Ventajas de `htop` Frente a top

1. Ofrece una interfaz visual mejorada con barras gráficas y colores.  
2. Permite navegar y seleccionar procesos usando teclado o mouse.  
3. Configuración rápida y flexible directamente desde la interfaz.  

## atop

![imagen](https://github.com/user-attachments/assets/3fd1ac9c-d9dc-4fdf-b274-d96d9e172f03)

Modificar para que lo haga cada 60 segundos
```bash
sudo nano /etc/default/atop
```
Cambiar la linea `INTERVAL=60` y guardar

Logs de atop
```bash
sudo cd /var/log/atop
# listar
ls
# para ver el log
atop -r nombre_log
```
