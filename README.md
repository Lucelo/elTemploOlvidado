# elTemploOlvidado

🚀 Proyecto Transversal de
Programación: "Tu Propia Aventura"
1. ¿Qué es este proyecto?
¡Hola a todos! A partir de esta semana, vamos a empezar el proyecto principal del módulo.
Vamos a construir, paso a paso, una Aventura Gráfica Interactiva.
La parte "común" será el motor del juego (la lógica), y la parte "personal" será vuestra
historia (el "skin").
Cada nueva Unidad Didáctica (POO, Ficheros, BBDD...) no será un tema aislado, sino una
nueva pieza que añadiremos al motor de vuestro juego para hacerlo más potente.
2. El Concepto: "Núcleo Común + Skin Personal"
Todas las parejas construiréis el mismo motor de juego, pero cada pareja diseñará su
propia historia.
El Núcleo (Lo que yo evalúo):
La lógica interna: cómo se gestiona el mapa, cómo se parsean los comandos, cómo se usa
un Array para las habitaciones, cómo se usa un Array para el inventario.
El Skin (Vuestra Creatividad):
La historia. ¿Tu juego va de escapar de un instituto? ¿De sobrevivir en una nave espacial?
¿De explorar una mazmorra (como el ejemplo de "Night Class")? Vosotros decidís:
● Las descripciones de las habitaciones.
● Los nombres de los objetos.
● El objetivo final del juego.
3. La Evolución del Proyecto (Fases del Motor)
● Fase 1 (UD1-UD3): El Motor Básico (¡ESTAMOS AQUÍ!)
○ Núcleo: if/else, switch, bucles y Arrays (UD3) para crear el mapa, gestionar
un inventario simple y colocar objetos en las salas.
○ Skin: Definir vuestra temática y crear las 3-4 primeras habitaciones y 2-3
objetos.
● Fase 2 (UD4-UD5): La Refactorización a POO (El Nivel 2)
○ Núcleo: ¡Aquí es donde refactorizaremos todo a POO! Crearemos las clases
Habitacion, Jugador, Objeto. Usaremos Herencia y Polimorfismo (inspirado
en el diseño de "Night Class", con ObjetosInventariables, Personajes, etc.).
○ Skin: Crear vuestros propios tipos de objetos y personajes.
● Fase 3 (UD6-UD7): El Inventario "Pro" y la Persistencia
○ Núcleo: Sustituiremos los arrays del inventario por Colecciones (ArrayList,
HashMap). Implementar el sistema de Guardar y Cargar Partida usando
Ficheros.
○ Skin: El motor ahora permite guardar. ¡Vuestro juego ya no se pierde!
● Fase 4 (UD8-UD9): La Aplicación Completa
○ Núcleo: Crear una Interfaz Gráfica (GUI) base y conectar el motor a una
Base de Datos (BBDD) con JDBC.
○ Skin: Diseñar vuestra propia GUI y BBDD (ej. para "Logros" o
"Puntuaciones").
5. ¿Cómo vamos a trabajar? (¡Importante!)
● EN PAREJAS: Formaréis parejas que se mantendrán, en principio, durante todo el
curso.
● 100% en Aula: Todo el desarrollo del proyecto se hará en nuestras horas de clase.
● Git: Usaremos Git desde el primer día. Cada pareja tendrá un solo repositorio
compartido. Ambos miembros deben hacer commits.
● Micro-Defensas: En cada entrega, no solo subiréis el código. La pareja saldrá y
elegiré a uno de los dos al azar para que me explique una parte del motor (la
lógica). Ambos debéis entender el 100% del proyecto.
6. ¿Cómo se va a evaluar?
Yo evalúo el Núcleo, no el Skin. Es decir, no evalúo si tu historia es buena, evalúo si tu
código es correcto, robusto y usa las estructuras que hemos visto (Arrays, POO,
Colecciones...).
Para cada Criterio de Evaluación (CE) (ej. "RA5.a - Usar arrays"), tendrás dos
oportunidades para demostrar que lo dominas:
1. El Examen Práctico de la UD: Una prueba individual y corta centrada en ese CE.
2. La Entrega del Proyecto: Donde demuestras (en pareja) que sabéis aplicar ese CE
en el motor de vuestro juego.
7. ¡A TRABAJAR! - Misión 1 (Entrega UD1-UD3)
Objetivo: Crear el esqueleto funcional del juego (el "Nivel 1") usando solo arrays y lógica
básica.
Fecha de Entrega:
Requisitos del "Núcleo" (Lo que se evalúa):
1. Repositorio Git: Cread un repositorio en GitHub y dadme acceso.
2. Clase Principal (Juego.java):
○ Debes mostrar una pequeña introducción al juego que ponga en situación al
jugador.
○ Un bucle while que mantenga el juego activo.
○ Un Scanner para leer los comandos del usuario.
○ El bucle debe terminar si el usuario teclea "salir".
3. Mapa Básico (con Arrays - RA5):
○ El mapa de habitaciones DEBE estar almacenado en un array (ej. String[]
habitaciones).
○ Una variable (ej. int habitacionActual = 0) debe controlar la posición del
jugador.
4. Inventario Básico (con Arrays - RA5):
○ El inventario del jugador DEBE ser un array (ej. String[] inventario = new
String[5];).
○ Las posiciones vacías deben contener null.
5. Objetos en Salas (con Arrays - RA5):
○ Debéis tener una forma de saber qué objetos hay en cada sala. (Pista:
podéis usar un array paralelo, ej. String[] objetosHabitacion0 = {"llave",
"nota"};, String[] objetosHabitacion1 = {"antorcha", null}; o una matriz String[][]
objetosMapa).
6. Parser de Comandos Básico (con switch o if-else - RA1):
○ Debe reconocer obligatoriamente los comandos:
■ ayuda muestra un listado con todos los comandos posibles y una
descripción de cada uno.
■ ir derecha, ir izquierda (modifica habitacionActual).
■ mirar (muestra la descripción de habitaciones[habitacionActual] y los
objetos que hay en esa sala).
■ coger [objeto] (busca el objeto en la sala, y si existe, lo añade al
primer hueco null del array inventario).
■ inventario (muestra los objetos del array inventario que no son null).
■ salir (termina el juego).
Requisitos del "Skin" (Vuestra parte creativa):
1. Decidid vuestra temática.
2. Escribid las descripciones de, al menos, 3 habitaciones para vuestro array
habitaciones.
3. Definid 2-3 objetos iniciales para vuestros arrays de objetos.
4. Aseguraos de que la conexión "izquierda/derecha" entre ellas tiene sentido en
vuestra historia.
