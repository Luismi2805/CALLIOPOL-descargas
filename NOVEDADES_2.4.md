# CALLIOPOL 2.4 — Vídeo, capturas web y extracción de documentos

CALLIOPOL 2.4 incorpora **VIDEOPOL (Calliopol Vídeo)** al lanzador y reúne las últimas mejoras de **CAPTURAPOL** y **EXTRAPOL**. La suite pasa a incluir **nueve aplicaciones portables** para trabajar localmente con documentos, expedientes, fotografías y grabaciones.

## Nueva aplicación: VIDEOPOL — Calliopol Vídeo

Una herramienta para revisar grabaciones y convertir los momentos relevantes en un relato organizado:

- Revisa hasta **cuatro vídeos**, con reproducción individual o conjunta, sincronización mediante desfases, avance por fotogramas y vista ampliada.
- Marca momentos y organízalos en **hitos**, con fotografías individuales, grupos y comentarios. Reordena el contenido antes de generar el acta.
- Añade flechas, círculos, recuadros, etiquetas e imágenes sobre las capturas. Las imágenes insertadas se pueden mover y redimensionar desde sus esquinas manteniendo la proporción.
- Genera **actas editables en Word**, con identificación de los vídeos, hitos, comentarios, fotogramas y un anexo con una imagen por página.
- Exporta junto al acta una carpeta de **fotogramas JPG**, numerados como en el documento y conservando los píxeles de las capturas.
- Realiza **volcados automáticos a PDF** por intervalos y frecuencia de captura, con un documento independiente para cada intervalo y opciones de firma.
- Guarda proyectos y permite continuar el trabajo. Calcula las huellas **SHA-256** de los vídeos y de las capturas.

El portable integra la **revisión 8** de Calliopol Vídeo. Los vídeos originales se conservan sin modificar; el Word es editable y no se firma automáticamente.

## CAPTURAPOL: portada y guardado más flexibles

- El campo **«Página web o nombre» es opcional**: admite texto libre, sin exigir una dirección con `http://` o `https://`.
- Propone **`CAPTURA <nombre original>.pdf`** como nombre del resultado y permite modificarlo al guardar.
- Mantiene la generación de un único **PDF A4 con portada y captura**, a partir de imágenes o PDF previamente guardados, con fecha y hora editables, huella SHA-256 y firma opcional.
- Conserva el archivo original y evita sobrescribir archivos existentes.

## EXTRAPOL: extracción más precisa y trabajo en segundo plano

- La extracción de datos y las búsquedas para cruces OSINT se centran en los bloques **DENUNCIANTE** y **MANIFIESTA**, excluyendo el acta de derechos y sus anexos.
- Mejora la delimitación del relato y evita incorporar cabeceras intercaladas o textos de cierre.
- Corrige identificaciones erróneas, como números de atestado tratados como teléfonos o referencias a L.E.Crim interpretadas como páginas web.
- La extracción inicial y la generación de Excel trabajan **en segundo plano**, con progreso por documento y errores visibles.
- Los errores de un archivo no interrumpen el resto del lote. Los PDF sin texto extraíble muestran una indicación para utilizar OCRPOL.
- La exportación a Excel elimina los caracteres de control que impiden guardar el archivo.

## Una suite con nueve programas

**RECONOPOL · DILIPOL · EXTRAPOL · OCRPOL · FOLIAPOL · ANONIPOL · NEXOPOL · CAPTURAPOL · VIDEOPOL**

Se mantienen las funciones de la versión 2.3, incluidos los anexos, el índice, la división de expedientes, el manifiesto de integridad y las opciones de firma de FOLIAPOL.

## Descarga y puesta en marcha

1. Descarga el **ZIP portable** desde los archivos adjuntos (**Assets**) de la release correspondiente.
2. Descomprime todo su contenido.
3. Abre la carpeta **CALLIOPOL 2.4** y ejecuta **CALLIOPOL.bat**.

**No necesitas instalar Python ni Git.** Para trasladar la suite, copia la carpeta completa, con sus ejecutables, bibliotecas y recursos.

Antes de sustituir una versión anterior, conserva una copia de tus datos y configuración. En VIDEOPOL conserva también las carpetas de los proyectos y los vídeos originales: guardar el JSON por separado no traslada todo el proyecto.

La firma electrónica requiere **AutoFirma**, el certificado y, cuando corresponda, los controladores de la tarjeta instalados en el equipo. AutoFirma no se incluye en el portable.

## Comprobaciones de esta distribución

Se han superado **105 pruebas automáticas**, comprobado el arranque del lanzador y de los nueve programas y probado la exportación de VIDEOPOL a Word y PDF con datos sintéticos.

El procesamiento de documentos y vídeos se realiza localmente. Las consultas OSINT abren servicios externos cuando se utilizan. Revisa siempre los resultados antes de incorporarlos a un expediente; NEXOPOL sigue en desarrollo.
