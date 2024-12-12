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
![imagen](https://github.com/user-attachments/assets/a20004d5-b336-4f8a-8486-80283c66f4b0)

