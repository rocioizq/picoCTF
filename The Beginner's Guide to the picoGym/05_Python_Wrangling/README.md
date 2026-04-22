# **Python Wrangling**

## **Descripción del Desafío**

**Nombre:** Python Wrangling

**Categoría:** General Skills

**Objetivo:** Ejecutar un script de Python utilizando los parámetros correctos para generar un archivo encriptado.

**Enunciado:**

Python scripts are invoked kind of like programs in the Terminal...

Can you run `ende.py` using `password.txt` to get `flag.txt.en`?

---

## **Metodología**

### **Exploración de archivos**

Primero listé los archivos disponibles:

```
ls
```

Identifiqué los archivos:

- `ende.py`
- `password.txt`
- `flag.txt`

---

### **Análisis del script**

Para entender cómo utilizar el script, revisé su contenido:

```
cat ende.py
```

Esto permitió identificar los parámetros necesarios para ejecutar el script.

---

### **Ejecución del script**

Ejecuté el script utilizando Python y los parámetros correctos:

```
python3 ende.py-e flag.txt password.txt
```

Esto generó el archivo `flag.txt.en`.

---

### **Obtención de la flag**

Una vez generado el archivo, lo abrí para visualizar su contenido:

```
cat flag.txt.en
```

Allí se encontraba la flag.

---

## **Herramientas Utilizadas**

- `python3` → Ejecución del script
- `cat` → Lectura de archivos
- `ls` → Listado de archivos

---

## **Aprendizajes Clave**

- Los scripts de Python pueden ejecutarse desde la terminal como programas.
- Es importante leer el código fuente para entender cómo utilizar un script.
- Los argumentos de entrada son clave para obtener el resultado esperado.