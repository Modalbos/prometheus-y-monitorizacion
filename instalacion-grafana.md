## Grafana
```bash
# Instalacion de paquetes necesarios
apt install apt-transport-https
software-properties-common wget
```
![imagen](https://github.com/user-attachments/assets/9a157d18-0e33-4531-be9d-4152b3da539b)
![imagen](https://github.com/user-attachments/assets/07426776-ff36-4723-a2d6-f3cddcf9f726)


```bash
# Añadimos la clave de grafana
wget -q -O - https://packages.grafana.com/gpg.key | apt-key add -
```
![imagen](https://github.com/user-attachments/assets/dc18652f-140a-4ee0-a8f4-c600178af6ce)

```bash
# Añadimos el repositorio de grafana
echo "deb https://packages.grafana.com/oss/deb stable main" | tee -a /etc/apt/sources.list.d/grafana.list
# si queremos buscar la key
apt-key list | grep grafana
```
![imagen](https://github.com/user-attachments/assets/bceb9522-f328-446c-9a35-79e689c5a0fa)
![imagen](https://github.com/user-attachments/assets/ccea3a09-40b5-4ee6-9658-7a654b64faf0)


```bash
# Actualizamos los repositorios
apt update
```
![imagen](https://github.com/user-attachments/assets/810bb61f-424b-4500-b604-5a26b3769f77)


```bash
# Instalamos grafana
apt install grafana
```
![imagen](https://github.com/user-attachments/assets/2624e5e5-e05b-4d3d-9bfb-9b3a5b4bcff7)

```bash
# Encendemos el servicio
systemctl daemon-reload
systemctl enable grafana-server
systemctl start grafana-server
```

![imagen](https://github.com/user-attachments/assets/497f5362-6bca-4982-a474-9a2ea3832164)

## acceso

![imagen](https://github.com/user-attachments/assets/77041338-83f5-4a40-93c7-9d9f0688e2c0)


## instalacion de prometheus en grafana


![imagen](https://github.com/user-attachments/assets/cccb0fb9-1cd0-4683-94b2-51ec638f7060)
### cargar el nodo

![imagen](https://github.com/user-attachments/assets/f9fd627a-f825-4253-b27b-edc237ea25e8)

### cargar el dashboard
![imagen](https://github.com/user-attachments/assets/345038a3-3b23-4da5-ab20-4ee999fb4698)

### archivos de configuracion

## prometheus
![imagen](https://github.com/user-attachments/assets/e20279b0-04e8-497c-b51c-7f366b15ed66)

## grafana
![imagen](https://github.com/user-attachments/assets/826b27ff-62ea-46e0-8997-61e1e6e024bd)

![imagen](https://github.com/user-attachments/assets/4c6571fc-068c-490b-8794-1b83f2e56060)


### pruebas de estres
### instalamos los paquetes de stress

## ram

![imagen](https://github.com/user-attachments/assets/3c49a8d8-6fed-45c6-970b-cdf161b6a836)

## cpu

![imagen](https://github.com/user-attachments/assets/daa1bbd4-4d2c-4889-90b0-3b549aedea00)

## disco
![imagen](https://github.com/user-attachments/assets/b52c4bcb-6967-48e3-9c7c-5c1339e6331f)

## ping
![imagen](https://github.com/user-attachments/assets/37ad171f-03ad-4bb3-871c-e9cc676606f9)




