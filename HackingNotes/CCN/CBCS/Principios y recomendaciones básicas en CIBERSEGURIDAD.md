### Implementación de seguridad:
* Análisis de Riesgos
* Gestión de Riesgos
* Gobernanza
* Vigilancia
* Planes de Contingencia

### Amenazas que nos podemos encontrar
#### Ciberespionaje:
Origen:  Estados, industrias o empresas
Utilización: Normalmente ataques dirigidos (APT)
Víctimas: Sector público y privado
Objetivo: Ventajas políticas, económicas, estratégicas o sociales
Atribución: Enorme dificultad de atribución

##### APT (Advanced Persistent Thread)= Ataque dirigido
Buscan obtener la mayor cantidad de información útil sobre la víctima, con el objetivo de preparar un ataque lo más efectivo posible.

###### Parámetros característicos:
* Capacidad de Desarrollo: 
	 
	 Exploits y vulnerabilidades
	 
* Persistencia
* Cifrado
	
	Métodos de cifrado y fortaleza de claves para intercambiar la información exfiltrada.
	
* Técnicas de Exfiltración
	
	rootkit, bootkit
	
	**Rootkit**: Herramienta que sirve para ocultar actividades ilegítimas en un sistema. Una vez ha sido instalado, permite al atacante actuar con el nivel de privilegios del administrador del equipo.
	
* Ocultación
* Resistencia a Ingeniería inversa

###### Vectores de infección
* Web Exploit Kit
* Phising
* USB Drive Attack

###### Tipos de código dañino
* Ransomware

	Su objetivo es secuentrar datos de la víctima encriptándolos y pidiendo un rescate por ellos.

* Troyano
	
	Programa que realiza aparentemente una función útil
	
* Gusano

	Diseñado para copiarse y propagarse mediante mecanismos de red

* Rookit
	
	Colección de herramientas usadas para ocultar una intrusión
	
* Adware
	
	Genera publicidad en el equipo de la víctima
	
* Spyware
	
	Programas idependites y ejecutables. Se encargan de monitorizar el equipo de la víctima.

### Deep Web
Solo accesible desde determinados navegadores web.

#### La red TOR
Permite a los usuarios navegar por la web de forma anónima.
Los datos viajan a través de nodos.
Existe un directorio de nodos intermedios con claves públicas asociadas para poder establecer la comunicación cifrada.

Tor crea circuítos virtuales compuestos por tres nodos aleatoriamente escogidos de su red.
El elemento origen cifra la comunicación con la clave pública del último nodo de la ruta escogida.

#### BitCoin
Las transacciones se hacen a través de P2P
Cada transacción se guarda en una base de datos denominada BlockChain, sustentada por un Red de Mineros.
Permite transacciones de forma anónima.
Muy práctico para blanquear dinero y evadir impuestos.
### Aplicaciones

#### Buenas prácticas
* Trabajar con usuario sin privilegios
* No ejecutar programas de origen dudoso
* Desactivar ejecución automática de macros en los programas de ofimática.

#### Cifrado de datos
Significa convertir texto plano a texto ilegible (texto cifrado), evitando que la información sea accesible por personal no autorizado.

Se clasifican en 3 tipos de cifrado:
* Cifrado de disco
* Cifrado de carpetas
* Cifrado de documentos

#### Cortafuegos personales

Son programas que monitorizan las conexiones entrates y salientes del equipo.
Bloquean el acceso no autorizado al equipo permitiendo al mismo tiempo las comunicaciones autorizadas.
Lo más complicado de un firewall es su correcta configuración.

#### Aplicaciones antimalware

El código malicioso o malware puede provocar:
* Borrado o alteración de archivos
* Consumo de recursos
* Accesos no autorizados a archivos
* Infección remota de los equipos
* etc

Las funciones mínimas de una herramienta antimalware:
* Filtrado
* Protección
* Análisis

Las aplicaciones antimalware deben disponer de actualizaciones regulares y ser productos comerciales de confianza que permitan una combinación de los siguientes métodos:
* Escáner de acceso
	Escanea archivos cuando son abiertos
* Escáner de demanda
	Escaner bajo un calendario establecido
* Escáner de correos electrónicos
* Control de firmas
* Métodos heurísticos




#### Borrado seguro de datos
Deben realizarse diversas pasadas de escritura sobra cada uno de los sectores donde se almacena la información.
### Navegación segura y correo electrónico

