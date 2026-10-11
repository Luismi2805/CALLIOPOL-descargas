# CALLIOPOL — Guía completa de uso

**Documentación de la versión 2.3 · 11 de octubre de 2026.**

CALLIOPOL reúne ocho herramientas para trabajar con documentos, fotografías,
capturas web y mapas de relaciones desde un único menú. El procesamiento de
documentos se realiza en el equipo del usuario. Las opciones de búsqueda en
fuentes abiertas abren páginas externas cuando se utilizan.

Esta guía describe las funciones preparadas para la versión 2.3. Su ZIP todavía
está pendiente de publicación en GitHub. Las versiones anteriores pueden no
incluir todos los programas y opciones descritos.

## Índice de la guía

- [1. Qué programa utilizar](#1-qué-programa-utilizar)
- [2. Descargar y abrir la suite](#2-descargar-y-abrir-la-suite)
- [3. El lanzador CALLIOPOL](#3-el-lanzador-calliopol)
- [4. RECONOPOL: reconocimientos fotográficos](#4-reconopol-reconocimientos-fotográficos)
- [5. DILIPOL: modelos de diligencias y formularios](#5-dilipol-modelos-de-diligencias-y-formularios)
- [6. EXTRAPOL: extracción de texto y datos](#6-extrapol-extracción-de-texto-y-datos)
- [7. OCRPOL: texto buscable en documentos escaneados](#7-ocrpol-texto-buscable-en-documentos-escaneados)
- [8. FOLIAPOL: preparación de expedientes PDF](#8-foliapol-preparación-de-expedientes-pdf)
- [9. ANONIPOL: anonimización de PDF](#9-anonipol-anonimización-de-pdf)
- [10. NEXOPOL: mapas de relaciones](#10-nexopol-mapas-de-relaciones)
- [11. CAPTURAPOL: documentación de capturas web](#11-capturapol-documentación-de-capturas-web)
- [12. Cómo combinar los programas](#12-cómo-combinar-los-programas)
- [13. Datos, copias de seguridad y actualización](#13-datos-copias-de-seguridad-y-actualización)
- [14. Problemas frecuentes](#14-problemas-frecuentes)
- [15. Glosario sencillo](#15-glosario-sencillo)

## 1. Qué programa utilizar

| Necesidad | Programa |
| --- | --- |
| Preparar un reconocimiento fotográfico y su acta | RECONOPOL |
| Buscar y copiar modelos de diligencias o abrir formularios | DILIPOL |
| Extraer texto y datos de PDF y organizarlos en Excel | EXTRAPOL |
| Poder buscar y copiar texto en un PDF escaneado | OCRPOL |
| Ordenar PDF, añadir anexos y crear un expediente con índice, manifiesto y firma opcionales | FOLIAPOL |
| Eliminar datos o zonas de un PDF para preparar una copia anonimizada | ANONIPOL |
| Organizar elementos y relaciones en un mapa visual | NEXOPOL |
| Convertir una captura web guardada como imagen o PDF en un documento A4 con portada | CAPTURAPOL |

## 2. Descargar y abrir la suite

1. Abre la sección [Releases de CALLIOPOL](https://github.com/Luismi2805/CALLIOPOL-descargas/releases).
2. Comprueba el número de versión y descarga el ZIP portable de sus archivos
   adjuntos, llamados **Assets** en GitHub.
3. Descomprime todo el ZIP en una carpeta del equipo o de un pendrive.
4. Abre la carpeta descomprimida y haz doble clic en **CALLIOPOL.bat**.
5. Selecciona el programa que necesitas.

Para usar el portable no hace falta instalar Python ni Git. AutoFirma y los
controladores de la tarjeta sí son necesarios cuando se elige la firma
electrónica con tarjeta. Para ver Excel, Word o vídeos se necesita una aplicación
compatible con esos formatos.

Conserva la estructura completa. Por ejemplo, una distribución de la versión
2.3 puede organizarse así:

```text
CALLIOPOL 2.3/
├── CALLIOPOL.bat
├── CALLIOPOL/
│   ├── CALLIOPOL.exe
│   ├── suite_config.json
│   └── ... bibliotecas, recursos y datos de uso
└── apps/
    ├── RECONOPOL/
    ├── DILIPOL/
    ├── EXTRAPOL/
    ├── OCRPOL/
    ├── FOLIAPOL/
    ├── ANONIPOL/
    ├── NEXOPOL/
    └── CAPTURAPOL/
```

El archivo `.exe` de cada programa necesita sus bibliotecas, plantillas y demás
recursos. Para llevar la suite a otro equipo, copia toda su carpeta.

## 3. El lanzador CALLIOPOL

CALLIOPOL es el menú desde el que se abren las herramientas. Al pasar el ratón
por un botón aparece una breve explicación de su utilidad. Cada herramienta
se abre en su propia ventana.

Si aparece **no disponible**, el lanzador no encuentra el ejecutable previsto.
Comprueba que se haya extraído el ZIP completo y que la carpeta de esa aplicación
esté dentro de `apps`.

**Exportar diagnóstico técnico** genera un informe con la versión, información
del equipo y disponibilidad de los programas. No incorpora el contenido de los
expedientes. El mensaje indica dónde se ha guardado.

## 4. RECONOPOL: reconocimientos fotográficos

RECONOPOL ayuda a preparar un acta de reconocimiento fotográfico a partir de
fichas PDF o fotografías individuales.

### Uso básico

1. Abre **Datos del Acta**, completa los datos necesarios y guárdalos.
2. Utiliza **Importar fichas** para elegir o crear la carpeta del caso e
   incorporar las fichas PDF. El programa extrae las fotografías.
3. Si ya tienes las fotos separadas, utiliza **Importar Solo Fotos** y completa
   los datos asociados que solicite.
4. Abre **Previsualizar acta**, carga las fotografías y selecciona las que
   deben aparecer.
5. Revisa las imágenes y los datos y genera el acta final.

El acta admite hasta 12 fotografías con numeración consecutiva. La numeración
del acta es independiente del nombre de la fotografía. Se genera el PDF y un
archivo de texto con el detalle de las personas incluidas.

**Fichas/Fotos tratadas** permite acceder a las carpetas de trabajo. Antes de
utilizar el acta, comprueba que cada foto corresponde a los datos de la persona
prevista y que la extracción desde las fichas ha sido correcta.

## 5. DILIPOL: modelos de diligencias y formularios

DILIPOL organiza una biblioteca de modelos de diligencias y permite acceder a
formularios para abrirlos con la aplicación correspondiente.

### Uso básico

1. Navega por las carpetas o utiliza el buscador para localizar un modelo.
2. Selecciona la diligencia o abre un resultado de búsqueda para mostrar su
   contenido.
3. Prepara el texto que necesitas en el área de trabajo y pulsa **Copiar
   contenido** para llevarlo al documento que estés redactando.
4. Utiliza **Abrir carpeta de formularios** para acceder a los PDF y documentos
   de esa biblioteca.

También permite crear, renombrar y eliminar archivos y carpetas. Esas acciones
modifican la biblioteca de trabajo. Conserva una copia de tus modelos propios
antes de reorganizarla o actualizar el programa.

Los textos y formularios son materiales que el usuario debe revisar y adaptar
al caso concreto. Copiar un modelo no completa automáticamente sus datos.

## 6. EXTRAPOL: extracción de texto y datos

EXTRAPOL toma el texto de documentos PDF, lo organiza en Excel y ayuda a
localizar datos como teléfonos, correos, cuentas bancarias, usuarios y páginas
web. Sus búsquedas en fuentes abiertas se conocen como **OSINT**.

### Uso por fases

1. Pulsa **Seleccionar PDFs** y elige los documentos.
2. Ejecuta **Fase 0: Procesar Texto**. Esta fase crea la base que utilizarán
   las demás.
3. Ejecuta **Fase 1: Crear Excel** para obtener el texto completo organizado
   por documento y un resumen.
4. Ejecuta **Fase 2: Extraer Datos Clave** para generar un extracto de los
   documentos y una tabla con los datos identificados.
5. Ejecuta **Fase 3: Cruces OSINT** para agrupar y comparar datos coincidentes
   entre documentos.
6. Ejecuta **Fase 4: Resultados OSINT** para preparar las acciones de búsqueda
   disponibles para los datos encontrados.

En **OSINT Links** puedes filtrar por valor y hacer doble clic en una acción
para abrir su consulta en el navegador. **Actualizar Links** recarga la tabla.
Los botones para abrir los Excel se habilitan al generar los resultados.

La detección de coincidencias ayuda a organizar la información; no demuestra
por sí sola una relación entre personas. Las consultas externas pueden enviar
el dato buscado al servicio abierto en el navegador.

Si el PDF es una imagen escaneada y no tiene texto seleccionable, procésalo
antes con OCRPOL. Si cambias los documentos, vuelve a ejecutar la Fase 0.

## 7. OCRPOL: texto buscable en documentos escaneados

OCRPOL reconoce el texto visible de un PDF escaneado y añade una capa que
permite buscar palabras y copiar texto.

### Uso básico

1. Selecciona uno o varios PDF.
2. Elige las opciones de OCR disponibles.
3. Inicia el procesamiento y espera a que finalice cada archivo.
4. Abre el PDF de salida y comprueba que puedes buscar y seleccionar texto.

El modo habitual respeta las páginas que ya contienen texto. **Forzar OCR**
permite rehacer el reconocimiento existente. Los PDF se procesan uno tras otro;
un error en un archivo no impide continuar con los demás.

El programa crea archivos de salida con un nombre distinto, como
`documento_salida.pdf`, y añade un número si ese nombre ya existe. Si se cancela,
se elimina la salida parcial del archivo activo.

El portable incorpora el motor de reconocimiento y modelos de español e inglés.
El reconocimiento de otros idiomas depende de que estén disponibles sus modelos.
Revisa especialmente cifras, nombres, documentos de identidad y palabras poco
legibles: el OCR puede confundir caracteres.

## 8. FOLIAPOL: preparación de expedientes PDF

FOLIAPOL ordena documentos, crea anexos con separadores y los reúne en un
expediente. Puede añadir índice, numeración, manifiesto de integridad y firma.

### Datos permanentes

En **Datos de la unidad** guarda Comisaría, Unidad, Dirección, Teléfono y
Correo electrónico. Se reutilizan en los documentos que crea FOLIAPOL.

Estos campos son iguales a los de CAPTURAPOL, pero cada aplicación guarda su
propia configuración; completa los datos en ambas cuando las utilices.

### Preparar el expediente

1. Rellena **Diligencias judiciales**, cuando corresponda, y
   **DILIGENCIAS/OPERACIÓN**. Este último dato es obligatorio y determina el
   nombre del archivo de salida.
2. Pulsa **Añadir PDF** para incorporar documentos independientes. También
   puedes arrastrar varios PDF sobre la lista.
3. Pulsa **Añadir anexo** para crear un conjunto de documentos con título.
4. Selecciona un anexo y utiliza **Añadir PDF al anexo** para incorporar sus PDF.
5. Ordena los elementos mediante **Subir** y **Bajar**. Al seleccionar el
   título de un anexo se mueve todo el conjunto con sus documentos.
6. Activa las opciones que necesitas y revisa los cortes si utilizas división
   manual.
7. Pulsa **GENERAR EXPEDIENTE PDF** y elige la carpeta de destino.

Los anexos se numeran automáticamente en su orden actual. Al moverlos o quitar
uno, sus números se ajustan. Un anexo vacío debe completarse antes de generar.

### Índice y numeración

**Incluir índice general** añade un índice al principio, con los PDF, anexos
y páginas correspondientes. Los nombres largos se distribuyen en varias líneas.

Cuando hay índice, las páginas del cuerpo del expediente se numeran de forma
continua, incluidos separadores y manifiesto. Las hojas del índice quedan fuera
de esa numeración. Las referencias del índice corresponden a los números
impresos en el expediente, no a la posición de página que indique el visor PDF.
La numeración del cuerpo continúa aunque se generen varias partes.

### División en partes de hasta 10 MB

| Modo | Qué hace el usuario |
| --- | --- |
| Automático | Deja que el programa busque cortes por páginas completas para respetar 10.000.000 bytes por archivo. |
| Manual | Indica después de qué páginas cortar o las selecciona en «Elegir páginas». |

**Elegir páginas** presenta la posición de las hojas en el conjunto, incluidos
el índice y los separadores. Un doble clic marca un corte después de esa hoja.
Por ejemplo, `15, 32` termina las primeras partes después de las posiciones 15
y 32 del conjunto completo.

Un PDF de entrada de más de 10 MB puede incorporarse: sus páginas se reparten
entre partes. Si un corte manual crea una parte demasiado grande, el programa
solicita cambiarlo. Si una página sola supera el límite, el documento necesita
reducirse antes; no se parte una hoja por la mitad ni se empeora la imagen para
forzar el tamaño.

Cuando cambia el orden, se añaden o retiran documentos, o cambia la composición
del índice o del manifiesto, los cortes se borran. Vuelve a elegirlos después de
terminar esos cambios.

### Manifiesto de integridad

Activa **Incluir manifiesto de integridad** y rellena **Funcionario actuante**.
Se activa también el índice. El manifiesto utiliza los datos de la unidad y la
referencia de diligencias; si está vacía, utiliza DILIGENCIAS/OPERACIÓN.

Para cada PDF original incorporado recoge:

- Nombre del archivo.
- Tipo de archivo.
- Tamaño en bytes.
- Huella SHA-256.

Incluye tanto documentos independientes como documentos de los anexos. Los
archivos repetidos figuran en cada posición en la que se incorporan. Las huellas
corresponden a los mismos bytes que se utilizan para la unión.

El manifiesto se une como **última sección**, se incluye en el índice y participa
en la numeración. No se guarda como PDF aparte. Si el expediente se divide,
hay **un solo manifiesto** para todos los documentos del conjunto, al final de
las partes resultantes. Puede tener varias páginas y sus hojas respetan los
mismos cortes que el resto del expediente.

Una huella funciona como una identificación del contenido de un archivo.
Cambiar el contenido produce otra huella. El manifiesto identifica los PDF
originales, antes de unirlos; no contiene una huella del propio PDF final dentro
de él, porque añadirla cambiaría ese archivo.

### Firma del expediente

| Opción | Uso |
| --- | --- |
| Sin firma | Crea el expediente sin firma electrónica. |
| Firmar electrónicamente ahora | Solicita la firma con AutoFirma y la tarjeta. |
| Preparar para firma externa | Crea campos de firma vacíos para firmar después con otra aplicación. |

La firma o una imagen de firma activan el índice. El cuadro visible se coloca
después de su última entrada. Si falta espacio, pasa a una hoja de continuación
del índice.

**Añadir imagen de firma** admite PNG y JPEG, muestra una vista previa y permite
quitar la imagen. Puedes utilizar la imagen como representación visual sin firma
electrónica, o combinarla con la firma de la tarjeta. La imagen por sí sola no
protege el archivo mediante una firma electrónica.

Al firmar electrónicamente, primero se termina toda la preparación del expediente.
Después se firma el contenido completo de cada PDF final, incluido el manifiesto
que le corresponda. Si hay varias partes, se firman **todas**. El cuadro visible
queda en la parte que contiene el final del índice y las otras llevan firma
invisible. Una firma invisible protege igualmente el contenido de su archivo.

El programa reserva espacio para las firmas y comprueba el tamaño final. Si
alguna firma falla o se cancela, no se guardan las partes nuevas como expediente
terminado. En el modo externo los documentos siguen sin firma electrónica hasta
que se firme cada archivo con la aplicación elegida.

Para firmar con tarjeta necesitas AutoFirma instalado y los controladores de la
tarjeta. Selecciona el certificado de **FIRMA**, no el de autenticación. Introduce
el PIN únicamente en la ventana que lo solicite el firmador.

La comprobación incorporada verifica localmente que la firma corresponde al
contenido completo. No consulta la revocación ni acredita la confianza externa
en el certificado. La prueba de esta función de FOLIAPOL con la tarjeta del
usuario sigue pendiente; las comprobaciones automáticas usan certificados de
prueba.

Si un PDF de entrada ya tiene firma electrónica, la unión no conserva su validez
en el expediente resultante. Conserva el original firmado y firma el expediente
final una vez terminada la unión.

## 9. ANONIPOL: anonimización de PDF

ANONIPOL crea copias de PDF en las que elimina determinados datos o zonas.
Ofrece tres modos:

| Modo | Funcionamiento |
| --- | --- |
| Básico | Elimina automáticamente los datos que reconoce como sensibles. |
| Avanzado | Muestra los datos detectados, sus categorías y apariciones para elegir qué eliminar. |
| Manual | Permite recorrer las páginas y dibujar las zonas que se deben eliminar. |

### Uso básico

1. Selecciona uno o varios PDF.
2. Elige el modo.
3. Si lo necesitas, añade términos propios que deben localizarse.
4. En modo avanzado revisa y marca los datos concretos. En modo manual marca
   visualmente las zonas, incluidas fotos o firmas.
5. Genera la copia anonimizada y revísala página por página.

La detección incluye distintos datos de identidad, contacto, domicilio,
finanzas y dispositivos. No garantiza reconocer cualquier dato personal:
utiliza términos propios o el modo manual para lo que no aparezca detectado.

Cuando un escaneo no tiene texto buscable, utiliza el motor local de OCRPOL antes
de la detección automática. Los idiomas disponibles dependen de sus modelos.
La eliminación se hace sobre el contenido del PDF mediante redacciones, y se
limpian los metadatos. El original no se sobrescribe.

Antes de compartir la copia, comprueba que no queden datos identificativos en
texto, imágenes o zonas que no se hayan marcado.

## 10. NEXOPOL: mapas de relaciones

NEXOPOL organiza elementos encontrados en PDF en un mapa visual. Permite
mostrar fichas, incorporar imágenes y dibujar relaciones entre ellas.

### Uso básico

1. Crea un proyecto con **Nuevo** o recupera uno con **Abrir**.
2. Pulsa **Añadir PDF** para extraer elementos de documentos con texto.
3. Selecciona fichas y colócalas en el lienzo.
4. Utiliza **Relacionar** para elegir origen, destino y dirección de una flecha.
5. Selecciona una ficha y utiliza **Añadir imagen** o **Ajustar ficha** cuando
   necesites completar su presentación.
6. Guarda el proyecto con **Guardar** o **Guardar como**.
7. Exporta el lienzo a PNG o PDF para incorporarlo a otro documento.

Los elementos repetidos se agrupan por su valor normalizado y conservan sus
apariciones en los documentos de origen. Las flechas expresan las relaciones
que establece el usuario; la extracción de datos no confirma esas relaciones.

Puede trabajar con varios lienzos: **Nuevo lienzo con selección** crea uno a
partir de fichas seleccionadas; **Enviar a lienzo** incorpora fichas a otro
lienzo existente; **Organizar lienzo** distribuye las fichas. Hay desplazamiento
horizontal y vertical, selección de varias fichas, deshacer y rehacer.

El formato `.nexopol` permite continuar editando el proyecto. La exportación a
PNG o PDF conserva una representación del gráfico. Las imágenes asociadas a
fichas se referencian por su ubicación: conserva también esas imágenes al mover
el proyecto a otro equipo.

**Buscar** abre las opciones disponibles para consultar un elemento en fuentes
externas. NEXOPOL sigue en desarrollo; revisa los mapas y conserva el proyecto
editable además de su exportación. Para PDF escaneados sin texto, utiliza
OCRPOL antes de incorporarlos.

## 11. CAPTURAPOL: documentación de capturas web

CAPTURAPOL convierte una captura web ya guardada en un PDF A4 con portada.
Puedes usar FireShot u otra herramienta para obtener primero el archivo.

### Preparar la captura

1. Abre la página en el navegador y guarda la captura completa como imagen o
   PDF con la herramienta elegida.
2. Conserva ese archivo original en su ubicación.
3. Abre CAPTURAPOL y guarda en **Datos de la unidad** Comisaría, Unidad, Correo
   electrónico, Teléfono y Dirección.
4. En **Preparar captura**, pulsa **Seleccionar captura** y elige el archivo.
5. Utiliza **Revisar captura** para comprobar el contenido recibido.

Acepta PDF e imágenes compatibles, como PNG, JPEG, BMP y TIFF de una sola imagen.
Los PDF protegidos con contraseña se rechazan.

### Completar los datos y generar

1. Rellena **Diligencias / referencia**, **Funcionario actuante** y
   **Dirección de la página web**. La dirección debe empezar por `http://` o
   `https://`.
2. Revisa la **Fecha**, la **Hora** y la **Zona horaria / UTC**.
3. Comprueba **Herramienta de captura**, que propone FireShot, y añade
   observaciones si las necesitas.
4. Elige **A4 vertical** o **A4 horizontal** y si se numeran las hojas de captura.
5. Selecciona una modalidad de firma.
6. Pulsa **GENERAR PDF**, elige dónde guardarlo y revisa el resultado con
   **Revisar PDF**.

La fecha y hora iniciales se toman de la creación del archivo en Windows y se
pueden cambiar. Copiar o descargar un archivo puede modificar la fecha de
creación que registra el equipo: comprueba que la propuesta sea la adecuada.
El formato es día/mes/año y horas:minutos:segundos.

La portada utiliza el modelo incluido en el programa. Los datos se rellenan
como texto dentro del documento; el apartado de firma dispone de su cuadro
cuando se elige una modalidad que lo requiere. La portada incluye la huella
SHA-256 del archivo original seleccionado.

### Qué resultado se obtiene

Se genera **un único PDF** con la portada y la captura en hojas A4 consecutivas.
No se crea una copia adicional de la captura y el original no se modifica.
Si el nombre elegido ya existe, se utiliza otro nombre para evitar sobrescribirlo.

Las capturas largas se distribuyen sin perder ni repetir franjas. Los PDF
conservan el orden y las proporciones de sus páginas; las páginas muy largas
pueden ocupar varias hojas A4. Las anotaciones y formularios visibles se fijan
como parte del contenido del documento de salida.

CAPTURAPOL no aplica OCR ni crea texto buscable a partir de imágenes. No visita
la dirección web introducida ni archiva la página en Archive.org: documenta el
archivo que recibe y los datos aportados por el usuario.

### Opciones de firma

- **Sin firma:** genera el documento sin apartado de firma.
- **Firmar electrónicamente ahora:** utiliza AutoFirma y la tarjeta; se guarda
  el resultado después de firmar y comprobar que la firma cubre todo el PDF,
  aunque su cuadro visible esté en la portada.
- **Preparar para firma externa:** añade un cuadro y un campo de firma vacío
  para utilizar otra aplicación posteriormente. El archivo todavía no está
  firmado electrónicamente.

AutoFirma y los controladores deben estar instalados en el equipo. El PIN se
introduce en el firmador y no se guarda en CAPTURAPOL. La comprobación de firma
es local y no comprueba revocación ni confianza externa en el certificado.

El manifiesto del expediente se crea opcionalmente en FOLIAPOL, no en CAPTURAPOL.
La carga de una imagen de firma descrita en esta guía es una opción de FOLIAPOL;
CAPTURAPOL ofrece las tres modalidades anteriores.

## 12. Cómo combinar los programas

| Trabajo | Secuencia posible |
| --- | --- |
| Analizar PDF escaneados y organizar sus datos | OCRPOL → EXTRAPOL → NEXOPOL |
| Incorporar una captura web a un expediente | Herramienta de captura → CAPTURAPOL → FOLIAPOL |
| Preparar documentación con fotografías | RECONOPOL → FOLIAPOL |
| Obtener una copia del expediente sin determinados datos | FOLIAPOL → ANONIPOL, conservando el expediente original |

Los archivos se pasan de un programa a otro seleccionándolos en cada aplicación;
estas secuencias no se ejecutan automáticamente desde el lanzador.

Si vas a incluir una captura en FOLIAPOL, puedes generar primero el PDF en
CAPTURAPOL sin firma y firmar el expediente completo al terminar. Unir un PDF
firmado a otro expediente no mantiene válida su firma en el nuevo archivo.
Del mismo modo, anonimizar o modificar un documento firmado requiere conservar
el original y, si procede, firmar la copia resultante después de modificarla.

## 13. Datos, copias de seguridad y actualización

### Dónde se guardan los datos

Al abrir una herramienta desde CALLIOPOL, el lanzador le asigna carpetas de
datos, configuración, registros y temporales dentro de `user_data`. En la
estructura portable actual esa carpeta depende de la ubicación del lanzador:
normalmente está en `CALLIOPOL/user_data` dentro de la suite. Los PDF que
permiten elegir destino se guardan en la carpeta seleccionada por el usuario.

Si una aplicación se abre directamente por su `.exe`, puede utilizar su propia
ubicación de datos. Para mantener un uso consistente de las carpetas, abre las
herramientas desde el lanzador.

Conserva copias de los datos de la unidad, modelos personalizados, proyectos,
fotografías y documentos de salida. Copiar únicamente los ejecutables no
conserva necesariamente esos materiales.

### Actualizar una herramienta

Cada programa tiene su carpeta portable en `apps`. Esto permite actualizar una
herramienta sin reconstruir las demás.

1. Cierra la herramienta que vas a actualizar.
2. Guarda una copia de sus datos y configuración. Cualquier actualización del
   lanzador requiere conservar también sus datos de uso.
3. Utiliza el paquete completo de actualización suministrado para esa aplicación.
4. Sustituye la carpeta de programa indicada en ese paquete, conservando los
   datos y modelos propios de la instalación destinataria.
5. Abre la herramienta desde CALLIOPOL y comprueba que mantiene tus datos.

No basta con copiar el `.exe`: deben acompañarlo sus bibliotecas y recursos.
Si se añade una aplicación nueva, la configuración del lanzador debe incluirla.
El lanzador se actualiza por separado cuando cambia su código o interfaz.

Algunas herramientas utilizan otros componentes de la suite. Por ejemplo,
ANONIPOL utiliza el motor de OCRPOL para escaneos sin texto. Mantén esos módulos
disponibles y con versiones compatibles al repartir actualizaciones.

### Al compartir un portable

Prepara la distribución sin datos de expedientes, configuraciones personales,
proyectos ni registros de uso. Los programas trabajan localmente, pero las
búsquedas externas de EXTRAPOL y NEXOPOL abren servicios del navegador. Utiliza
las ubicaciones de trabajo y las copias de seguridad previstas para tus documentos.

## 14. Problemas frecuentes

| Situación | Comprobación o solución |
| --- | --- |
| Un programa aparece como no disponible | Comprueba que su carpeta completa esté en `apps` y que no falte su ejecutable. |
| El portable no abre después de copiarlo | Comprueba que copiaste toda la estructura y descomprimiste el ZIP antes de ejecutarlo. |
| AutoFirma no se encuentra | Comprueba su instalación. AutoFirma no viene incluido en la suite. |
| No aparece el certificado para firmar | Comprueba la tarjeta, sus controladores y la disponibilidad del certificado de FIRMA. |
| Se cancela la firma de una parte de FOLIAPOL | Repite la generación cuando puedas completar la firma de todas las partes. No se publican resultados nuevos a medias. |
| Un corte manual de FOLIAPOL supera 10 MB | Añade otro corte o mueve el corte anterior usando el orden completo de «Elegir páginas». |
| Una página sola supera 10 MB | Reduce previamente el documento de origen; la división por páginas no puede reducir una hoja que ya supera el límite. |
| FOLIAPOL no puede incorporar un archivo | Revisa el nombre y la ubicación que muestra el error y comprueba si el PDF está dañado o protegido. |
| No aparecen datos en EXTRAPOL o NEXOPOL | Comprueba que el PDF tenga texto seleccionable; si es un escaneo, utiliza OCRPOL primero. |
| EXTRAPOL no genera los Excel esperados | Ejecuta primero la Fase 0 con los documentos actuales y después la fase correspondiente. |
| La fecha propuesta por CAPTURAPOL no coincide con la captura | Revisa si el archivo se copió o descargó y cambia manualmente la fecha y la hora. |
| El manifiesto no aparece en un PDF separado | Es la última sección del expediente de FOLIAPOL y su entrada figura en el índice. |
| ANONIPOL no detecta un dato concreto | Añádelo a los términos propios o utiliza el modo manual y revisa el resultado. |

## 15. Glosario sencillo

| Término | Significado en esta guía |
| --- | --- |
| Portable | Programa preparado para ejecutarse desde su carpeta, con sus bibliotecas y recursos. Algunas funciones necesitan componentes externos, como AutoFirma. |
| Lanzador | Menú principal desde el que se abren los programas. |
| OCR | Reconocimiento del texto de una imagen o escaneo para poder buscarlo y copiarlo. |
| OSINT | Consulta de información en fuentes abiertas, como servicios y páginas web. |
| Hash o huella SHA-256 | Código calculado a partir del contenido de un archivo que ayuda a comprobar si ese contenido coincide con otro. |
| Manifiesto de integridad | Relación de los archivos incorporados y de sus huellas y tamaños. |
| Firma electrónica | Firma basada en un certificado que permite comprobar que corresponde al contenido del documento. |
| Firma invisible | Firma electrónica cuyo cuadro no se muestra en la página. Sigue protegiendo el archivo firmado. |
| Imagen de firma | Representación visual de una firma manuscrita; por sí sola no es una firma electrónica. |
| Firma externa | Firma que se realiza después de generar el PDF, utilizando otra aplicación. |

Consulta las [novedades de CALLIOPOL 2.3](NOVEDADES_2.3.md) para conocer los
cambios de esta actualización.
