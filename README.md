<p align="center"><img width=450 alt="RevShellRelay" src="https://github.com/vpanal/revshellrelay/blob/main/assets/revshellrelay.png"></p>

RevShellRelay es un script en Python diseñado para manejar comunicaciones entre un atacante y una víctima a través de sockets, permitiendo estabilizar una shell inversa a una terminal interactiva.

## Características
- Configura una shell remota con soporte para reconexion del atacante.
- Configuración personalizada mediante argumentos.

## Requisitos
- Python 3.x
- Librerías estándar de Python: `socket`, `threading`, `argparse`, `sys`, `termios`, `tty`

## Instalación
   ```bash
   git clone https://github.com/vpanal/revshellrelay.git
   cd revshellrelay
   ```

## Uso
### Ejemplo básico:
```bash
python3 revshellrelay.py --host 0.0.0.0 --port 4444 --host2 0.0.0.0 --port2 5000 -p 12345
```

### Argumentos:
- `--host`: Dirección IP del servidor para recibir la reverse shell (por defecto: `0.0.0.0`).
- `--host2`: Dirección IP para la conexión del cliente atacante (por defecto: `0.0.0.0`).
- `--port`: Puerto para la conexión de datos (por defecto: `4444`).
- `--port2`: Puerto para la conexión de la shell (por defecto: `5000`).
- `-p`: Contraseña para autenticación (por defecto: `12345`).

### Ejemplo con parámetros personalizados:
```bash
python3 revshellrelay.py --host 192.168.1.10 --port 5555 --host2 192.168.1.20 --port2 6000 -p 98765
```

## Demo

<p align="left"><img width=100% alt="Demostración de uso" src="https://github.com/vpanal/revshellrelay/blob/main/assets/demo.gif"></p>

## Notas de seguridad
Este script está diseñado únicamente para propósitos educativos y de pruebas en entornos controlados. **No lo uses en sistemas sin autorización explícita.**

## Contribuciones
Si deseas contribuir, realiza un fork del repositorio, haz tus cambios y envía un pull request.

## Licencia
Este proyecto está bajo la Licencia MIT. Consulta el archivo `LICENSE` para más detalles.

