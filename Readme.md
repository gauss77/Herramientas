
# Criptografía

- [CyberChef](https://gchq.github.io/CyberChef/) - Herramienta de manipulación de datos para descifrar y codificar mensajes cifrados (página web).
- [Hashcat](https://hashcat.net/hashcat/) - Herramienta de cracking de contraseñas que admite una amplia variedad de algoritmos de hash (herramienta de línea de comandos).
Ejemplo de uso: `hashcat -m 0 -a 0 hash.txt rockyou.txt` donde `hash.txt` es el archivo que contiene los hashes a crackear y `rockyou.txt` es el archivo que contiene la lista de contraseñas.
- [John the Ripper](https://www.openwall.com/john/) - Herramienta de cracking de contraseñas que admite varios tipos de cifrado y formatos de archivo (herramienta de línea de comandos).
Ejemplo de uso: `john hash.txt` donde `hash.txt` es el archivo que contiene los hashes a crackear.
- [Binwalk](https://github.com/ReFirmLabs/binwalk) - Herramienta para analizar archivos binarios y extraer firmware, imágenes y otros datos incrustados (herramienta de línea de comandos).
Ejemplo de uso: `binwalk archivo.bin` donde `archivo.bin` es el archivo binario que deseas analizar.
- [Foremost](https://github.com/korczis/foremost) - Herramienta de recuperación de datos para extraer archivos de un sistema de archivos o una imagen de disco (herramienta de línea de comandos).
Ejemplo de uso: `foremost -t all -i imagen.dd` donde `imagen.dd` es la imagen de disco que deseas analizar.
- [Strings](https://linux.die.net/man/1/strings) - Utilidad de línea de comandos que puede buscar cadenas de texto en un archivo binario (herramienta de línea de comandos).
Ejemplo de uso: `strings archivo.bin` donde `archivo.bin` es el archivo binario del que deseas extraer las cadenas de texto.

# Esteganografía

- [Steghide](http://steghide.sourceforge.net/) - Herramienta de esteganografía para ocultar datos en imágenes y archivos de audio (herramienta de línea de comandos).
Ejemplo de uso: `steghide extract -sf imagen.jpg` donde `imagen.jpg` es el archivo de imagen que contiene datos ocultos.
- [Exiftool](https://exiftool.org/) - Herramienta para leer y escribir metadatos en archivos de imagen, audio y video (herramienta de línea de comandos).
Ejemplo de uso: `exiftool archivo.jpg` donde `archivo.jpg` es el archivo de imagen del que deseas obtener información.

# Forense

- [Autopsy](https://www.sleuthkit.org/autopsy/) - Herramienta de análisis forense que puede analizar imágenes de discos y sistemas de archivos (herramienta gráfica).
- [Volatility](https://www.volatilityfoundation.org/) - Herramienta de análisis de memoria para extraer información de la memoria volátil de un sistema (herramienta de línea de comandos).
Ejemplo de uso: `volatility -f memoria.mem imageinfo` donde `memoria.mem` es el archivo de imagen de memoria volátil que deseas analizar.
- [Wireshark](https://www.wireshark.org/) - Analizador de tráfico de red que puede ser útil para encontrar evidencia en el tráfico de red capturado (herramienta gráfica).

# Hacking Web

- [Burp Suite](https://portswigger.net/burp) - Suite de herramientas de hacking web para probar y explotar vulnerabilidades en aplicaciones web (herramienta gráfica).
- [SQLMap](https://github.com/sqlmapproject/sqlmap) - Herramienta de automatización de inyección SQL para probar vulnerabilidades en bases de datos (herramienta de línea de comandos).
Ejemplo de uso: `sqlmap -u "http://example.com/?id=1" --dbms=mysql --dump` donde `http://example.com/?id=1` es la URL de la aplicación web vulnerable, `--dbms=mysql` indica el tipo de base de datos y `--dump` indica que deseas descargar toda la información de la base de datos.
- [OWASP ZAP](https://www.zaproxy.org/) - Proxy de seguridad web de código abierto que se puede utilizar para encontrar y explotar vulnerabilidades (herramienta gráfica).

# Misc



# OSINT

- [The Harvester](https://github.com/laramies/theHarvester) - Herramienta de recopilación de información que puede buscar correos electrónicos, nombres de usuario, hostnames, etc. en fuentes públicas (herramienta de línea de comandos).
Ejemplo de uso: `theharvester -d example.com -l 500 -b google` donde `example.com` es el dominio que deseas analizar, `-l 500` indica que deseas limitar la salida a 500 resultados y `-b google` indica que deseas usar la búsqueda de Google.
- [Maltego](https://www.maltego.com/) - Herramienta de investigación y análisis de enlaces para recopilar información y relaciones en línea (herramienta gráfica).

# Pwning

- [GDB](https://www.gnu.org/software/gdb/) - Depurador de código abierto que puede ser útil para analizar y explotar vulnerabilidades en binarios ejecutables (herramienta de línea de comandos).
- [IDA Pro](https://www.hex-rays.com/products/ida/) - Desensamblador y depurador que puede ser útil para analizar binarios ejecutables y encontrar vulnerabilidades (herramienta gráfica).
- [Pwntools](https://github.com/Gallopsled/pwntools) - Marco de explotación para binarios ejecutables que puede ser útil para crear exploits (herramienta de línea de comandos).
Ejemplo de uso: `python -c "from pwn import *; print(hexdump(asm(shellcraft.sh())))"` para crear un exploit simple que ejecute una shell en el objetivo.

# Reversing

- [Ghidra](https://ghidra-sre.org/) - Marco de ingeniería inversa de código abierto que puede ser útil para analizar binarios ejecutables (herramienta gráfica).
- [Radare2](https://github.com/radareorg/radare2) - Marco de ingeniería inversa de código abierto que puede ser útil para analizar binarios ejecutables (herramienta de línea de comandos).
Ejemplo de uso: `r2 archivo` donde `archivo` es el archivo binario que deseas analizar.
- [IDA Pro](https://www.hex-rays.com/products/ida/) - Desensamblador y depurador que puede ser útil para analizar binarios ejecutables y encontrar vulnerabilidades (herramienta gráfica).

# Tráfico de Red

- [Tcpdump](https://www.tcpdump.org/) - Herramienta de línea de comandos para capturar y analizar el tráfico de red en tiempo real (herramienta de línea de comandos).
Ejemplo de uso: `tcpdump -i eth0 tcp port 80` donde `eth0` es la interfaz de red y `tcp port 80` indica que deseas capturar el tráfico TCP en el puerto 80.
- [Scapy](https://scapy.net/) - Herramienta de manipulación de paquetes de red que puede ser útil para crear y enviar paquetes personalizados (herramienta de línea de comandos).
Ejemplo de uso: `sudo scapy` para iniciar Scapy en modo interactivo y luego `send(IP(dst="www.google.com")/ICMP())` para enviar un paquete ICMP a la dirección IP de Google.
- [Wireshark](https://www.wireshark.org/) - Analizador de tráfico de red que puede ser útil para encontrar y analizar paquetes específicos (herramienta gráfica).


