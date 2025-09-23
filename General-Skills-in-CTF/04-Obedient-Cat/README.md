# Obedient Cat

## **Descripción del Desafío**

* **Nombre:** Obedient Cat
* **Categoría:** General Skills in CTF's
* **Objetivo:** Resolver un desafío introductorio aplicando técnicas básicas de reconocimiento, análisis de pistas y uso de comandos simples.
* **Enunciado:** Este archivo tiene una bandera visible (también conocida como "in-the-clear"). Y se descarga la bandera correspondiente.

## Metodología

1. **Descarga del archivo:**
   En la terminal de picoCTF, utilicé `wget` para descargar el archivo:

   ```bash
   wget https://artifacts.picoctf.net/c/123/obedient_cat.txt
   ```

2. **Listar archivos del directorio:**

   ```bash
   ls
   ```

   Esto me permitió ver todos los archivos presentes en el directorio.

3. **Identificación del tipo de archivo:**

   ```bash
   file flag
   ```

   Así determiné que el archivo era de tipo ASCII, y por lo tanto podía leerlo como texto plano.

4. **Lectura del contenido del archivo:**

   ```bash
   cat flag
   ```

5. **Flag encontrada:**
   Dentro del archivo se encontraba la bandera en el formato estándar de picoCTF.

## Herramientas Utilizadas

* Terminal online de picoCTF (Webshell)
* Comandos básicos: `ls`, `file`, `cat`

## Aprendizajes Clave

* Importancia de inspeccionar los archivos y entender su tipo antes de abrirlos.
* Reforzamiento del flujo básico para encontrar banderas: descargar → listar → identificar tipo → leer → registrar.
* Familiarización con comandos de Bash básicos en el contexto de CTFs.
