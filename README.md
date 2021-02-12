## [iRis Warp 1.0.x]

## [1.0.9] - GENERAL- 2021-02-11

### Agregado 

### Cambiado
- Se mejoro la performance del divisor de emisiones para que funcione rapido via VPN ( https://sagai.jitbit.com/helpdesk/Ticket/34966863 )
- Se mejoro la performance al momento de filtrar un interprete por obra ( https://sagai.jitbit.com/helpdesk/Ticket/34407516 )
- Se modifico el formato del PDF a entregar a los socios, mostrando ahora los importes negativos asi como cambiando los nombres de las columnas ( https://sagai.jitbit.com/helpdesk/Ticket/34647693 )
- Se cambio el flujo de pesificacion de los socios. Se pesifica a las 5pm y se pasa a Softland a la noche. Ademas se cambiaron las etiquetas de los campos para que quede mas claro

### Arreglado 

### Deprecado

### Eliminado

## [1.0.8] - GENERAL- 2021-02-11

### Agregado 
- Reporte automatico de los martes de afip no pagar para socios (https://sagai.jitbit.com/helpdesk/Ticket/34822922)
  - Script: SOC001 - No pagar AFIP Saldo

### Cambiado

### Arreglado 

### Deprecado

### Eliminado


## [1.0.7] - GENERAL- 2021-02-08

### Agregado 

### Cambiado
- Error al generar archivo de revision ( https://sagai.jitbit.com/helpdesk/Ticket/34403297 ) 
  - Script: 0607  >  ImprimirRE
  - Script: 0607  >  ImprimirRE proceed

### Arreglado 

### Deprecado

### Eliminado


## [1.0.6] - GENERAL- 2021-01-19

### Agregado 

### Cambiado
- Se modifico el script 221 para excluir las liquidaciones que no esten asociadas a una obra ( https://sagai.jitbit.com/helpdesk/Ticket/34353707 ) 

### Arreglado 

### Deprecado

### Eliminado


## [1.0.5] - GENERAL- 2021-01-15

### Agregado 
- Se agrego un layout para que muestre los importes con dolarizacion ( https://sagai.jitbit.com/helpdesk/Ticket/34306701 ) 
- Se agrego un script "Export" en iris_warp_schedule para pasar las emisiones a legacy ( https://sagai.jitbit.com/helpdesk/Ticket/34251974 )
- Se agrego el campo exportado en ScheduleDB ( https://sagai.jitbit.com/helpdesk/Ticket/34251974 )

### Cambiado


### Arreglado 

### Deprecado

### Eliminado


## [1.0.4] - GENERAL- 2021-01-14

### Agregado 

### Cambiado
- Se renombro el script: "@Emisiones Interprete"  -->  "0266  >  Emisiones Interprete"
- Se cambio el comportamiento del dropdown de "ENTIDADES > Documentos" ( https://sagai.jitbit.com/helpdesk/Ticket/34182326 )
- Se agregaron los campos de comex_BancoPais en INX y Apo ( https://sagai.jitbit.com/helpdesk/Ticket/34280809 ) 
- Se modifico el script 1002  >  Sincronizar interpretes Subrutina y 1003  >  Enviar apoderados en interfaz ( https://sagai.jitbit.com/helpdesk/Ticket/34280809 )

### Arreglado 
- No exporta solo las emisiones de las obras marcadas ( https://sagai.jitbit.com/helpdesk/Ticket/34250327 ):
- Script: 0266  >  Emisiones Interprete
- Script 407 - Consolidacion de obras ( https://sagai.jitbit.com/helpdesk/Ticket/34101494 )


### Deprecado

### Eliminado


## [1.0.3] - GENERAL- 2021-01-07 

### Agregado
- 0501  >  MigrarDolarizacion ( https://sagai.jitbit.com/helpdesk/Ticket/33527224 )  y ( https://sagai.jitbit.com/helpdesk/Ticket/32234253 )

### Cambiado 
- Script 0501  >  MigrarObras ; para reparacion de contexto
- 0501  >  IniciarFusion ; para poder incorporar la fusion de dolares
- Revisiones entidades extranjeras ( https://sagai.jitbit.com/helpdesk/Ticket/33536864 ):
  - Script: 0601  >  NuevaRevision
  
### Arreglado 
- Emisiones desordenadas al exportar ( https://sagai.jitbit.com/helpdesk/Ticket/33827990 ):
  - Script: 0348  >  PDF Emisiones de Obra
  - Script: 0348  >  PDF Emisiones de Obra Sin Importes


### Deprecado


### Eliminado

## [1.0.2] - GENERAL- 2021-01-06 

### Agregado
- Layout: ÷ 0707 - LIQ - liquidacionDeDerechos - RepartoV5

### Cambiado 
 - Por cambió de nombres en campos de tabla obrPaises
   - Script 311
   - Script 318
   - Script 312 
   - Script 335
  
 - Para que vayan al layout que corresponde:
   - Script: @liquidarObraManual - creacionDePDF
   - Script: @liquidarObra - creacionDePDF
   - Script: Generar PDF Liq
   - Script: Z-99@liquidarObra - creacionDePDF de INXLIQ
   - Script: @liquidarObra - creacionDePDF INTERNACIONAL
   - Script: 0221 > Imprimir Derechos
   - Script: 0222 > PDF Liquidaciones Obras
   - Script: 0222 > PDF Obra
   - Script: 0234 > View Cta Cte Detail Copy
   - Script: 0342 > ExportarLQ
  
### Arreglado 
- No se cargaban correctamente los interpretes de las series ( https://sagai.jitbit.com/helpdesk/Ticket/34056536 )
- No se cargaban correctamente los interpretes en al hacer obra global ( https://sagai.jitbit.com/helpdesk/Ticket/34051060 )
- Se calculaba incorrectamente el pais debido a un cambio en el nombre de los campos de la table obrPaises (https://sagai.jitbit.com/helpdesk/Ticket/34079072)
- Se unificó el formato de los PDFs ( https://sagai.jitbit.com/helpdesk/Ticket/33835302 )
- Se agregó el valor obra en el PDF ( https://sagai.jitbit.com/helpdesk/Ticket/34040542 )
- Se sacaron del PDF las liquidaciones con importe menor a 0 ( https://sagai.jitbit.com/helpdesk/Ticket/33861037 )
- Si la persona tiene doble mandato o no entidad, se pone como No Pagar (99-5) ( https://sagai.jitbit.com/helpdesk/Ticket/32301118 )

### Deprecado
- Script x0006  >  Actualizacion Entidad Pagadora
- Script @DuplicarObra

### Eliminado
- Layout: ÷ 0707 - LIQ - liquidacionDeDerechos - PDF - Reparto
- Layout: ÷ 0707 - LIQ - liquidacionDeDerechos - PDF Internacional
- Layout: ÷ 0707 - LIQ - liquidacionDeDerechos - PDF Copy
- Layout: ÷ 0707 - LIQ - liquidacionDeDerechos - PDF OSX
- Layout: ÷ 0707 - LIQ - liquidacionDeDerechos - PDF

## [1.0.1] - GENERAL- 2021-01-05 

### Agregado 
Se hace script # x0045  >  EscribrirEntidadINX para actualizar a diario el campo Entidad Gestion.
  
### Cambiado 
Se mejoro la performance del campo Entidad Gestion.
Se audita el campo Entidad Gestion
Los reportes de Saldos salen totales o mayor o igual a $1 ( https://sagai.jitbit.com/helpdesk/Ticket/32264365 )

### Arreglado 
No se cargaban correctamente los no identificados ( https://sagai.jitbit.com/helpdesk/Ticket/34022001 ) y  ( https://sagai.jitbit.com/helpdesk/Ticket/34047163 )

### Deprecado
Script x0006  >  Actualizacion Entidad Pagadora
  

## [iRis Warp 1.0.0] - 2021-01-04 


Se accede mediante la aplicación Claris(FileMaker). Conexión mediante VPN a los servidores de SAGAI, desde el host 10.200.1.112 en el cual se encuentra la aplicación “Iris_warp”. 
El usuario debe: 

Conectarse a VPN (Previamente configurada por IT). 

Abrir aplicación de escritorio “Claris File Maker Pro”. 

Dirigirse a “Favoritos”. 

Hacer clic en “Añadir aplicación” y seleccionar “Desde anfitriones”. 

Hacer clic en el símbolo “+” al costado de la barra buscadora. 

Escribir el anfitrión:  10.200.1.112 y dar clic “Guardar”. 

En el costado izquierdo de la ventana aparecerá el host, hacer clic en el mismo.  

Se desplegarán todas las aplicaciones que pertenecen al anfitrión, buscar “iris_warp” y hacer doble clic. 

La aplicación ya está configurada en Favoritos para su rápido acceso.  


## [1.0.0] - GENERAL- 2020-12-18 


### Agregado 

Excluir manualmente un pago. (https://sagai.jitbit.com/helpdesk/Ticket/33734278) 

Se pone splash screen con la información del usuario y del sistema. 

  

### Cambiado 

Menues: reagrupados para que haya mayor consistencia. 

Se mejoro la performance del divisor de obras para que corra desde el servidor. 

Se implemento metodología de documentación de scripts. 

Agregar motivo de comentario interprete  
(https://sagai.jitbit.com/helpdesk/Ticket/32612357) 

Borrar Comentarios interpretes  
(https://sagai.jitbit.com/helpdesk/Ticket/32646798) 

Permitir consolidar las obras internacionales ignorando la falta de secuencias (https://sagai.jitbit.com/helpdesk/Ticket/33672620) 

  

### Arreglado 

Algunos no id mostraban por error un numero de socio. (https://sagai.jitbit.com/helpdesk/Ticket/33760736) 

  

### Eliminado 

Campos aa__disponible y aa__saldo que hacían referencia a la tabla de Aerolíneas Argentinas (deprecada). 

Campo c_cobroHE que se utilizaba para el envío de liquidaciones (deprecado).	 

Script 2002 > pasar lote (deprecado por cambio en el envío de liquidaciones). 

Script 2003 > porcentajes (deprecado por cambio en el envío de liquidaciones). 

Script 2004 > menores adultos (deprecado por cambio en el envío de liquidaciones). 

Script 2005 > apoderados (deprecado por cambio en el envío de liquidaciones). 

Script 2006 > propagar info (deprecado por cambio en el envío de liquidaciones). 

Script 2007 > propagarInfoFIX (deprecado por cambio en el envío de liquidaciones). 

Script 2008 > Send via Mandrill (deprecado por cambio en el envío de liquidaciones). 

Tabla RevSondeo (deprecado por el uso del PowerBI). 

0681 > Traer Datos First (deprecado por el uso del PowerBI). 

0682 > Traer Datos Revisiones (deprecado por el uso del PowerBI). 

0683 > Abrir Dashboard Revisiones (deprecado por el uso del PowerBI). 

0684 > Buscar Rango (deprecado por el uso del PowerBI). 

0685 > Buscar Año (deprecado por el uso del PowerBI). 

0686 > Buscar Totales (deprecado por el uso del PowerBI). 

0687 > Buscar Revisiones (deprecado por el uso del PowerBI). 

0688 > Mostrar Registros (deprecado por el uso del PowerBI). 

0689 > Imprimir (deprecado por el uso del PowerBI). 

0690 > ObtenerCambios (deprecado por el uso del PowerBI). 

Tabla Monday_boards (deprecado). 

0190 > Monday Sync (deprecado). 

0191 > Monday Obtener Boards (deprecado). 

0192 > Monday Obtener Pulses Obras (deprecado). 

0193 > Monday Obtener Pulses Series (deprecado). 

0194 > Monday Mandar Boards (deprecado). 

0195 > Monday Mandar Obras Loop (deprecado). 

0195 > Monday Mandar Obra (deprecado). 

0196 > Monday Mandar Series Loop (deprecado). 

0196 > Monday Mandar Serie (deprecado). 

AltaDiaria ( deprecado por baja a doppler ) 

 

 

## [1.0.0] - REPORTES - 2020-12-18 

 

### Agregado 

 

  

### Cambiado 

Se optimizaron los reportes para que corran por servidor y envíe un correo para informar el inicio y el fin del mismo. 

ADM000 - Listado saldos a pagar (total) 

ADM000 - Listado saldos a pagar (>30) 

ADM001 - Con saldo sin CUIT 

ADM002 - No pagar AFIP 

ADM003 - Difiere con AFIP 

ADM004 - Saldos Totales 

ADM005 - Comercio Exterior 

ADM006 - CUIT a revisar 

ADM007 - AFIP > 50K 

ADM008 - Interpretes comercio exterior 

ADM009 - Interpretes Disponibles 

LIQ001 - Obras Repartidas Historicas para Socios 

LIQ002 - Obras Duplicadas 

LIQ003 - Interpretes a no pagar 

LIQ004 - Exportar Listado de socios 

LIQ005 - Socios con liquidaciones 

LIQ006 - Listado de socios vivos 

LIQ007 - Listado de socios fallecidos 

LIQ008 - Detalle liquidado por Socio 

LIQ009 - Detalle liquidado por No Socios 

LIQ010 - Detalle liquidado por Representados 

LIQ011 - Detalle por Liquidacion de socios 

LIQ012 - Detalle por Liquidacion de No Socios y Representados 

LIQ013 - Obras que tienen apuntadores 

LIQ014 - Interpretes Duplicados 

LIQ015 - Obras abiertas 

LIQ016 - Obras con errores 

LIQ017 - Socios y sus Herederos 

LIQ018 - Interpretes No socios a cobrar 

LIQ019 - Obras a completar 

LIQ020 - Socios sin foto 

LIQ021 - Obras internacionales de los Interpretes (Excel) 

LIQ022 - Obras internacionales de los Interpretes (PDF) 

LIQ023 - Socios por Periodo 

LIQ023 - Socios por Periodo Proceed 

LIQ024 - Te estamos buscando 

LIQ025 - Listado Asamblea 

LIQ026 - Revisiones por status 

LIQ026 - Revisiones por status Proceed 

LIQ027 - Revisiones por periodo 

LIQ027 - Revisiones por periodo Proceed 

LIQ028 - Liquidaciones por anio 

LIQ028 - Liquidaciones por anio Proceed 

LIQ029 - Control Fichas (programas) 

LIQ030 - Control Programas 

LIQ031 - Control Novelas 

LIQ032 - Emisiones en proceso (Ingresa y Alerta) 

LIQ033 - Emisiones en proceso (alertas) 

LIQ034 - Emisiones en proceso (no ingresa) 

LIQ035 - Emisiones en proceso (vacias) 

LIQ036 - Control Primario 

LIQ037 - Emisiones Ingresan 

LIQ038 - Emisiones por canal 

LIQ039 - Programas por canal 

LIQ040 - Programas sin actores 

LIQ041 - Programas Totales 

LIQ042 - Exportar listado de socios vivos 

LIQ043 - Revisiones completa 

  

### Arreglado 

  

### Eliminado 

 

## [1.0.0] - DOBLAJE- 2020-12-18 

 

  

### Agregado 

Se permite que en la ficha de doblaje se pueda cargar un mismo interprete que en la ficha de “cuerpo”. 

 

  

### Cambiado 

Estructura en la tabla obrMatriz;  

Estructura en la tabla obrFicha;  

Estructura en la tabla LIQ 

Script 0308 > Eliminar Multiple 

Script 0318 > Obra Apertura 

Script 0318 > Obra Cierre 

Script 0318 > Ficha Cierre Imagen 

Script 0318 > Ficha Apertura 

Script 0339 > controlModificaciones (Warp) 

Script 0339 > Revision Cambio Interprete (Warp) 

Script 0339 > RevisionCambioSecuencias (Warp) 

Script 0339 > RevisionEliminarInterprte (Warp) 

Script 0339 > RevisionNuevoInterprete (Warp) 

Script 2000  >  liquidarObra - VP + liquidar (warp) 

Script 2000  >  Calcular VP (warp) 

  

### Arreglado 

  

### Eliminado 

 

 

## [1.0.0] - INTERNACIONAL- 2020-12-18 

 

### Agregado 

 

### Cambiado 

Comentarios Internacionales  
(https://sagai.jitbit.com/helpdesk/Ticket/31942858) 

Comentarios de entidades  
(https://sagai.jitbit.com/helpdesk/Ticket/31942858) 

Numero de obra declarado por la entidad  
(https://sagai.jitbit.com/helpdesk/Ticket/31980407) 

 


### Arreglado 
 

### Eliminado 

 

 

## [UNRELEASED]  

 

Saldos negativos son No Pagar. 

Categoría de interprete. 

Menores con CBU, se les paga. 

Pesificar importes mayores a 10 centavos. 

Conectar el listado de Socios a MailChimp. 