El navegador web permite el acceso a la siguiente información:
* La IP pública con la que se conecta el usuario
* La resolución de pantalla
* El valor del campo "User-Agent"
* Qué páginas se leen y cuales no
* El idioma y zona GMT de SO.
* Si aceptan o no "cookies"
* Las fuentes del sistema y plugins intalados.

#### Navegación segura

Recomendaciones para una navegación segura:
* Acceder únicamente a sitios de confianza
* Mantener actualizado el navegador a la última versión disponible.
* Configurar el nivel de seguridad del navegador según sus preferencias
* Descargar los programas desde sitios oficiales para evitar suplantaciones maliciosas.
* Configurar el navegador para evitar ventanas emergente.
* Utilizar un usuario sin permisos de "adminitrador" para navegar por Internet e impedir la instalación de programas y cambios en los valores del sistema.
* Borrar las "cookies", los ficheros temporales y ele historial cuando se utilicen equipos ajenos para no dejar rastro de la navegación.
* Desactivar la posiblidad "script" en navegadores web.
* Hacer uso de HTTPS (SSL/TLS) frente a HTTP
* Emplear máquinas virtuales para navegar por internet

#### Correo electrónico

Recomendaciones:
* No abrir ningún enlace ni descargar ningún fichero adjunto de correos sospechosos.
* No confiar únicamente en el nombre del remitente.
* Fijarse en la extensión del fichero adjunto
* No habilitar macros de los documentos ofimáticos.
* No hacer clic en ningín enlace que solicite datos personales o bancarios.
* Tener siempre actualizado el SO, las aplicaciones ofimáticas y el navegador.
* Utilizar herramientas de seguridad para mitigar exploits de manera complementaria la software antivirus.
* Evitar hacer clic directamente en cualquier enlace desde el propio cliente de correo.
* Utilizar contraseñas robustas para el acceso al correo electrónico.
* Cifrar los mensajes de correo que contengan información sensible.

### Virtualización
La virtualización tiene la misma premisa que cualquier otro sistema, que es la minimización de la superficie de ataque.

Indicaciones a la hora de configurar un host de máquinas virtuales:
* Últimas actualizaciones del SO.
* Última version disponible del sistema de virtualización.
* Tener al menos un adaptador de red en exclusiva para la infraestructura de virtualización.
* Crear un entorno de laboratorio aislado del entorno de producción
* Disponer de un grupo de seguridad para gestionar la plataforma de seguridad.
* Proteger los dispositivos de almacenamientos en los que se guardan los archivos de recursos y definición de la máquina virtual.
* Mantener estrancos a los administradores de los guest respecto a los de host.

Indicaciones a la hora de configurar un guest:
* Hacer esquema previo de la infraestructura de virtualización
* Dimensionar la creación de máquinas virtuales a las necesidades reales y a los recursos de hardware disponibles en el host.
* Cifrar los ficheros de máquinas virtuales, instantaneas y discos duros virtuales destinados al almacenamiento de la platafaroma de virtualización.
* Instalar las últimas actualizaciones de seguridad en cada sistema operativo guest.
* Valorar la instalación de los agentes de hipervisor, tipo Guest Additions, y en caso de hacerlo, mantenerlos actualizados.
* Asegurar con antimalware y firewalls todos los sistemas operativos invitados.
* Conectar DVD, CD y medios externos solo cuando sea necesario y desactivarlos tras su uso.
* Mantener activas solamente las máquinas virtuales imprescindibles.
* Usar para la conexión con la red corporativo o con Internet una interfaz de red virtual diferenciada que de deberá desactivar cuando no se vaya a utilizar.
* Cifrar los medios de almacenamiento externos que contenga ficheros de virtualización de respaldo y custodiarlos convenientemente.

### Seguridad de Dispositivos Móviles y Redes Inalámbricas

#### Dispositivos móviles
Recomendaciones:
* Establecer un método seguro para desbloquear el terminal.
* Eliminar previsualización de los mensajes.
* Deshabilitar las conexiones innecesarias mientras no vayan a utilizarse.
* Mantener actualizado el software del dispositivo.
* Tener cuidado con el acceso y las solicitudes de permisos de las aplicaciones.
* Ignorar y borrar mensajes de origen desconocido que invitan a descargar contenidos o acceder a sitios web.
* Activar el acceso PIN a las conexiones Bluetooth y configurar el dispositivo en modo oculto.
* Descargar aplicaciones únicamente de las tiendas oficiales.
* Evitar realizar jailbreaking o rooting del terminal.
* Utilizar una VPN.
* Evitar en la medida de lo posible el uso de impresoras, faxes o redes WiFi públicas, salvo que se disponga de las herramientas necesarias para asegurar sus comunicaciones.
* Limpiar metadatos de imágenes.
* Separar comunicaciones personales de las profesionales.
* Implementar la gestión centralizada de dispositivos móviles mediante el empleo de agentes MDM (Mobile Device Management).

