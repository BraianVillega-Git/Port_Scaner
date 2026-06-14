# Port Scanner en Python

Un script simple de escaneo de puertos realizado en Python, utilizando sockets para verificar si los puertos de un host están abiertos o cerrados.

## 📋 Descripción

Este script realiza un escaneo de puertos en el rango de **1 a 1024** (puertos comunes) en una IP proporcionada por el usuario. Utiliza la biblioteca `socket` para intentar conectar con cada puerto y `termcolor` para mostrar el resultado con colores en la terminal.

## ⚙️ Funcionalidades

- Escaneo de puertos del 1 al 1024.
- Tiempo de espera de 1 segundo por conexión (`settimeout(1)`).
- Muestra puertos abiertos en **verde**.
- Manejo de errores para puertos cerrados o con timeout.
- Input interactivo de la IP target.

## 🛠️ Requisitos

- Python 3.x
- Biblioteca `termcolor`

## 📦 Instalación

1. Instalar la dependencia necesaria:

```bash
pip install termcolor
```

2. Clonar o descargar el script:

```bash
git clone <url-del-repo>
# o simplemente descarga el archivo port_scanner.py
```

## 🚀 Uso

```bash
python port_scanner.py
```

Luego, introduce la IP del host que deseas escanear:


[+] Introduce la Direccion IP: 192.168.1.1


El script mostrará en la terminal los puertos abiertos en color verde.

## ⚠️ Notas

- Este script está diseñado para uso **educativo** y de pruebas en sistemas propios o con autorización.
- No está optimizado para rendimiento ni para escaneo de grandes rangos de IPs.
- El timeout de 1 segundo puede hacer que el escaneo sea lento en redes con latencia.

## 📄 Estructura del código

```python
create_socket()   # Crea un socket TCP con timeout de 1s
port_scanner()    # Intenta conectar con un puerto específico
main()            # Itera sobre los puertos 1-1024 y llama a port_scanner
```

## ⚖️ Licencia

Este proyecto es de uso educativo. Úsalo responsablemente y solo en sistemas donde tengas autorización.
