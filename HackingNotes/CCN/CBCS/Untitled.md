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




