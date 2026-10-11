# CALLIOPOL 2.3 — Novedades

**Fecha de documentación: 11 de octubre de 2026.**

CALLIOPOL 2.3 incorpora CAPTURAPOL, amplía la preparación de expedientes en
FOLIAPOL y permite actualizar cada programa portable por separado.

Estas notas describen la actualización 2.3. Su paquete portable todavía está
pendiente de publicación en GitHub. La última descarga publicada es la 2.2.1;
ese ZIP anterior no incorpora las novedades descritas aquí.

## Nueva aplicación: CAPTURAPOL

CAPTURAPOL prepara un documento A4 a partir de una captura de página web que el
usuario ya haya guardado con FireShot u otra herramienta compatible.

- Admite capturas guardadas como **imagen o PDF**.
- Distribuye las capturas largas en hojas A4 consecutivas, conservando su orden
  y proporciones. Permite elegir orientación vertical u horizontal.
- Añade una portada con los datos de la unidad, la referencia, el funcionario,
  la dirección web y los datos de la captura.
- Guarda los datos permanentes de Comisaría, Unidad, Correo electrónico,
  Teléfono y Dirección en un panel propio.
- Propone la fecha y hora de creación del archivo en Windows. El usuario puede
  modificarlas y revisar la zona horaria.
- Incluye en la portada la huella SHA-256 del archivo de captura original.
- Permite revisar la captura y el PDF generado y numerar las hojas de captura.
- Ofrece tres opciones: **Sin firma**, **Firmar electrónicamente ahora** y
  **Preparar para firma externa**.
- Genera **un único PDF final**, sin guardar una copia adicional de la captura
  ni modificar el archivo original.

CAPTURAPOL trabaja con el archivo recibido: no abre la página web, no realiza
por sí mismo la captura y no guarda la página en Archive.org. El manifiesto de
integridad del expediente se crea en FOLIAPOL.

## Mejoras de FOLIAPOL

### Anexos con numeración automática

Los anexos se numeran consecutivamente según su posición. Al mover o eliminar
un anexo, la numeración se actualiza. Seleccionar el título permite desplazar
el anexo completo, junto con todos sus PDF.

### División automática y manual

El expediente puede dividirse por páginas completas en archivos de hasta
**10 MB — 10.000.000 bytes — cada uno**.

- El modo automático busca cortes que respeten el límite de tamaño.
- El modo manual permite indicar después de qué páginas terminará cada parte.
- «Elegir páginas» muestra el orden completo, incluidos el índice, los
  separadores y el manifiesto seleccionado.
- Se admite un PDF de entrada de más de 10 MB: sus páginas pueden repartirse
  entre varias partes del expediente.
- Al cambiar la composición del expediente se borran los cortes anteriores
  para que el usuario pueda elegirlos de nuevo sobre el orden actualizado.
- Los errores al leer o incorporar un PDF identifican el archivo original y
  su ubicación.

Si una sola página supera el límite incluso guardada por separado, debe
reducirse previamente el documento de origen. La división conserva páginas
completas y no rebaja la calidad de las imágenes para forzar el tamaño.

### Manifiesto de integridad dentro del expediente

La opción **Incluir manifiesto de integridad** está desmarcada por defecto.
Al activarla se solicita el funcionario actuante y se incluye también el índice.

El manifiesto recoge, en orden de incorporación, el nombre, el tipo, el tamaño
en bytes y la huella SHA-256 de **todos los PDF originales incluidos**, tanto
independientes como pertenecientes a anexos. Si un mismo PDF aparece varias
veces, figura en cada posición correspondiente.

Se añade como **última sección del expediente**, aparece en el índice y participa
en la numeración continua. No se genera un PDF de manifiesto aparte. Cuando hay
varias partes, se mantiene **un único manifiesto** para todos los documentos
incorporados, situado al final del conjunto; puede ocupar varias hojas.

Las huellas corresponden a los archivos originales antes de unirlos. No se
incluye una huella del propio PDF final dentro de él: añadirla cambiaría el
archivo que se intenta identificar.

### Firma del expediente completo

FOLIAPOL ofrece las mismas tres modalidades de firma que CAPTURAPOL:

| Opción | Resultado |
| --- | --- |
| Sin firma | Genera el expediente sin firma electrónica. |
| Firmar electrónicamente ahora | Usa AutoFirma y el certificado de FIRMA de la tarjeta para firmar todos los PDF finales. |
| Preparar para firma externa | Añade un campo de firma vacío a cada PDF final para firmarlo después con otra aplicación. |

El cuadro visible se coloca **al final del índice**. Si falta espacio, el índice
continúa en otra hoja. La firma o una imagen de firma activan automáticamente el
índice.

Es posible añadir una imagen PNG/JPEG, verla previamente y quitarla. Puede
utilizarse sola como representación visual o junto con la firma electrónica.
**La imagen por sí sola no constituye una firma electrónica.**

Primero se termina la unión, el manifiesto, la numeración y la división. Después
se firma el contenido completo de cada PDF final. La parte que contiene el final
del índice lleva el cuadro visible; las otras partes llevan firmas invisibles.

Se reserva espacio para la firma antes de dividir y se comprueba el tamaño
final. Si una firma falla, se cancela o no cubre el archivo completo, no se guarda
ninguna de las partes nuevas como resultado terminado.

## CALLIOPOL y actualización de portables

El lanzador muestra una breve explicación al pasar el ratón sobre cada programa.

Cada aplicación tiene su propio portable dentro de `apps/<PROGRAMA>/`. Cuando se
modifica una herramienta, se puede reconstruir y distribuir únicamente su
carpeta completa. Las demás aplicaciones no necesitan recompilarse.

La lista de aplicaciones del lanzador se puede actualizar por separado. El
lanzador se recompila cuando cambia su propia interfaz o código.

Para transportar la suite completa se copia toda su carpeta. Para repartir
una actualización de una herramienta se copia su carpeta completa, incluyendo
bibliotecas y recursos; no basta con sustituir únicamente el `.exe`. Deben
conservarse los datos y la configuración de la instalación destinataria.

## Requisitos de firma

AutoFirma debe estar instalado en el equipo. No se incluye dentro del portable.
La tarjeta necesita sus controladores habituales y su certificado de FIRMA.
La selección del certificado y la introducción del PIN se hacen en las ventanas
del firmador; CALLIOPOL no almacena el PIN.

La comprobación incorporada verifica localmente que la firma corresponde al
contenido completo del archivo. No comprueba la revocación ni la confianza
externa en el certificado.

## Comprobaciones realizadas

- 67 pruebas automáticas superadas sobre CAPTURAPOL, FOLIAPOL, configuración y
  construcción modular.
- Revisión visual de índices cortos y de varias páginas con imagen de firma.
- Comprobación de firma de todas las partes con certificados de prueba.
- Comprobación de que una firma fallida no deja un expediente parcialmente
  publicado y de que se respetan los límites de tamaño finales.
- Arranque verificado del portable actualizado de FOLIAPOL y comprobación de
  que los demás ejecutables y el lanzador no cambiaron durante esa actualización.

La integración inicial de AutoFirma se probó con la tarjeta del usuario en
CAPTURAPOL. La firma nueva de FOLIAPOL todavía debe comprobarse con esa tarjeta.

Consulta la [guía completa de CALLIOPOL](GUIA_CALLIOPOL.md) para conocer los
programas y su uso paso a paso.
