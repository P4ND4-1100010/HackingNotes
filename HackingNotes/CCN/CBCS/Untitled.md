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

Indicaciones al a hora de configurar un host de máquinas virtuales:
* Últimas actualizaciones del SO.
* Última version disponible del sistema de virtualización.
* Tener al menos un adaptador de red en exclusiva para la infraestructura de virtualización.
* Crear un entorno de 