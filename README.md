## [iRis Warp 1.0.x]

## [1.0.2] - GENERAL- 2021-01-06 


### Agregado 

### Cambiado 
  - Script 311 por cambio de nombres en campos de tabla obrPaises
  - Script 312 por cambio de nombres en campos de tabla obrPaises
  
### Arreglado 
- No se cargaban correctamente los interpretes de las series ( https://sagai.jitbit.com/helpdesk/Ticket/34056536 )
- No se cargaban correctamente los interpretes en al hacer obra global ( https://sagai.jitbit.com/helpdesk/Ticket/34051060 )
- Se calculaba incorrectamente el pais debido a un cambio en el nombre de los campos de la table obrPaises (https://sagai.jitbit.com/helpdesk/Ticket/34079072) 

### Deprecado
- Script x0006  >  Actualizacion Entidad Pagadora
- Script @DuplicarObra

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