#### Redes inalámbricas
Recomendaciones:
* Cambiar la contraseña de acceso por defecto para la administración del Punto de Acceso.
* Modificar el SSID configurado por defecto no empleando nombres que pudieran identificar a la entidad y que permitan pasar desapercibidos.
* Activar el filtrado de direcciones MAC de los dispositivos WiFi para permitir que se conecten los dispositivos con las direcciones MAC especificadas.
* Configurar WPA2-AES en modo de confidencialidad de datos.
* Limitar la cobertura WLAN.
* Desconectar la red cuando no se utilice.
* Desactivar UPnP.
* Actualizar el "firmware" del router periódicamente.
* Usar direcciones IP estáticas o limitar el número de direcciones reservadas.
* Activar el cortafuegos del router.
* Activar la opción de registro para el router y analizar periódicamente el historial de accesos.
* Cambiar el DNS  que por defecto trae configurado el router (Usar uno como DNSCrypt).

### Mensajaría instantanea y redes sociales
#### Mensajería instantanea

Riesgos:
* Fallos a la hora de borrar las conversaciones almacenadas.
* Implicaciones de terner activa la copia de seguridad.
* Conexión a los servicios usando Wifi públicas o de dudosa procedencia.

Recomendaciones:
* Mantener el teléfono bloqueado.
* Eliminar la previsualización de los mensajes.
* Configuración de las aplicaciones
	
	Para solo recibir mensajes de las personas autorizadas.
	
* Desactivar la conectividad adicional del teléfono.
* Código abierto y revisado.

#### Redes sociales
El factor humano es el eslabón más débil.

Buenas prácticas para su uso:
* Creación cuidadosa del perfil y la configuración de privacidad.
* Reflexión sobre todo lo que se publica y emplear un pseudónimo.
* Emplear constraseñas complejas.
* Emplear autenticación en dos factores.
* Escoger cuidadosamente nuestros amigos.
* No permitir a las redes sociales examinar la libreta de direcciones de correo.
* Prestar atención a los servicios de localización y la información del teléfono móvil.
* Precaución con los enlaces.
* Escribir directamente la dirección de su sitio de redes sociales en el navegador.
* Tener precaución al instalar elementos adicionales.
* Revisar la información publicada.
*
### Internet de las cosas (IoT)
Red que interconecta miles de objetos físicos ofreciendo datos en tiempo real, convirtiendose en los sensores del mundo físico.
Cada vez más cirberdelincuentes emplean IoT para realizar ataques de denegación de servicio (DDoS). 

Aspectos de vital importancia:
* Seguridad.
* Interoperabilidad
* Manejabilidad de dichos sistemas.

Se debe establecer técnicas de monitorización y control para reducir la exposición al riesgo.

Se deberá:

* Cambiar las contraseñas por defecto.
* Mantener actualizados los dispositivos.
* Desactivar la conectividad remota cuando no se utilicen y mantener deshabilitados los componentes no necesarios.
* Mantener abiertos solo los puertos de comunicación que sean realmente necesarios y modificar los puertos de escucha si es posible.
* Si no permiten la configuración de seguridad, operar con ellos siempre en una LAN.
* Comprobar la visibilidad de los dispositivos en buscadores de dispositivos IoT.
* Asegurar la autenticidad, confidencialidad e integridad de todas las comunicaciones LAN.
* Comprobar periódicamente la configuración de seguridad.




### Política de seguridad
Es un conjunto de reglas que se deciden aplicar en las actividades del sistema y a los recursos de comunicaciones que pertenecen a una organización.
Las reglas incluyen: Seguridad física, personal, administrativa y de la red.
Define qué se desea proteger.



El diseño de una estrategia de seguridad depende de la actividad que se desarrolle en la empresa.

Pasos básicos para desarrollar una estrategia:

* Crear una política de seguridad
* Realizar un análisis de riesgos
* Aplicar las salvaguardas
* Concienciar a los usuarios
