# CALLIOPOL

Suite portable de nueve aplicaciones para trabajar con documentos, expedientes, fotografías, capturas web, vídeos y mapas de relaciones desde un único lanzador.

El procesamiento de documentos y vídeos se realiza localmente. Las consultas en fuentes abiertas acceden a servicios externos cuando se utilizan.

## Descargar

**[DESCARGAR CALLIOPOL — ÚLTIMA VERSIÓN](https://github.com/Luismi2805/CALLIOPOL-descargas/releases/latest)**

En la página de la release, descarga el **ZIP portable** disponible dentro de **Assets**.

1. Descarga el ZIP con nombre CALLIOPOL.2.4.zip al final de la página.
2. Descomprime todo su contenido.
3. Abre la carpeta descomprimida.
4. Ejecuta **CALLIOPOL.bat**.

**No necesitas instalar Python ni Git.** Para transportar la suite, copia toda su carpeta: los ejecutables necesitan sus bibliotecas y recursos.

## Novedades de CALLIOPOL 2.4

### VIDEOPOL — Calliopol Vídeo

Nueva aplicación para revisar grabaciones y preparar actas con los momentos relevantes.

Permite trabajar con hasta cuatro vídeos, marcar hitos, organizar fotografías individuales y grupos, añadir comentarios y marcas visuales, generar actas editables en Word y realizar volcados automáticos a PDF.

Al exportar el acta, crea también una carpeta con los fotogramas JPG numerados como en el documento. Los proyectos pueden guardarse para continuar el trabajo.

### CAPTURAPOL

El campo **«Página web o nombre» pasa a ser opcional** y admite texto libre. El documento propone el nombre **CAPTURA <nombre original>.pdf**, que puede modificarse al guardar.

Mantiene la generación de un único PDF A4 con portada y captura, huella SHA-256 y firma opcional, conservando el archivo original.

### EXTRAPOL

Mejora la extracción de los bloques **DENUNCIANTE** y **MANIFIESTA**, excluyendo el acta de derechos y sus anexos y corrigiendo identificaciones erróneas.

La extracción de texto y la generación de Excel se ejecutan en segundo plano, con progreso y errores por documento. También se corrigen caracteres que impedían guardar algunos Excel.

## Programas incluidos

| Programa | Para qué sirve |
| --- | --- |
| RECONOPOL | Preparar reconocimientos fotográficos y sus actas. |
| DILIPOL | Consultar modelos de diligencias y acceder a formularios. |
| EXTRAPOL | Extraer texto y datos de PDF, organizarlos en Excel y preparar consultas en fuentes abiertas. |
| OCRPOL | Añadir texto buscable a documentos PDF escaneados. |
| FOLIAPOL | Ordenar y unir PDF en expedientes con anexos, índice, división, manifiesto de integridad y firma opcionales. |
| ANONIPOL | Preparar copias anonimizadas de documentos PDF. |
| NEXOPOL | Organizar elementos y relaciones en mapas visuales. Sigue en desarrollo. |
| CAPTURAPOL | Convertir capturas web guardadas como imagen o PDF en documentos A4 con portada y firma opcional. |
| VIDEOPOL — Calliopol Vídeo | Revisar grabaciones, organizar hitos y fotogramas y generar actas Word y volcados PDF. |

## Documentación

- **[Guía de CALLIOPOL](GUIA_CALLIOPOL.md)**: instrucciones de las aplicaciones incluidas en la versión 2.3.
- **[Novedades de CALLIOPOL 2.3](NOVEDADES_2.3.md)**: incorporación de CAPTURAPOL y mejoras de FOLIAPOL.
- **[Todas las releases](https://github.com/Luismi2805/CALLIOPOL-descargas/releases)**: versiones y archivos de descarga.

## Guía en vídeo

**[VER GUÍA DE CALLIOPOL](https://github.com/Luismi2805/CALLIOPOL-descargas/releases/download/v2.2/Guia_de_CALLIOPOL_2.mp4)**

El vídeo corresponde a una versión anterior y no incluye todas las funciones incorporadas posteriormente.

## Firma electrónica

Las funciones de firma de CAPTURAPOL, FOLIAPOL y los PDF de VIDEOPOL requieren **AutoFirma instalado en Windows**, un certificado adecuado y, cuando corresponda, los controladores de la tarjeta.

AutoFirma no se incluye en el portable. También pueden generarse documentos sin firma o prepararlos para firmarlos posteriormente con otra aplicación.

## Datos y proyectos

Antes de sustituir una versión anterior, conserva una copia de tus datos y configuración.

En VIDEOPOL, conserva las carpetas de los proyectos, sus capturas y los vídeos originales. Guardar únicamente el archivo JSON no traslada el proyecto completo.

## Antes de utilizar los resultados

Revisa los documentos, fotogramas, datos extraídos y copias anonimizadas antes de incorporarlos a un expediente. Conserva los originales y realiza las pruebas con datos ficticios.
