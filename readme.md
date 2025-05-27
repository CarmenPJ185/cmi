## MILKY WAY

Proyecto de Creación Multimedia Interactiva de la  Facultad de Bellas Artes de la Univesidad de Granada



# 1 Datos 



**Titulo** : Milky Way

**Web:**   https://possummind.itch.io/milky-way

**Autor:**  Carmen Pérez Jiménez

**Resumen** : Se ha agotado la leche en toda la galaxia, por ello se busca un granjero que pueda ir a todos los planetas para poder ordeñar las vacas, para ello, necesitará habilidad, precisión y un buen sentido del ritmo. Deeberás viajar de planeta en planeta, enfrentando pruebas musicales para recolectar la leche galáctica. ¿Podrás convertirte en el rey de la pista para recolectar toda la leche del universo y restaurar el equilibrio lácteo intergaláctico?

**Estilo/género:**  Juego de ritmo

**Logotipo** :

![portada](https://github.com/user-attachments/assets/59a9fd3c-6b5b-4d5b-9516-28730db076f3)


**Resolución:** 800x600px 

**Probado en:**   Google Chrome

**Tamaño proyecto:** 1,5GB 

**Licencia** Este proyecto tiene una Licencia CC Reconocimiento Compartir igual (CC BY-SA)

**Fecha** : 27/05/2025

**Medios** :

- Github: Possum.Mind



# 2. Memoria del proyecto 

### 2.1 Storyboard: 
Teaser-

![teaser](https://github.com/user-attachments/assets/4811b724-0d28-40f1-8917-959f1e958c14)

Gameplay-

![gameplay](https://github.com/user-attachments/assets/ebce0c44-dfef-4e7e-8525-0a2b3b320f78)

A medida que vas avanzando en la canción van apareciendo las vacas que vas ordeñando.




### 2.2. Esquema de navegación 


![esquema de navegación](https://github.com/user-attachments/assets/e0fd5723-6a86-45f1-a7f5-b745f99acb3b)




# 3. Metodología

Metodología de desarrollo de productos multimedia basado en una metodología de UX (User Experience)



### Etapa 1: Ideación de proyecto

El año pasado participé con mi hermano en la Game Jam que se realizó en la facultad de informática, la temática fue "Espacio exterior", recientemente en aquella época vi una serie llamada "Carol and Tuesday" donde salía una canción que me gustaba mucho, "Milky Way", surgió la idea de crear un juego de ordeñar vacas galacticas asustando las vacas con el cursor para llevarlas a las maquinas de ordeñar y conseguir leche mientras tenias que matar a los aliens haciendo click para que no robaran las vacas, sin embargo el juego nunca salió, el código se rompió y la idea era muy ambiciosa para realizarla en dos días.
Decidí retomar el concepto espacial de vacas galácticas, desde hace un año mi habilidad en el dibujo digital ha cambiado y por ello decidí volver a dibujarlas y darle una vuelta distinta al gameplay partiendo de algo más sencillo dentro de mis gustos personales.

![image](https://github.com/user-attachments/assets/a605ab42-2137-44ea-b515-c0e7cb188688)

![image](https://github.com/user-attachments/assets/b81dffa4-f4f1-4103-8f29-fbde48a5f5ab)



**Motivación de la propuesta** 

Esta idea me motivó por un lado, porque podía llevar a cabo aquel primer proyecto que nunca llegó a ver la luz, y por el otro lado, me gusta mucho escuchar música pero soy muy mala en la música, a penas tengo conocimientos al respecto, los juegos de ritmo me hacen sentir que me ayudan un poquito a entender la música y por ello la decisión de crear este proyecto.
Al principio me propuse aprender lo básico para crear al menos una canción, estilo lofi, para añadir en los niveles del juego, iba a utilizar reaper y me descargué varios plugins gratuitos pensados para ello como el Love-Fi 4 o efectos de batería de Labs, empecé a crear la canción pero por falta de tiempo opté por abandonar la idea.



**Publico / audiencia**

- Orientado a jóvenes de a partir de 9 años y adultos.





### Etapa 2: Desarrollo / actividades realizadas

- Juego: surgieron tres problemas mientras realizaba el gameplay:
  Empecé programando el movimiento de caída de las flechas y como se regeneraban, pero no aparecía ninguna flecha, para ello cambié la velocidad con la que caían, iban demasido despacio y por ello no llegaban a    aparecer en pantalla.
  Una vez que tenía todo listo, cuando se te escaba una flecha que no llegabas a pulsar mientras jugabas, esa flecha no se borraba del juego provocando grandes errores, revisando el código resultó que varios 
  timers que usé al principio para ayudarme a crear un patrón de juego aleatorio antes de definir la posición de las flechas eran los acusantes del problema y simplemente los borré.
- Animaciones: Fue compliccado crear al principio el teaser con la abimación del cohete y una vez que lo hice no pasaba de escena una vez que terminaba la animación, tenía un timer donde se suponiía que al       
  terminar el tiempo que duraba la animación cambiaba a la siguiente escena, el fallo estaba en que no escribí bien la ubicación de la siguiente escena.
  Durante el gamplay tuve dificultades con las vacas, creé una especie de galería animada, lo misque que la galería normal del juego pero usando un AnimatedSprite2D que a parte tenía un AnimationPlayer con un 
  movimiento que hacían todas las vacas y un Timer que era el encargadoo de cambiar de vaca cada 70 segundos, es un poco más complejo que la galería normal pero no tanto. Si hubiera tenido más tiempo me habría 
  gustado o colocar esta galería de vacas pero que cambiaran entre ellas de manera aleatoria y a ser posible en punción de la puntuación, o asignar una canción corta de entre 30 y 70 segundos a cada vaca y que 
  cada vez que cambiase de vaca, sonase la melodía que cada una tiene asignada.
- Video: No llegué a tener problemas. 
- Audio: Al principio no sabía como colocar una música que sonara entre escenas, descubrí las escenas globales y con ello fue bastante fácil.
- Menús y elementos de navegación (botones): No sabía como hacer para que al pulsar el botón sonara el sonido, conseguía hacer que sonase al pasar el cursor por encima pero poco más, luego me di cuenta que no sonaba porque no le daba tiempo a sonar entre una escena y otra, solo había que poner un Timer que contara unos 0.5 segundos antes de cambiar de escena para dar tiempo al sonido.




### Etapa 3: Problemas identificados

En la animación del menú, cuando se reinicia hace movimientos raros, dura a penas poco menos de un segundo y no afecta a la jugabilidad ni a las funciones de naada pero visualmente en caso de llegar a verlo se ve raro.
Como he comentado antes, me habría gustado hacer que las vacas participaran más añadiendo melodias, me habría gustado que fueran coleccionables también, de ir desbloqueandolas, pero de momento no he tenido tiempo para idear todo esto.ç
Por lo general he llegado a resolver los fallos más grandes, es verdad que podría limpiar un poco más el código, en algunas partes se queda muerto y no hace nada, algunos botones no llegan a cumplir con ese requisito de hacer un sonido al pulsar... detalles menores que podrían mejorar pero que no afectan al juego en si.



# 4. Conclusiones 

Pienso que es obvio que el juego se encuentra incompleto, me gustaría llegar a terminarlo implementando todo aquello que he ido comentado anteriormente, el sistema de coleccionar vacas y que estas tengas sus propias canciones que van surgiendo a lo largo de la partida, unas serían más difíciles (las flechas bajarían más rápido) y otras más faciles (las flechas bajarían despacio) y llegar a crear yo misma las melodías .
También, en parte, me siento satisfecha, estéticamente el juego tiene una apariencia muy marcada y característica que incluso podría decir que "se ve bonito", he consiguido realizar aquella idea de la Game Jam que en su momento me entristeció bastante y teniendo en cuenta que la última vez no llegó a salir nada del juego y que en esta ocasión se puede jugar aunque sea un solo nivel ya es un gran paso para futuros proyectos.







# 5 Referencias 

Como inspiración me basé en dos juegos:
En el minijuego de baile que aparecía en Clup Penguin
![image](https://github.com/user-attachments/assets/5001f983-cedb-4fe3-bfc3-4b768bb2e383)

Y en el juego de Friday Night Funkin
![image](https://github.com/user-attachments/assets/6f638d7a-4998-49be-b946-d76a39b670dd)





**Recursos y materiales audiovisuales:**

* Musica:
  "Milky Way" del anime "Carol and Tuesday" (2017), cantado por Madison McFerrin
  Efectos de sonido de pixabay (https://pixabay.com/es/)
* Vídeo: vacasbailando con música del Pou (https://www.tiktok.com/@_milanesa_de_locro_/video/6979059074201619717)
* Tipografía:
  Sacadas de DaFont (https://www.dafont.com/es/)
  Galctic-Bold
  Ginger Galaxy
  Fiexus

**Herramientas utilizadas**

- Godot 4.4
- Procreate (assets)



(imagen de la licencia, copiar y pegar aquí la correcta)

https://creativecommons.org/licenses/?lang=es

Mayo 2025
