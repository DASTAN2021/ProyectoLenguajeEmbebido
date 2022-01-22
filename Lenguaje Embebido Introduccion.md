# SISTEMAS EMBEBIDOS

![Texto alternativo](https://1.bp.blogspot.com/-1vEGc7tXSM4/YMh2a_NIjnI/AAAAAAAAF60/gpR5X51Z3YEfopKMqGLU4o2zQS_lLgVhwCLcBGAsYHQ/s0/3770921.jpg)

## Introdución

¿Qué es un sistema Embebido?

 Sistema embebido “empotrado, incrustado o integrado” este sistema fue diseñado en una computadora para realizar funciones específicas, y cuyos componentes se encuentran integrados en una placa base. 
 Se lo lleva a cabo atraves de un microcontrolador, es decir, que se incluye en interfaces de entrada/salida, así como una memoria de tamaño reducido en el mismo chip.
Una vez diseñado el lenguaje se puede utilizar en tareas que impliquen una computación en tiempo real. 
Microprocesador, Microcontrolador, C/C++, Arduino, Raspberry, o sistemas en tiempo real en estos programas se pueden aplicar el lenguaje embebido. 

### Microcontroladores  
![Texto alternativo](https://eleycom.es/wp-content/uploads/2017/04/PICWEB.jpg)

- Funciones  específicas
- Sensores
- Tiempo  de  respuesta  mínimo

Microcontroladores: Han incorporado más capacidades que les permiten la interacción con el mundo físico en tiemporeal, además de mejores desempeños en ambientes de tipo industrial.

Sin embargo también se constató que el microprocesador por si  solo es inoperante, es necesario acompañarlo de los componentes necesarios para que pueda llevar acabo una determinada función.
Los componentes, deberám resolver problemas lógicos, de control, de direccionamiento, de tratamiento de buses, de almacenamiento de datos, de comunicación E/S, etc.

### Sistemas actuales 
En la actualidad,los procesadores se handesarrollado en relación a las aplicaciones.Por esta razón,los mi crocontroladores cuentan con periféricos internos para tener una interacción con el mundo real. Esporello, que secuenta:

- Pines digitales
- Conversores análogos - digitales y digitales - análogos
- Interrupciones
- Módulos de comunicación y visualización.

Cada pin del microcontrolador puede tener varios usos y está relacionado a los registros de trabajo que permiten configurarlo según la aplicación a realizar.

Video de refuerso:
[enlace en línea](https://www.youtube.com/playlist?list=PLg9EfzMaKPILl1Vkvoy93pmBi8JN6yKuF)

![Texto alternativo](https://i.pinimg.com/originals/cc/b2/f5/ccb2f5f1008b324e19add5295cc14e68.png)


## MÓDULOS DE COMUNICACIÓN
![Texto alternativo](https://i0.wp.com/www.zonamaker.com/images/contenido/impresora_3d/crea_impresora/3_electronica_imp/esquema_impresora.jpg)

Los  datos transmitidos por el puerto  serial pueden ser sometidos  aun formato de transmisión. Mas información en Arduino LanguageReference.
 una de  las impresoras  que se puede conectar con andruino  son  las computadoras  en 3D  con el andruino es mas  facil  armar una impresora 3D ya que esta lleva  cómo usa los periféricos usados (motores, display, botones, etc…).

Serial.begin() y el Serial.print() y su codificación detallamos a continuación 
## Serial.begin()
Rutina
para abrir el puerto serial
Junto a la apertura del puerto se
debe de definir la velocidad de
transmisión de datos.

### Sintaxis :

Serial.begin(SPEED)

SPEED: Velocidad en bits por
segundo.
## Serial.print
Esta rutina da inicio a la
transmisión de caracteres a través
del puerto serial.

### Sintaxis :
Serial.print
(VALOR)

VALOR:
cualquier tipo de dato,
desde cadenas hasta caracteres.

Aparte  de estos  codigos  va ya la programacion  para ello  se necesita una linea de codigo 

### blinkSerial.ino
Inicializa el puerto serial con una velocidad de transmisión de 9600 bits por
segundo. a continuacion se dara un extrato de la programacion:


int
led 13;

void
setup()
{

pinMode
(led OUTPUT);

Serial.begin
(9600)   //Inicializa el puerto serial con una velocidad de transmisión de 9600 bits por
segundo.

}

void
loop() {

Serial.print
("ALTO/n");

digitalWrite
(led,HIGH);

delay
(1000);

Serial.println
("BAJO"); // El uso de
Serial.println () nos ahorra la necesidad de
cadena enviada.
incluir el carácter de retorno de línea (“ \n”) en cada

digitalWrite
led LOW(led;low);

delay
(1000);

}

## ENTRADA DE COMUNICACION SERIAL

![Texto alternativo](https://3.bp.blogspot.com/-5n--UZFuAxM/WW7jPz0eIJI/AAAAAAAABEU/oTHSQ--e02ECHtaqxkUUtY91Zid74w5NwCLcBGAs/s1600/96.png)

comunicación serial puede ser utilizada para adquisición de datos, control, depuración de código, etc. El concepto de comunicación serial permite la transmisión- recepción bit a bit de un byte completo, este método de comunicación puede alcanzar mayores distancias.