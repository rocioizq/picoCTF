# strings it

## **Descripción del Desafío**

* **Nombre:** strings it.
* **Link del reto:** [link](https://play.picoctf.org/practice/challenge/58).
* **Categoría:** General Skills.
* **Objetivo:** Encontrar la flag dentro de un archivo binario sin ejecutarlo.
* **Enunciado:** ¿Puedes encontrar la bandera en el archivo sin ejecutarlo?

## Metodología

1. **Descarga del archivo:**
   Utilicé `wget` para bajar el binario a mi espacio de trabajo:
   ```bash
   wget [https://mercury.picoctf.net/static/94d0015d06aa40d33301d5ab603417bc/strings](https://mercury.picoctf.net/static/94d0015d06aa40d33301d5ab603417bc/strings)
   ```
   Uso del comando strings: Dado que el archivo es un binario, utilicé strings para ver solo las cadenas de texto legibles.

2. **Uso del comando strings:**
    Dado que el archivo es un binario, utilicé strings para ver solo las cadenas de texto legibles.

3. **Filtrado con grep:** 
    Para no leer miles de líneas, filtré la salida buscando el formato estándar de la bandera:
    ```bash
    strings strings | grep "picoCTF"
    ```
4. **Flag encontrada:** 
    El comando me devolvió inmediatamente la flag.

![Flag encontrada](1.png)

## Herramientas Utilizadas
- Terminal de Linux (Webshell).
- Comandos: strings, grep, wget.

## Aprendizajes Clave
- Análisis estático básico: obtener información de un archivo sin correr el riesgo de ejecutarlo.
- Combinación de comandos mediante pipes (|) para agilizar búsquedas.