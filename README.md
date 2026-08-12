

<div align="center">

# 📝 Prueba Práctica — Unidad IV
### Validación, Gestión, Herramientas y Estándares de Requisitos
**Ingeniería de Requisitos (ISR-401) — Evaluación Individual en Clase**

</div>

---


# 🔗 Acceso rápido

<div align="center">

### 📂 Repositorio

👉 **https://github.com/ptigasis-Alexander/Pruba_Practica_UND4_Tigasi_Sampedro**

### 📄 Documento PDF

👉 **[EvaluacionUnidad4.pdf](./EvaluacionUnidad4.pdf)**

### 📝 Código fuente LaTeX

👉 **[EvaluacionUnidad4.tex](./EvaluacionUnidad4.tex)**

### 📚 Referencias bibliográficas

👉 **[referenciasEV4.bib](./referenciasEV4.bib)**

</div>

Repositorio **público**, con el documento fuente en LaTeX, el PDF compilado y las imágenes/capturas de respaldo del intento rendido en el SGA.

---

## 📖 Qué contiene esta evaluación

Prueba práctica individual, en clase, de 120 minutos, sobre el caso **"Sistema de Gestión de Pedidos"**. Cubre las tres perspectivas de modelado y su validación:

| Punto | Contenido |
|---|---|
| P1 | Diagrama de clases UML (Cliente, Pedido, LíneaPedido, Producto) |
| P2 | Diagrama de actividades — proceso "Registrar pedido" |
| P3 | Máquina de estados (Registrado → Confirmado → Enviado → Entregado / Cancelado) |
| P4 | Matriz de consistencia entre P1–P2–P3 |
| P5 | Especificación de requisitos (RF1, RF2, RNF1, RNF2) con esquema de atributos |
| P6 | Priorización MoSCoW |
| P7 | Validación por inspección (ISO/IEC/IEEE 29148) + retrabajo de RNF2 |
| P8 | Pruebas de aceptación trazadas (PA1–PA4) |
| P9 | Matriz de trazabilidad |
| P10 | Gestión del cambio (SC-1) y línea base |

Incluye además las capturas de pantalla del resumen y del intento del cuestionario rendido en el SGA, embebidas en la carátula del PDF como evidencia.

---

## 📂 Archivos de este repositorio

| Archivo | Función |
|---|---|
| `EvaluacionUnidad4.tex` | Documento fuente LaTeX (carátula, P1–P10, anexos) |
| `EvaluacionUnidad4.pdf` | PDF ya compilado, listo para revisión/entrega |
| `referenciasEV4.bib` | Bibliografía (ISO/IEC/IEEE 29148, ISO/IEC 25010, Fagan, Pohl, SWEBOK, OMG UML) |
| `Imagenes_DCF_IR_LATEX/` | Capturas del SGA y escaneos de los diagramas manuscritos originales |
| `README.md` | Este documento |

---

## ⚙️ Cómo compilar el documento

El `.tex` usa `fontspec` y `tikz`, por lo que **requiere XeLaTeX o LuaLaTeX** (no compila con pdfLaTeX clásico). La bibliografía usa `natbib` + `bibtex`.

### Opción A — Overleaf (recomendada, sin instalar nada)

1. Crea un proyecto nuevo → **Upload Project** y sube el `.zip` del repositorio (o los archivos `EvaluacionUnidad4.tex`, `referenciasEV4.bib` y la carpeta `Imagenes_DCF_IR_LATEX/` con su contenido).
2. En **Menu → Compiler**, selecciona **XeLaTeX**.
3. Compila (▶). Overleaf ejecuta automáticamente el ciclo LaTeX → BibTeX → LaTeX → LaTeX necesario para que salgan bien el índice y las citas.

### Opción B — Local (TeX Live / MiKTeX)

```bash
# 1. Compilación inicial (genera el .aux con las citas pendientes)
xelatex EvaluacionUnidad4.tex

# 2. Procesa la bibliografía
bibtex EvaluacionUnidad4

# 3-4. Dos pasadas más para resolver referencias cruzadas, TOC y citas
xelatex EvaluacionUnidad4.tex
xelatex EvaluacionUnidad4.tex
```

Requisitos previos: distribución LaTeX completa (TeX Live `full` o MiKTeX) con los paquetes `fontspec`, `tikz`, `natbib`, `booktabs`, `longtable`, `tabularx`, `fancyhdr`, `titlesec`, `enumitem`, `parskip`, `hyperref`.

> **Nota:** las imágenes deben estar en `Imagenes_DCF_IR_LATEX/` con el nombre exacto (`ResumenCuestionarioSGA.png`, `CuestionarioSGA1.png`…`7.png`, `DiagramaClase.png`, `diagramaActividad.png`, `DiagramaMaquina.png`, `DiagrmaMaquinaEstadoCorregido.png`, `Hoja1.png`…`Hoja5.png`). Si falta alguna, el documento compila igual y muestra un recuadro "Imagen no encontrada" en su lugar, gracias al comando `\scanfig`.

---

## 🧪 Cómo verificar que compiló bien

- El PDF debe tener **portada + índice + 10 secciones (P1–P10) + Marco normativo + Anexos**, sin páginas en blanco inesperadas ni recuadros de "Imagen no encontrada".
- Revisa las citas bibliográficas del texto: deben verse como números entre corchetes (por ejemplo, 1). Si en su lugar aparecen signos de interrogación entre corchetes, falta correr bibtex o falta una pasada extra de xelatex.
- Confirma que el repositorio responde en GitHub:
  ```bash
  curl -I https://github.com/ptigasis-Alexander/Pruba_Practica_UND4_Tigasi_Sampedro
  ```
  Debe devolver `HTTP/2 200`.

---
---

## 🔒 Guía para guardar el trabajo de forma segura

1. **Compila y revisa el PDF antes de subirlo** — no subas un PDF a medio generar ni con errores de citas.
2. **Sube siempre el `.tex` fuente junto al `.pdf`**, no solo el PDF: así puedes recompilar si necesitas corregir algo después.
3. **No borres `Imagenes_DCF_IR_LATEX/`** — sin esas imágenes el documento no vuelve a compilar igual (las capturas del SGA son evidencia y no se pueden regenerar).
4. **Evita subir archivos auxiliares** (`.aux`, `.log`, `.out`, `.toc`, `.bbl`, `.blg`) al repositorio; agrégalos a un `.gitignore` para mantenerlo limpio:
   ```
   *.aux
   *.log
   *.out
   *.toc
   *.bbl
   *.blg
   *.fls
   *.fdb_latexmk
   *.synctex.gz
   ```
5. **Haz commit inmediatamente después de rendir el cuestionario en el SGA**, con las capturas ya incluidas, para que quede un respaldo con fecha verificable antes de la entrega.
6. **Guarda una copia local del PDF final** (fuera del repositorio, p. ej. en tu Drive) por si hay problemas de acceso a GitHub al momento de la revisión.

---

<div align="center">

## Universidad Técnica Estatal de Quevedo
### Facultad de Ciencias de la Ingeniería
### Carrera de Ingeniería de Software
### Ingeniería de Requisitos (ISR-401)

**Prueba Práctica — Unidad IV**
**Estudiante:** Tigasi Sampedro Paúl Alexander

---
⭐ **Documento elaborado con fines exclusivamente académicos.**

</div>
