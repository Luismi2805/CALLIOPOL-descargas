# CALLIOPOL — Guía de uso

**Versión 2.4 · Actualizada el 1 de noviembre de 2026.**

CALLIOPOL reúne nueve herramientas para trabajar con documentos, fotografías, capturas web, vídeos y mapas de relaciones desde un único menú.

El procesamiento de documentos y vídeos se realiza localmente. Las consultas en fuentes abiertas abren servicios externos cuando se utilizan.

## Índice

- [1. Qué programa utilizar](#1-qué-programa-utilizar)
- [2. Descargar y abrir CALLIOPOL](#2-descargar-y-abrir-calliopol)
- [3. El lanzador](#3-el-lanzador)
- [4. RECONOPOL: reconocimientos fotográficos](#4-reconopol-reconocimientos-fotográficos)
- [5. DILIPOL: diligencias y formularios](#5-dilipol-diligencias-y-formularios)
- [6. EXTRAPOL: extracción de texto y datos](#6-extrapol-extracción-de-texto-y-datos)
- [7. OCRPOL: reconocimiento de texto](#7-ocrpol-reconocimiento-de-texto)
- [8. FOLIAPOL: preparación de expedientes](#8-foliapol-preparación-de-expedientes)
- [9. ANONIPOL: anonimización de documentos](#9-anonipol-anonimización-de-documentos)
- [10. NEXOPOL: mapas de relaciones](#10-nexopol-mapas-de-relaciones)
- [11. CAPTURAPOL: documentación de capturas](#11-capturapol-documentación-de-capturas)
- [12. VIDEOPOL: Calliopol Vídeo](#12-videopol-calliopol-vídeo)
- [13. Cómo combinar los programas](#13-cómo-combinar-los-programas)
- [14. Datos, copias y actualizaciones](#14-datos-copias-y-actualizaciones)
- [15. Problemas frecuentes](#15-problemas-frecuentes)
- [16. Glosario](#16-glosario)

## 1. Qué programa utilizar

| Necesidad | Programa |
| --- | --- |
| Preparar un reconocimiento fotográfico y su acta | RECONOPOL |
| Consultar modelos de diligencias y formularios | DILIPOL |
| Extraer texto y datos de PDF y organizarlos en Excel | EXTRAPOL |
| Buscar y copiar texto de un PDF escaneado | OCRPOL |
| Ordenar y unir PDF en un expediente con anexos, índice y firma opcional | FOLIAPOL |
| Preparar una copia anonimizada de un PDF | ANONIPOL |
| Representar elementos y relaciones en un mapa visual | NEXOPOL |
| Convertir una captura guardada como imagen o PDF en un documento A4 con portada | CAPTURAPOL |
| Revisar vídeos, organizar fotogramas y preparar actas o volcados automáticos | VIDEOPOL — Calliopol Vídeo |

## 2. Descargar y abrir CALLIOPOL

1. Abre la sección [Releases de CALLIOPOL](https://github.com/Luismi2805/CALLIOPOL-descargas/releases).
2. Selecciona la versión que quieras descargar.
3. En **Assets**, descarga el ZIP portable.
4. Descomprime todo su contenido.
5. Abre la carpeta **CALLIOPOL 2.4**.
6. Ejecuta **CALLIOPOL.bat**.

No necesitas instalar Python ni Git.

Para abrir los documentos exportados necesitarás aplicaciones compatibles con PDF, DOCX o XLSX. La firma electrónica requiere AutoFirma y, cuando se utiliza una tarjeta, sus controladores.

La estructura principal es:

```text
CALLIOPOL 2.4/
├── CALLIOPOL.bat
├── CALLIOPOL/
│   ├── CALLIOPOL.exe
│   ├── suite_config.json
│   └── ... bibliotecas y recursos
└── apps/
    ├── RECONOPOL/
    ├── DILIPOL/
    ├── EXTRAPOL/
    ├── OCRPOL/
    ├── FOLIAPOL/
    ├── ANONIPOL/
    ├── NEXOPOL/
    ├── CAPTURAPOL/
    └── VIDEOPOL/
```

**Conserva la carpeta completa.** Copiar únicamente los ejecutables deja fuera bibliotecas y recursos necesarios.

## 3. El lanzador

El lanzador muestra los botones de las aplicaciones. Al pasar el ratón sobre ellos aparece una explicación de su utilidad.

Pulsa un botón para abrir la herramienta correspondiente en una ventana independiente.

Si aparece **no disponible**, comprueba que se haya extraído el ZIP completo y que la aplicación conserve su carpeta dentro de `apps`.

**Exportar diagnóstico técnico** genera un informe sobre la versión, el equipo y la disponibilidad de los programas. No incorpora el contenido de los expedientes. El mensaje indica dónde se ha guardado.

## 4. RECONOPOL: reconocimientos fotográficos

RECONOPOL permite preparar actas a partir de fichas PDF o fotografías individuales.

### Uso básico

1. Abre **Datos del Acta**, completa los campos necesarios y guárdalos.
2. Utiliza **Importar fichas** para incorporar fichas PDF a la carpeta del caso.
3. Si ya tienes las imágenes separadas, utiliza **Importar Solo Fotos**.
4. Abre **Previsualizar acta**.
5. Carga y selecciona las fotografías que deben aparecer.
6. Revisa la composición y genera el acta.

El acta admite hasta doce fotografías con numeración consecutiva. Esa numeración es independiente del nombre de cada archivo.

Se genera el PDF y un archivo de texto con el detalle de las personas incluidas.

**Fichas/Fotos tratadas** permite acceder a las carpetas de trabajo. Comprueba siempre que cada fotografía corresponde a los datos previstos y que su extracción ha sido correcta.

## 5. DILIPOL: diligencias y formularios

DILIPOL organiza una biblioteca de modelos de diligencias y formularios.

### Uso básico

1. Navega por las carpetas o utiliza el buscador.
2. Selecciona un modelo para mostrar su contenido.
3. Prepara el texto que necesitas.
4. Pulsa **Copiar contenido** para llevarlo al documento que estés redactando.
5. Utiliza **Abrir carpeta de formularios** para acceder a los documentos de esa biblioteca.

También permite crear, renombrar y eliminar archivos y carpetas. Estas acciones modifican la biblioteca de trabajo.

Conserva una copia de los modelos personalizados antes de reorganizar o actualizar el programa. Revisa y adapta los textos al caso concreto.

## 6. EXTRAPOL: extracción de texto y datos

EXTRAPOL extrae texto de documentos PDF, lo organiza en Excel e identifica datos para facilitar su revisión y las consultas en fuentes abiertas.

### Uso por fases

1. Pulsa **Seleccionar PDFs** y elige los documentos.
2. Ejecuta **Fase 0: Procesar Texto** para preparar la base de trabajo.
3. Ejecuta **Fase 1: Crear Excel** para obtener el texto completo organizado por documento.
4. Ejecuta **Fase 2: Extraer Datos Clave** para generar el extracto y los datos identificados.
5. Ejecuta **Fase 3: Cruces OSINT** para agrupar y comparar coincidencias.
6. Ejecuta **Fase 4: Resultados OSINT** para preparar las acciones de consulta disponibles.

Los botones para abrir los Excel se habilitan cuando se generan los resultados.

### Qué información se analiza

La Fase 1 permite consultar el texto completo extraído.

La extracción de datos clave y las funciones de cruces y resultados OSINT se centran en los bloques **DENUNCIANTE** y **MANIFIESTA**. El acta de información de derechos y sus anexos quedan fuera de ese análisis.

Si el documento no contiene esos bloques reconocibles, el programa no utiliza automáticamente todo el documento como sustituto para las búsquedas.

### Progreso y errores

La extracción inicial y la generación de Excel se realizan en segundo plano. La ventana muestra el documento en procesamiento y los errores que se produzcan.

Un error en un PDF no impide continuar con los demás archivos del lote.

Si un PDF no tiene texto extraíble, utiliza OCRPOL y vuelve a incorporarlo. Cuando cambies los documentos, repite la Fase 0.

### Consultas OSINT

En **OSINT Links** puedes filtrar por valor y hacer doble clic en una acción para abrir la consulta en el navegador. **Actualizar Links** recarga la tabla.

Las coincidencias ayudan a organizar la información, pero requieren comprobación. Abrir una consulta puede enviar el dato buscado al servicio externo correspondiente.

## 7. OCRPOL: reconocimiento de texto

OCRPOL añade una capa de texto a documentos PDF escaneados para poder buscar palabras y copiar su contenido.

### Uso básico

1. Selecciona uno o varios PDF.
2. Elige las opciones de reconocimiento.
3. Inicia el procesamiento.
4. Espera a que termine.
5. Abre el resultado y comprueba que puedes buscar y seleccionar texto.

El modo habitual respeta las páginas que ya contienen texto. **Forzar OCR** permite rehacer el reconocimiento existente.

Los archivos se procesan uno tras otro. Un error no impide continuar con los demás.

Las salidas se guardan con un nombre distinto del original. Si el nombre ya existe, se añade un número. Al cancelar, se retira la salida parcial del archivo activo.

El portable incorpora modelos de español e inglés. Otros idiomas requieren sus modelos correspondientes.

Revisa especialmente cifras, nombres y documentos de identidad: el reconocimiento puede confundir caracteres.

## 8. FOLIAPOL: preparación de expedientes

FOLIAPOL reúne documentos PDF en un expediente y permite añadir anexos, separadores, índice, numeración, manifiesto de integridad y firma.

### Datos de la unidad

En **Datos de la unidad**, guarda Comisaría, Unidad, Dirección, Teléfono y Correo electrónico.

Cada aplicación conserva su propia configuración. Completa también estos datos en CAPTURAPOL o VIDEOPOL cuando los utilices.

### Preparar el expediente

1. Rellena **Diligencias judiciales**, cuando corresponda.
2. Completa **DILIGENCIAS/OPERACIÓN**. Es obligatorio y determina el nombre de salida.
3. Pulsa **Añadir PDF** para incorporar documentos independientes. También puedes arrastrarlos sobre la lista.
4. Pulsa **Añadir anexo** para crear un conjunto con título.
5. Selecciona el anexo y utiliza **Añadir PDF al anexo**.
6. Ordena los elementos con **Subir** y **Bajar**.
7. Selecciona las opciones de índice, división, manifiesto y firma.
8. Pulsa **GENERAR EXPEDIENTE PDF** y elige el destino.

Los anexos se numeran automáticamente. Al seleccionar su título puedes mover el conjunto completo con sus documentos.

### Índice y numeración

**Incluir índice general** añade una relación de documentos y anexos con sus páginas.

La numeración del cuerpo es continua e incluye separadores y manifiesto. Las hojas del índice quedan fuera de esa numeración.

Las referencias del índice corresponden a los números impresos, que pueden ser distintos de la posición indicada por el visor PDF.

### Dividir el expediente

El expediente puede dividirse por páginas completas en archivos de hasta **10.000.000 bytes**.

| Modo | Funcionamiento |
| --- | --- |
| Automático | El programa busca cortes que respeten el límite. |
| Manual | El usuario indica después de qué páginas debe terminar cada parte. |

**Elegir páginas** muestra las posiciones del conjunto completo, incluidos índice y separadores. Un doble clic permite marcar un corte.

Un documento de entrada mayor de 10 MB puede repartirse entre partes. Si una página sola supera el límite, debes reducir previamente el documento de origen.

Al cambiar la composición del expediente se borran los cortes anteriores. Elígelos después de terminar la organización.

### Manifiesto de integridad

Activa **Incluir manifiesto de integridad** y completa **Funcionario actuante**. Esta opción activa también el índice.

El manifiesto recoge, para cada PDF original:

- Nombre.
- Tipo de archivo.
- Tamaño en bytes.
- Huella SHA-256.

Incluye documentos independientes y documentos de los anexos.

Se incorpora como **última sección del expediente**, aparece en el índice y participa en la numeración. No se genera como PDF separado.

Si el expediente se divide, hay un único manifiesto para el conjunto, situado al final. Las huellas corresponden a los originales incorporados, antes de unirlos.

### Firma

| Opción | Resultado |
| --- | --- |
| Sin firma | Expediente sin firma electrónica. |
| Firmar electrónicamente ahora | Firma los PDF finales mediante AutoFirma. |
| Preparar para firma externa | Añade campos vacíos para firmar posteriormente. |

El cuadro visible se coloca al final del índice. Si hay varias partes, se firman todas; las restantes llevan firma invisible.

Si una firma falla o se cancela, no se guardan las nuevas partes como expediente terminado.

**Añadir imagen de firma** permite utilizar una imagen PNG o JPEG como representación visual. La imagen por sí sola no constituye una firma electrónica.

Para firmar con tarjeta, selecciona el certificado de **FIRMA** y escribe el PIN en la ventana del firmador.

La comprobación local verifica la correspondencia entre firma y contenido; no sustituye una validación de confianza y revocación del certificado.

Si incorporas un PDF ya firmado, conserva el original: su firma no se mantiene válida en el expediente generado mediante la unión.

## 9. ANONIPOL: anonimización de documentos

ANONIPOL prepara copias de PDF eliminando determinados datos o zonas.

| Modo | Uso |
| --- | --- |
| Básico | Eliminación automática de los datos reconocidos. |
| Avanzado | Revisión de datos detectados para elegir cuáles eliminar. |
| Manual | Selección visual de las zonas que deben eliminarse. |

### Uso básico

1. Selecciona los PDF.
2. Elige un modo.
3. Añade términos propios si necesitas localizar datos concretos.
4. Revisa los datos detectados o marca las zonas.
5. Genera la copia.
6. Comprueba el resultado página por página.

La detección automática no identifica necesariamente todos los datos. Utiliza términos propios o el modo manual para completar la revisión.

Para documentos escaneados sin texto buscable se utiliza el motor de OCRPOL.

La aplicación aplica redacciones sobre el contenido del PDF y limpia metadatos. El original no se sobrescribe.

Antes de compartir una copia, comprueba también imágenes, fotografías, firmas y otras zonas identificativas.

## 10. NEXOPOL: mapas de relaciones

NEXOPOL permite organizar elementos extraídos de documentos en fichas y representar relaciones en un mapa visual.

### Uso básico

1. Crea un proyecto con **Nuevo** o recupera uno con **Abrir**.
2. Utiliza **Añadir PDF** para incorporar documentos con texto.
3. Coloca las fichas en el lienzo.
4. Utiliza **Relacionar** para establecer origen, destino y dirección de las flechas.
5. Completa las fichas con **Añadir imagen** o **Ajustar ficha**.
6. Guarda el proyecto.
7. Exporta el mapa a PNG o PDF.

Los elementos repetidos se agrupan por su valor normalizado y conservan sus apariciones en los documentos de origen.

Las flechas representan relaciones establecidas por el usuario; la extracción no confirma por sí misma esas relaciones.

Puede trabajar con varios lienzos y permite organizar fichas, seleccionar varias, deshacer y rehacer.

Conserva el proyecto editable y las imágenes asociadas a las fichas. La exportación PNG o PDF contiene una representación del mapa.

**NEXOPOL sigue en desarrollo.** Revisa sus resultados y utiliza OCRPOL antes de incorporar documentos escaneados sin texto.

## 11. CAPTURAPOL: documentación de capturas

CAPTURAPOL convierte una captura previamente guardada como imagen o PDF en un documento A4 con portada.

### Preparar el archivo

1. Guarda la captura completa con FireShot u otra herramienta compatible.
2. Conserva el archivo original.
3. Abre CAPTURAPOL.
4. Completa y guarda **Datos de la unidad**.
5. En **Preparar captura**, pulsa **Seleccionar captura**.
6. Comprueba el contenido con **Revisar captura**.

Acepta PDF e imágenes compatibles. Los PDF protegidos con contraseña se rechazan.

### Completar los datos

1. Rellena **Diligencias / referencia** y **Funcionario actuante**.
2. Completa **Página web o nombre** si lo necesitas. Es opcional y admite texto libre.
3. Revisa fecha, hora y zona horaria.
4. Comprueba la herramienta de captura y añade observaciones.
5. Elige orientación vertical u horizontal y numeración.
6. Selecciona la modalidad de firma.
7. Pulsa **GENERAR PDF**.
8. Revisa el nombre propuesto y elige el destino.

El nombre inicial es **CAPTURA <nombre original>.pdf**. Puedes cambiarlo antes de guardar.

La fecha y hora se proponen a partir de la creación del archivo en Windows. Copiar o descargar el archivo puede cambiar esa fecha: revísala y corrígela cuando corresponda.

### Resultado

Se genera un único PDF con portada y captura distribuida en hojas A4. El original se conserva y no se crea otra copia adicional.

La portada incluye la huella SHA-256 del archivo original.

Las capturas largas se distribuyen en hojas consecutivas. En los PDF se mantienen el orden y las proporciones; una página larga puede ocupar varias hojas.

Si el nombre de salida ya existe, se utiliza otro para evitar sobrescribirlo.

CAPTURAPOL trabaja con el archivo recibido. La obtención de la captura se realiza previamente con la herramienta elegida.

### Firma

- **Sin firma:** genera el documento sin apartado de firma.
- **Firmar electrónicamente ahora:** utiliza AutoFirma y guarda el resultado después de comprobar la firma.
- **Preparar para firma externa:** incorpora un campo vacío para firmar posteriormente.

La firma electrónica corresponde al PDF completo, aunque el cuadro visible esté en la portada.

AutoFirma y los controladores de la tarjeta deben estar instalados. El PIN se introduce en el firmador y no se guarda en CAPTURAPOL.

## 12. VIDEOPOL: Calliopol Vídeo

VIDEOPOL permite revisar grabaciones, seleccionar fotogramas, organizarlos en un relato y generar actas o volcados automáticos.

### 12.1. Crear el proyecto

1. Abre **Calliopol Vídeo** desde el lanzador.
2. Pulsa **Nuevo**.
3. Utiliza **Añadir vídeos** para incorporar hasta cuatro archivos.
4. Espera a que termine la inspección inicial.
5. Utiliza **Nombrar cámara / datos horarios** para identificar las cámaras.
6. Guarda el proyecto.

La aplicación calcula la huella SHA-256 de los vídeos. Los archivos originales se conservan sin modificar.

### 12.2. Revisar las grabaciones

En **Cámaras y momentos**, cada cámara dispone de controles para:

- Reproducir y pausar.
- Avanzar o retroceder por fotogramas.
- Cambiar la posición de reproducción.
- Elegir velocidad.
- Controlar el silencio.
- Capturar un fotograma.
- Marcar un momento.
- Abrir la vista ampliada.

**Ampliar** abre la cámara en una ventana mayor que conserva los controles de revisión. Puedes volver con Esc, la X o el botón de retorno.

### 12.3. Revisar varias cámaras

Marca **Conjunta** en las cámaras que quieras controlar juntas.

Para ajustar grabaciones con horarios diferentes:

1. Pausa cada cámara en un mismo hecho reconocible.
2. Selecciona la cámara de referencia.
3. Pulsa **Alinear con cámara activa**.
4. Comprueba la correspondencia al reproducirlas.

Los desfases permiten coordinar las posiciones. Revisa su ajuste con un hecho común.

Volver a una marca actúa sobre la cámara correspondiente y desactiva la sincronización.

### 12.4. Marcar momentos y crear hitos

Un **hito** es un apartado del relato, como «Llegada», «Acceso al inmueble» o «Salida».

1. Sitúa la cámara en el momento relevante.
2. Pulsa **Marcar momento**.
3. Crea un hito o vincula la marca al que corresponda.
4. Continúa revisando y captura las imágenes necesarias.

Las capturas se asignan al hito activo de esa cámara según sus marcas. Al desplazarte hacia delante o hacia atrás, el hito activo puede cambiar.

Comprueba el hito de destino antes de capturar. Antes de la primera marca puede no haber un hito asignado.

### 12.5. Organizar fotografías y grupos

En **Organizador del acta** puedes preparar el orden del documento.

Las capturas nuevas se incorporan como fotografías individuales. Para reunir varias:

1. Selecciona las fotografías utilizando Ctrl o Mayús.
2. Pulsa **Crear grupo con seleccionadas**.
3. Escribe el comentario común.
4. Añade comentarios propios a las imágenes que lo necesiten.

También puedes:

- Añadir imágenes a un grupo existente.
- Separar fotografías de un grupo.
- Reordenar hitos, bloques e imágenes.
- Mover bloques a otro hito.
- Insertar texto libre.
- Comparar hasta cuatro capturas.

Un hito puede tener su comentario general. Los grupos admiten un comentario común y cada fotografía puede conservar el suyo.

Revisa el orden del árbol: será el utilizado para preparar el relato.

### 12.6. Añadir marcas gráficas

Selecciona una captura y abre **Marcas gráficas**.

Las herramientas permiten incorporar:

- Círculos.
- Recuadros.
- Flechas.
- Texto y etiquetas.
- Imágenes insertadas.

Puedes elegir color y tamaño de letra.

Para una imagen insertada:

1. Selecciona **Insertar imagen**.
2. Arrastra un recuadro y elige el archivo.
3. Utiliza **Seleccionar / mover** para desplazarla.
4. Arrastra un tirador de esquina para cambiar su tamaño manteniendo la proporción.

Las marcas se guardan en el proyecto sin modificar el vídeo original.

### 12.7. Generar el acta Word

1. Abre **Datos de la unidad y del acta**.
2. Completa los campos necesarios.
3. Guarda los datos permanentes de la unidad.
4. Revisa hitos, grupos, fotografías y comentarios.
5. Pulsa **Exportar Word**.
6. Elige el destino.
7. Abre y revisa el documento generado.

El acta se exporta en formato **DOCX editable** e incorpora la identificación de los vídeos y el relato organizado.

Incluye un anexo con una fotografía por página, a mayor tamaño.

Junto al acta se crea una carpeta con copias **JPG de los fotogramas**, numeradas como en el documento. Conservan los píxeles de las capturas y las marcas visibles.

El Word no se firma automáticamente. Revisa su contenido y maquetación con una aplicación compatible.

### 12.8. Realizar un volcado automático

El volcado obtiene fotogramas de intervalos definidos con una frecuencia en segundos.

1. Abre **Volcado automático**.
2. Selecciona el vídeo.
3. Indica inicio, fin y frecuencia.
4. Pulsa **Añadir intervalo**.
5. Repite la operación si necesitas más intervalos.
6. Revisa la previsión.
7. Selecciona la modalidad de firma.
8. Pulsa **Generar PDF**.

**Vídeo completo** rellena los límites con la duración de la cámara elegida.

Cada intervalo genera su propia acta PDF. Si hay varias, el programa solicita una carpeta de destino.

Por ejemplo, una frecuencia de diez segundos solicita una captura en cada posición prevista del intervalo. La extracción utiliza los fotogramas realmente disponibles; los saltos o huecos del archivo pueden afectar al resultado.

### 12.9. Firmar los PDF

Las opciones del volcado son:

- **Sin firma**.
- **Preparar para firma externa**.
- **Firmar con AutoFirma**.

La firma externa incorpora un campo vacío. El documento sigue sin firma electrónica hasta que se complete con otra aplicación.

La firma con AutoFirma requiere su instalación y el certificado correspondiente. Si falla, se conserva el PDF sin firmar para poder reintentar.

**Reintentar firma de PDF** permite seleccionar un documento preparado e intentar firmar una copia.

### 12.10. Guardar y recuperar el trabajo

Utiliza **Guardar** y **Abrir proyecto** para continuar el trabajo.

La aplicación realiza guardados automáticos y ofrece recuperación cuando corresponde.

Cada proyecto utiliza una carpeta con su información y sus capturas. Los vídeos originales se referencian por separado.

**Guardar el JSON en otra ubicación no traslada el proyecto completo.** Conserva también la carpeta de capturas y los vídeos.

Si un vídeo cambia de ubicación, utiliza **Localizar vídeo de cámara activa**. Se comprueba que su huella coincide antes de volver a vincularlo.

### 12.11. Informe de situación

En **Informe de situación** puedes revisar la disponibilidad de archivos y las incidencias.

Las opciones permiten:

- Actualizar el informe.
- Volver a comprobar vídeos y hashes.
- Comprobar todas las imágenes de los vídeos.
- Localizar un vídeo que se haya movido.

La inspección inicial y la lectura completa son comprobaciones diferentes. Un archivo puede abrirse inicialmente y presentar problemas en un punto posterior.

La compatibilidad depende del formato y la codificación de cada grabación. Los formatos propietarios de determinados sistemas CCTV pueden requerir una exportación compatible desde su aplicación de origen.

## 13. Cómo combinar los programas

| Trabajo | Secuencia posible |
| --- | --- |
| Analizar PDF escaneados | OCRPOL → EXTRAPOL |
| Preparar mapas a partir de documentos escaneados | OCRPOL → NEXOPOL |
| Incorporar una captura a un expediente | Herramienta de captura → CAPTURAPOL → FOLIAPOL |
| Incorporar un reconocimiento fotográfico | RECONOPOL → FOLIAPOL |
| Incorporar un volcado de vídeo | VIDEOPOL → FOLIAPOL |
| Incorporar el acta Word de vídeo | VIDEOPOL → revisión y exportación a PDF con una aplicación compatible → FOLIAPOL |
| Preparar una copia anonimizada del expediente | FOLIAPOL → ANONIPOL |

Estas secuencias se realizan seleccionando los archivos en cada herramienta. El lanzador no las ejecuta automáticamente.

Si vas a unir varios documentos y firmar el resultado, termina primero la composición y firma después el expediente final.

Conserva los originales firmados: unir, anonimizar o modificar un documento firmado afecta a su firma en el archivo resultante.

## 14. Datos, copias y actualizaciones

### Dónde se guardan los datos

Al abrir las herramientas desde el lanzador, los datos de uso se guardan normalmente dentro de:

```text
CALLIOPOL 2.4/CALLIOPOL/user_data/
```

Esta ubicación incluye carpetas de datos, configuración, registros y temporales para cada aplicación.

Los documentos que permiten elegir destino se guardan donde indique el usuario.

Abrir directamente el ejecutable de una herramienta puede hacer que utilice otra ubicación de datos. Utiliza el lanzador para mantener un funcionamiento consistente.

### Qué debes conservar

Realiza copias de:

- Datos y configuración de la unidad.
- Modelos y formularios personalizados.
- Proyectos.
- Fotografías y capturas.
- Vídeos originales.
- Documentos generados.

En VIDEOPOL conserva el conjunto del proyecto y sus archivos asociados. En NEXOPOL conserva también las imágenes vinculadas.

### Actualizar la suite

1. Cierra las aplicaciones.
2. Haz una copia de los datos, proyectos y modelos propios.
3. Descomprime la nueva versión en una carpeta independiente.
4. Conserva la versión anterior hasta comprobar el funcionamiento.
5. Recupera los datos y la configuración que correspondan, manteniendo sus rutas y archivos asociados.
6. Comprueba los proyectos antes de retirar la copia anterior.

### Actualizar una herramienta

Cada aplicación tiene una carpeta portable dentro de `apps`.

Cuando se distribuya una actualización individual, utiliza su carpeta completa y las instrucciones del paquete. El ejecutable debe acompañarse de sus bibliotecas y recursos.

Si se añade una aplicación, también debe estar incluida en la configuración del lanzador.

### Compartir una copia del programa

Prepara las distribuciones sin expedientes, proyectos, configuraciones personales ni registros de uso.

Mantén las copias de trabajo y de seguridad en las ubicaciones previstas para tus documentos.

## 15. Problemas frecuentes

| Situación | Qué comprobar |
| --- | --- |
| Un programa aparece como no disponible | Que conserve su carpeta completa dentro de `apps`. |
| El portable no abre después de copiarlo | Que se haya descomprimido todo el ZIP y copiado toda la estructura. |
| AutoFirma no se encuentra | Que esté instalado en el equipo. |
| No aparece el certificado de firma | La tarjeta, sus controladores y el certificado de FIRMA. |
| Un PDF escaneado no permite extraer datos | Procésalo primero con OCRPOL. |
| EXTRAPOL no genera los resultados esperados | Ejecuta de nuevo la Fase 0 con los documentos actuales. |
| EXTRAPOL no extrae datos de un documento con texto | Comprueba que contenga los bloques DENUNCIANTE y MANIFIESTA reconocibles. |
| Un corte de FOLIAPOL supera 10 MB | Añade o cambia los cortes. |
| Una página sola supera 10 MB | Reduce previamente el documento de origen. |
| El manifiesto no aparece como PDF separado | Está unido al final del expediente. |
| La fecha propuesta por CAPTURAPOL no coincide | Revisa si el archivo fue copiado o descargado y corrige fecha y hora. |
| CAPTURAPOL pide una página web | En la versión 2.4 el campo es opcional; comprueba que utilizas la versión actualizada. |
| Una captura de vídeo aparece en otro hito | Comprueba las marcas temporales de esa cámara y el hito activo. |
| Varias fotos deben compartir comentario | Selecciónalas y crea un grupo. |
| Una imagen insertada debe cambiar de tamaño | Selecciónala y arrastra uno de sus tiradores de esquina. |
| VIDEOPOL no encuentra un vídeo | Utiliza Localizar vídeo y selecciona el original correspondiente. |
| Un proyecto de vídeo no abre bien tras moverlo | Comprueba la carpeta de capturas, el JSON y las rutas de los vídeos originales. |
| Un vídeo no puede reproducirse | Comprueba su formato y codificación; puede requerir exportación desde el sistema de origen. |
| El Word necesita ajustes de presentación | Ábrelo con una aplicación compatible, revisa su maquetación y guarda los cambios. |
| ANONIPOL no detecta un dato | Añádelo como término propio o utiliza el modo manual. |

## 16. Glosario

| Término | Significado |
| --- | --- |
| Portable | Aplicación preparada para ejecutarse desde una carpeta con sus recursos. |
| Lanzador | Menú principal desde el que se abren las herramientas. |
| OCR | Reconocimiento del texto presente en imágenes o documentos escaneados. |
| OSINT | Consulta de información en fuentes abiertas. |
| Fotograma | Imagen correspondiente a un momento de un vídeo. |
| Hito | Apartado del relato al que se vinculan momentos y capturas. |
| Grupo | Conjunto de fotografías que puede tener un comentario común. |
| Intervalo | Tramo de vídeo definido por un inicio y un fin. |
| Desfase | Diferencia temporal utilizada para alinear varias grabaciones. |
| Hash o SHA-256 | Huella calculada a partir de los bytes de un archivo para comprobar su coincidencia. |
| Manifiesto de integridad | Relación de archivos con sus tamaños y huellas. |
| Firma electrónica | Firma basada en un certificado y vinculada al contenido del documento. |
| Firma invisible | Firma electrónica sin cuadro visible en la página. |
| Imagen de firma | Representación visual que por sí sola no constituye una firma electrónica. |
| Firma externa | Firma completada después de generar el PDF mediante otra aplicación. |

**Revisa siempre los resultados antes de incorporarlos a un expediente y conserva los archivos originales.**
