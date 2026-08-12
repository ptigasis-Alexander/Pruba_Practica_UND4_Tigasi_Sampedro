

<div align="center">

# 📝 Prueba Práctica — Unidad IV

### Validación, Gestión, Herramientas y Estándares de Requisitos

**Ingeniería de Requisitos (ISR-401)**
**Evaluación individual en clase**

</div>

---

## 🔗 Acceso rápido

<div align="center">

### 📂 Repositorio público

👉 **[Pruba_Practica_UND4_Tigasi_Sampedro](https://github.com/ptigasis-Alexander/Pruba_Practica_UND4_Tigasi_Sampedro)**

### 📄 Documento PDF

👉 **[EvaluacionUnidad4.pdf](./EvaluacionUnidad4.pdf)**

### 📝 Código fuente LaTeX

👉 **[EvaluacionUnidad4.tex](./EvaluacionUnidad4.tex)**

### 📚 Referencias bibliográficas

👉 **[referenciasEV4.bib](./referenciasEV4.bib)**

</div>

---

## 📌 Descripción

Este repositorio contiene el desarrollo de la **Prueba Práctica de la Unidad IV** de la asignatura **Ingeniería de Requisitos (ISR-401)**, realizada individualmente a partir del caso:

> **Sistema de Gestión de Pedidos**

El trabajo comprende el modelado de datos, funciones y comportamiento del sistema, así como la especificación, priorización, validación, trazabilidad, gestión del cambio y configuración de requisitos.

También se incluyen las capturas del resumen y del intento del cuestionario realizado en el SGA, los diagramas UML y las hojas manuscritas utilizadas como evidencia.

---

## 👤 Información académica

| Dato          | Información                            |
| ------------- | -------------------------------------- |
| Universidad   | Universidad Técnica Estatal de Quevedo |
| Facultad      | Facultad de Ciencias de la Ingeniería  |
| Carrera       | Ingeniería de Software                 |
| Asignatura    | Ingeniería de Requisitos (ISR-401)     |
| Docente       | Ing. Gleiston Guerrero, Mg.            |
| Estudiante    | Tigasi Sampedro Paúl Alexander         |
| Modalidad     | Individual, en clase                   |
| Duración      | 120 minutos                            |
| Fecha         | 11 de agosto de 2026                   |
| Caso práctico | Sistema de Gestión de Pedidos          |

---

## 📖 Contenido de la evaluación

| Punto   | Actividad desarrollada                                                  |
| ------- | ----------------------------------------------------------------------- |
| **P1**  | Diagrama de clases UML con Cliente, Pedido, LíneaPedido y Producto      |
| **P2**  | Diagrama de actividades del proceso “Registrar pedido”                  |
| **P3**  | Máquina de estados del ciclo de vida de un pedido                       |
| **P4**  | Tabla de consistencia entre los modelos P1, P2 y P3                     |
| **P5**  | Especificación de dos requisitos funcionales y dos no funcionales       |
| **P6**  | Priorización de los requisitos mediante MoSCoW                          |
| **P7**  | Validación por inspección basada en ISO/IEC/IEEE 29148                  |
| **P8**  | Cuatro pruebas de aceptación trazadas a los requisitos                  |
| **P9**  | Matriz de trazabilidad hacia atrás, hacia adelante y horizontal         |
| **P10** | Solicitud de cambio, análisis de impacto, decisión del CCB y línea base |

---

## 📂 Estructura del repositorio

```text
Pruba_Practica_UND4_Tigasi_Sampedro/
│
├── EvaluacionUnidad4.tex
├── EvaluacionUnidad4.pdf
├── referenciasEV4.bib
├── README.md
│
└── Imagenes_DCF_IR_LATEX/
    ├── ResumenCuestionarioSGA.png
    ├── CuestionarioSGA1.png
    ├── CuestionarioSGA2.png
    ├── CuestionarioSGA3.png
    ├── CuestionarioSGA4.png
    ├── CuestionarioSGA5.png
    ├── CuestionarioSGA6.png
    ├── CuestionarioSGA7.png
    ├── DiagramaClase.png
    ├── diagramaActividad.png
    ├── DiagramaMaquina.png
    ├── DiagrmaMaquinaEstadoCorregido.png
    ├── Hoja1.png
    ├── Hoja2.png
    ├── Hoja3.png
    ├── Hoja4.png
    ├── Hoja5.png
    └── imagenes_README.md
```

---

## 📄 Función de los archivos

| Archivo o carpeta        | Función                                              |
| ------------------------ | ---------------------------------------------------- |
| `EvaluacionUnidad4.tex`  | Archivo principal con el código fuente LaTeX         |
| `EvaluacionUnidad4.pdf`  | Documento final compilado y listo para revisión      |
| `referenciasEV4.bib`     | Referencias bibliográficas utilizadas                |
| `Imagenes_DCF_IR_LATEX/` | Capturas del SGA, diagramas y evidencias manuscritas |
| `README.md`              | Descripción e instrucciones exactas de compilación   |

---

## ⚙️ Instrucciones de compilación

### Archivo principal

El archivo principal que debe compilarse es:

```text
EvaluacionUnidad4.tex
```

### Compilador requerido

El documento está configurado para compilarse con:

```text
pdfLaTeX
```

La bibliografía se procesa mediante **BibTeX** y el paquete `natbib`.

---

## ☁️ Opción A — Compilación en Overleaf

1. Descargue el repositorio desde GitHub mediante **Code → Download ZIP**.
2. Ingrese a Overleaf.
3. Seleccione **New Project → Upload Project**.
4. Suba el archivo `.zip` descargado.
5. Abra la opción **Menu**.
6. En **Main document**, seleccione `EvaluacionUnidad4.tex`.
7. En **Compiler**, seleccione **pdfLaTeX**.
8. Presione **Recompile**.
9. Verifique que el PDF se genere sin errores.

Overleaf realizará las pasadas necesarias para procesar el índice, las referencias cruzadas, las citas y la bibliografía.

---

## 💻 Opción B — Compilación local

Para compilar el proyecto localmente se necesita una distribución LaTeX completa, como **TeX Live** o **MiKTeX**.

Abra una terminal dentro de la carpeta principal del repositorio y ejecute los siguientes comandos, respetando el orden:

```bash
pdflatex EvaluacionUnidad4.tex
bibtex EvaluacionUnidad4
pdflatex EvaluacionUnidad4.tex
pdflatex EvaluacionUnidad4.tex
```

### Explicación del orden

1. La primera ejecución de `pdflatex` genera los archivos auxiliares y detecta las citas.
2. `bibtex` procesa las referencias contenidas en `referenciasEV4.bib`.
3. La segunda ejecución de `pdflatex` incorpora la bibliografía.
4. La última ejecución actualiza el índice, la numeración y las referencias cruzadas.

El archivo generado será:

```text
EvaluacionUnidad4.pdf
```

---

## 📦 Dependencias

El proyecto utiliza los siguientes paquetes de LaTeX:

* `inputenc`
* `fontenc`
* `babel`
* `float`
* `geometry`
* `amsmath`
* `amssymb`
* `xcolor`
* `longtable`
* `booktabs`
* `array`
* `calc`
* `graphicx`
* `hyperref`
* `fancyhdr`
* `titlesec`
* `enumitem`
* `parskip`
* `caption`
* `tabularx`
* `tikz`
* `natbib`

También se utilizan las siguientes bibliotecas de TikZ:

```text
shapes
arrows.meta
positioning
calc
fit
```

Se recomienda utilizar una instalación completa de TeX Live o MiKTeX para evitar errores por dependencias faltantes.

---

## 🖼️ Requisitos de las imágenes

La siguiente carpeta debe conservarse en la misma ubicación que el archivo principal:

```text
Imagenes_DCF_IR_LATEX/
```

Los nombres de las imágenes deben mantenerse exactamente como aparecen en el repositorio, respetando mayúsculas, minúsculas y extensiones.

### Capturas del cuestionario del SGA

```text
ResumenCuestionarioSGA.png
CuestionarioSGA1.png
CuestionarioSGA2.png
CuestionarioSGA3.png
CuestionarioSGA4.png
CuestionarioSGA5.png
CuestionarioSGA6.png
CuestionarioSGA7.png
```

### Diagramas UML

```text
DiagramaClase.png
diagramaActividad.png
DiagramaMaquina.png
DiagrmaMaquinaEstadoCorregido.png
```

### Evidencias manuscritas

```text
Hoja1.png
Hoja2.png
Hoja3.png
Hoja4.png
Hoja5.png
```

El documento utiliza la siguiente ruta para localizar las imágenes:

```latex
\graphicspath{{Imagenes_DCF_IR_LATEX/}}
```

Por este motivo, la carpeta no debe cambiarse de nombre ni moverse a otra ubicación.

El comando personalizado `\scanfig` muestra un recuadro con el mensaje “Imagen no encontrada” cuando falta una imagen utilizada mediante dicho comando. Sin embargo, las imágenes insertadas directamente con `\includegraphics` son necesarias para completar correctamente la compilación.

---

## ✅ Verificación del PDF

Después de compilar el documento, se debe comprobar que el PDF contenga:

* Portada con los datos de identificación.
* URL completa del repositorio en una sola línea.
* Captura legible del resumen del cuestionario del SGA.
* Capturas legibles del intento o evaluación del SGA.
* Índice del documento.
* Desarrollo completo de las actividades P1–P10.
* Marco normativo.
* Referencias bibliográficas.
* Anexos con diagramas y evidencias manuscritas.
* Numeración correcta de páginas, secciones, tablas y figuras.
* Tablas y diagramas dentro de los márgenes.
* Citas bibliográficas correctamente generadas.
* Todas las imágenes visibles.
* Ningún recuadro de “Imagen no encontrada”.

Las citas deben aparecer como números entre corchetes, por ejemplo:

```text
[1]
```

Si aparecen signos de interrogación como `[?]`, se debe repetir el ciclo completo:

```bash
pdflatex EvaluacionUnidad4.tex
bibtex EvaluacionUnidad4
pdflatex EvaluacionUnidad4.tex
pdflatex EvaluacionUnidad4.tex
```

---

## 🔍 Verificación del repositorio

El repositorio público se encuentra disponible en:

```text
https://github.com/ptigasis-Alexander/Pruba_Practica_UND4_Tigasi_Sampedro
```

También se puede verificar su disponibilidad mediante el siguiente comando:

```bash
curl -I https://github.com/ptigasis-Alexander/Pruba_Practica_UND4_Tigasi_Sampedro
```

El servidor debe responder con un código satisfactorio, normalmente:

```text
HTTP/2 200
```


---

## 📚 Referencias empleadas

El documento contiene referencias relacionadas con:

* ISO/IEC/IEEE 29148:2018.
* ISO/IEC 25010.
* Ingeniería de requisitos.
* Inspección formal de software.
* SWEBOK.
* Especificación UML de OMG.

Las referencias completas están disponibles en:

👉 **[referenciasEV4.bib](./referenciasEV4.bib)**

---

<div align="center">

## Universidad Técnica Estatal de Quevedo

### Facultad de Ciencias de la Ingeniería

### Carrera de Ingeniería de Software

### Ingeniería de Requisitos (ISR-401)

**Prueba Práctica — Unidad IV**

**Estudiante: Tigasi Sampedro Paúl Alexander**

---

⭐ **Documento elaborado con fines exclusivamente académicos.**

</div>
