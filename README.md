# CALLIOPOL

Suite portable de ocho aplicaciones para trabajar con documentos, expedientes,
fotografías, capturas web y mapas de relaciones desde un único lanzador.

El procesamiento de documentos se realiza localmente en el equipo. Las opciones
de consulta en fuentes abiertas abren páginas externas cuando se utilizan.

## Documentación de CALLIOPOL 2.3

- **[Novedades de la versión 2.3](NOVEDADES_2.3.md)**: CAPTURAPOL, mejoras de
  FOLIAPOL, manifiesto dentro del expediente, firma de todas las partes y
  actualización de cada portable por separado.
- **[Guía completa de CALLIOPOL](GUIA_CALLIOPOL.md)**: explicación de todos los
  programas, instrucciones paso a paso, ejemplos y problemas frecuentes.

## Descargar la versión publicada

**[DESCARGAR CALLIOPOL 2.3] [CALLIOPOL 2.3](https://github.com/Luismi2805/CALLIOPOL-descargas/releases/download/V.2.3/CALLIOPOL.2.3.zip)**

También puedes consultar todas las versiones en
**[Releases](https://github.com/Luismi2805/CALLIOPOL-descargas/releases)**.

1. Descarga el ZIP portable de la versión elegida desde sus archivos adjuntos
   (**Assets**).
2. Descomprime el ZIP completo.
3. Abre la carpeta descomprimida y ejecuta **CALLIOPOL.bat**.

No necesitas instalar Python ni Git para usar el portable. Para transportarlo,
copia toda su carpeta: los ejecutables necesitan sus bibliotecas y recursos.

## Programas de la suite 2.3

| Programa | Para qué sirve |
| --- | --- |
| RECONOPOL | Preparar reconocimientos fotográficos y sus actas. |
| DILIPOL | Buscar y copiar modelos de diligencias y acceder a formularios. |
| EXTRAPOL | Extraer texto y datos de PDF, organizarlos en Excel y preparar consultas en fuentes abiertas. |
| OCRPOL | Añadir texto buscable a documentos PDF escaneados. |
| FOLIAPOL | Ordenar y unir PDF en expedientes con anexos, índice, manifiesto de integridad y firma opcionales. |
| ANONIPOL | Preparar copias de PDF eliminando datos o zonas seleccionadas. |
| NEXOPOL | Organizar elementos y relaciones en mapas visuales. Sigue en desarrollo. |
| CAPTURAPOL | Convertir capturas web ya guardadas como imagen o PDF en documentos A4 con portada y firma opcional. |

FOLIAPOL puede crear un único manifiesto de todos los PDF originales incorporados
y unirlo al final del expediente, con su entrada en el índice. Puede firmar
electrónicamente todas las partes del resultado, con cuadro visible al final del
índice y firmas invisibles en las demás partes. Permite incorporar una imagen
de firma; una imagen por sí sola no constituye una firma electrónica.

CAPTURAPOL genera un único PDF final con portada y captura, sin guardar una copia
adicional del original. Recibe un archivo previamente capturado; no realiza por
sí mismo la captura del navegador ni la guarda en Archive.org.

Cada programa tiene su propio portable, que puede actualizarse sin reconstruir
los demás. Para actualizarlo se distribuye su carpeta completa y se conservan
los datos y la configuración del usuario.

## Firma con tarjeta

La firma electrónica de CAPTURAPOL y FOLIAPOL necesita **AutoFirma instalado en
Windows** y los controladores de la tarjeta. AutoFirma no viene dentro del
portable. El certificado de FIRMA se selecciona y el PIN se introduce en las
ventanas del firmador.

También puedes generar documentos sin firma o prepararlos para firmar con otra
aplicación. En este último caso siguen sin firma electrónica hasta que se firmen.

## Guía en vídeo

**[VER GUÍA DE CALLIOPOL](https://github.com/Luismi2805/CALLIOPOL-descargas/releases/download/v2.2/Guia_de_CALLIOPOL_2.mp4)**

El vídeo corresponde a una versión anterior. Para las funciones nuevas de la
2.3 consulta la guía escrita y las novedades enlazadas arriba.

## Antes de utilizar los resultados

Revisa los PDF, las fotografías, los datos extraídos y las copias anonimizadas
antes de utilizarlos. Conserva los originales y copias de tus modelos y
configuración. Las pruebas deben hacerse con documentos ficticios.
