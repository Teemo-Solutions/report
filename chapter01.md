<style>
  body {
    font-family: 'Times New Roman', sans-serif;
    text-align: justify;
    font-size: 12px;
    margin-left: 2em;
    margin-right: 2em;
    line-height: 2;
  }
  
  p {
    text-indent: 2em; /* Sangría en el primer renglón de cada párrafo */
  }

  h1 {
    margin-left: 0; /* No aplica sangría para el título principal */
  }

  h2 {
    margin-left: 0; /* No aplica sangría para subtítulos de nivel 2 */
  }

  h3 {
    margin-left: 2em; /* Aplica una sangría de 2em para subtítulos de nivel 3 */
  }

  h4 {
    margin-left: 4em; /* Aplica una sangría de 4em para subtítulos de nivel 4 */
  }
</style>

# **CAPÍTULO I: INTRODUCCIÓN**
## 1.1. Startup Profile
### 1.1.1. Description de la Startup
**Teemo Solutions** es una startup que conecta a los gamers con los videojuegos que realmente les interesan. Con nuestro producto principal, **Vortex**, hemos creado una plataforma web donde los jugadores pueden descubrir nuevos títulos basados en sus gustos, conectar con amigos y recibir recomendaciones personalizadas.

<p align="center">
  <img src="assets/logos/teemo_solutions_icon.jpg"  style="width:150px; height:auto;" alt="">
  <img src="assets/logos/vortex_icon.svg"  style="width:150px; height:auto;" alt="">
</p>

Además, las empresas desarrolladoras pueden promocionar sus juegos directamente a una audiencia apasionada. Vortex también ofrece una opción de suscripción para acceder a características avanzadas que mejoran la experiencia de los usuarios. En Teemo Solutions, nos apasionan los videojuegos y queremos ayudar a los gamers a encontrar su próximo juego favorito.

### 1.1.2. Perfiles de integrantes del equipo
<table>
  <tr>
    <th colspan="2">Quijandria Aranedal, Vicente </th>
  </tr>
  <tr>
    <td><img src="assets/chapter01/team/vicente-photo.png" style="width:500px; height:auto;" alt=""></td>
    <td>descripción</td>
  </tr>
  <tr>
    <th colspan="2">Lizano Coll Cardenas, Fernando Jesus</th>
  </tr>
  <tr>
    <td><img src="assets/chapter01/team/fernando-photo.png" style="width:500px; height:auto;" alt=""></td>
    <td>Me llamo Fernando Jesus Lizano Coll Cardenas. A mis 19 años me considero un apasionado por el mundo de la programación y aprendizaje constante. Actualmente tengo conocimientos en el lenguaje de C++, HTML, CSS, JavaScript y Python. Aunque mis conocimientos son todavía básicos. Me identifico como alguien de pensamiento de superación. Busco crecer en cada aspecto de mi vida y enfrentar desafíos con una actitud positiva y resoluta. Espero poder aportar y motivar a mis compañeros durante la elaboración de este proyecto.</td>
  </tr>
  <tr>
    <th colspan="2">Renteria Palacios, Yasser</th>
  </tr>
  <td><img src="assets/chapter01/team/yasser-photo.png" style="width:500px; height:auto;" alt=""></td>
    <td>Soy estudiante de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas (UPC), apasionado por la programación y el aprendizaje continuo de nuevos lenguajes de programación. Mi mayor anhelo es desarrollar un videojuego, combinando mi amor por la tecnología y la creatividad. En mi tiempo libre, disfruto de jugar videojuegos, viajar y sumergirme en nuevas culturas, buscando siempre experiencias que enriquezcan tanto mi vida personal como profesional.</td>
  <tr>
    <th colspan="2">Riega Salas, Jose Miguel</th>
  </tr>
  <tr>
    <td><img src="assets/chapter01/team/jose-photo.png" style="width:500px; height:auto;" alt=""></td>
    <td>descripción</td>
  <tr>
    <th colspan="2">Torres García, Andrés Alberto
  </th>
  </tr>
  <tr>
    <td><img src="assets/chapter01/team/andres-photo.png" style="width:500px; height:auto;" alt=""></td>
    <td>Hola, soy Andrés Alberto Torres García, estudiante de 19 años en el quinto ciclo de Ingeniería de Software. Siempre me ha interesado tecnología, siempre me he preguntado cómo funcionan las cosas, lo que me motiva a ir más allá de lo que se me enseña en clase. Esta curiosidad me impulsa a explorar cada detalle, ayundome ampliar mis conocimiento y definir mejor mi enfoque profesional.Además de la tecnología, el fútbol es otra de mis grandes pasiones, lo he practicado durante prácticamente toda mi vida. La dedicación al deporte me ha enseñado el valor del trabajo en equipo, la disciplina y la perseverancia, cualidades que aplico también en mi vida académica y profesional.
  </td>
</table>

## 1.2. Solution Profile
### 1.2.1. Antecedentes y problemática

Para analizar los antecedentes y problemáticas del desarrollo nuestro proyecto, estaremos utilizando la técnica de las 5W y 2H (Who, What, When, Where, Why, How, How much). La cual ha sido estructurada de la siguiente manera:

1. **Who (Quién)**
   * **Gamers:** Jugadores que buscan descubrir nuevos títulos basados en sus preferencias y conexiones sociales.
   * **Empresar Desarrolladoras:** Equipos de desarrollo de videojuegos que buscan nuevas formas de promocionar sus juegos a audiencias específicas. 
<br><br>
2. **What (Qué)**
   * **Aplicación web open source:** Una plataforma que sirve como un sistema de recomendación de videojuegos. Incluye funcionalidades para la creación de perfiles, recomendaciones personalizadas, conexión con amigos y promoción de juegos por parte de empresas.
   * **Problemas actuales:** Los gamers enfrentan dificultades para descubrir nuevos juegos que se alineen con sus gustos, mientras que las empresas buscan maneras más efectivas de promocionar sus títulos en el mercado.
<br><br>
3. **When (Cuándo)**
    * **Contexto actual:** En un mercado de videojuegos que está en constante crecimiento, con un flujo continuo de nuevos títulos, surge la necesidad de herramientas que faciliten el descubrimiento y promoción de juegos. La demanda de personalización y conectividad en las plataformas de entretenimiento es más fuerte que nunca.
<br><br>
4. **Where (Dónde)**
   * **Plataforma digital:** La aplicación estará disponible online, accesible desde cualquier lugar con conexión a internet. Dirigida a usuarios de habla hispana, con la posibilidad de expansión a otros idiomas.
<br><br>
5. **Why (Por qué)**
   * **Necesidad del mercado:** La industria de los videojuegos está cada vez más saturada, lo que dificulta que tanto jugadores como desarrolladores se destaquen. Los gamers buscan recomendaciones personalizadas y confiables, mientras que las empresas necesitan una plataforma efectiva para llegar a sus audiencias.
   * **Beneficio:** Facilitar el descubrimiento de nuevos juegos y mejorar la visibilidad de los títulos de las empresas, fomentando una comunidad más conectada y personalizada.
<br><br>
6. **How (Cómo)**
   * **Desarrollo de la aplicación:** La aplicación será desarrollada como un proyecto open source, permitiendo la colaboración de la comunidad. Incluirá funcionalidades para la creación de perfiles, sistemas de recomendación basados en algoritmos y redes sociales, y herramientas para que las empresas publiquen y promocionen sus juegos.
   * **Promoción:** Se utilizarán estrategias de marketing digital para atraer tanto a gamers como a empresas desarrolladoras. Se promoverá la plataforma como una solución innovadora para los problemas de descubrimiento y promoción en la industria del gaming.
<br><br>
7. **How much (Cuánto)**
   * **Costos de desarrollo:** Aunque el proyecto será open source, habrá costos asociados a la infraestructura, mantenimiento, y posibles actualizaciones.
   * **Modelos de ingresos:** A través de suscripciones premium que ofrecen funcionalidades avanzadas y posiblemente publicidad pagada para las empresas desarrolladoras.

Esta estructura nos permite una comprensión clara y detallada de los antecedentes y problemáticas relacionadas con el desarrollo de la aplicación web para recomendaciones de videojuegos.

### 1.2.2 Lean UX Process
#### 1.2.2.1. Lean UX Problem Statements

En la actual era digital, los videojuegos se han convertido en una de las principales formas de entretenimiento, con una enorme diversidad de títulos y plataformas disponibles. Sin embargo, muchos jugadores enfrentan la dificultad de descubrir nuevos juegos que realmente se alineen con sus preferencias y estilo de juego. Además, la experiencia social de compartir estos intereses con amigos está fragmentada entre múltiples plataformas, lo que dificulta la interacción fluida entre jugadores. Por otro lado, los desarrolladores de juegos independientes enfrentan barreras para dar a conocer sus creaciones en un mercado saturado.
<br>
Vortex busca resolver estos problemas proporcionando una plataforma unificada donde los usuarios pueden recibir recomendaciones personalizadas de videojuegos basadas en sus preferencias y listas de favoritos. La plataforma también permite la interacción social, permitiendo agregar amigos y compartir intereses en juegos. Para los desarrolladores, Vortex ofrece la oportunidad de subir y promocionar sus videojuegos directamente a una audiencia segmentada, aumentando la visibilidad y el alcance de sus proyectos. De este modo, Vortex se posiciona como una solución integral tanto para jugadores en busca de su próximo juego favorito, como para desarrolladores que buscan dar a conocer sus innovaciones.

#### 1.2.2.2. Lean UX Assumptions

**Bussiness Assumptions**

1. **Creemos que nuestros clientes tienen la necesidad de:**  
   Encontrar recomendaciones de juegos que realmente se adapten a lo que el usuario deja indicios de necesitar.

2. **Estas necesidades se pueden satisfacer con:**  
   una plataforma web que personalice las recomendaciones de juegos, permita la interacción social y ofrezca sugerencias basadas en las preferencias individuales de los gamers.

3. **Nuestros clientes iniciales son (o serán):**  
   gamers apasionados que buscan recomendaciones personalizadas y conexiones dentro de una comunidad de jugadores.

4. **El valor principal que un cliente quiere obtener de nuestro servicio es:**  
   encontrar nuevos videojuegos que coincidan con sus intereses y conectarse con otros jugadores de manera eficiente y personalizada.

5. **Los clientes también pueden obtener estos beneficios adicionales:**  
   promociones exclusivas de juegos, acceso a comunidades dedicadas y recomendaciones que optimicen su experiencia de juego.

6. **Adquiriremos a la mayoría de nuestros clientes a través de:**  
   campañas de marketing dirigidas en redes sociales, influencers del mundo gaming y colaboraciones con desarrolladores de videojuegos.   

7. **Ganaremos dinero mediante:**  
   suscripciones premium que ofrezcan características avanzadas, así como acuerdos publicitarios con desarrolladores de videojuegos que promocionen sus títulos en nuestra plataforma.  

8. **Nuestra competencia principal en el mercado será:**  
   otras plataformas de recomendaciones de videojuegos y redes sociales orientadas a gamers.

9. **Les superaremos debido a:**  
   nuestras recomendaciones personalizadas y la integración de una comunidad activa que facilita tanto la interacción social como el descubrimiento de juegos.

10. **El mayor riesgo para nuestro producto es:**  
   que los algoritmos de recomendación no ofrezcan títulos relevantes o que la experiencia social dentro de la plataforma no sea suficientemente atractiva para retener a los usuarios.


 ---

**User Assumptions**

1. **¿Quién es el usuario?**  
   Los usuarios son gamers que buscan nuevas experiencias de juego y que disfrutan de estar al día con los títulos más recientes y populares.

2. **¿Dónde encaja nuestro producto en su trabajo o vida?**  
   Nuestro producto encaja en su rutina diaria de entretenimiento, ayudándoles a descubrir nuevos juegos y conectarse con otros jugadores con intereses similares.

3. **¿Qué problemas resuelve nuestro producto?**  
   Resuelve la sobrecarga de opciones de juegos, facilitando la selección de títulos basados en gustos individuales, y ofrece una plataforma social que conecta a gamers.

4. **¿Cuándo y cómo se utiliza nuestro producto?**  
   Se utiliza cuando los gamers buscan nuevos títulos para jugar o desean interactuar con otros jugadores, ofreciendo recomendaciones personalizadas y herramientas de comunicación.

5. **¿Qué características son importantes?**  
   Recomendaciones precisas de videojuegos, integración social, capacidad de personalización de preferencias, promociones exclusivas y una experiencia de usuario fluida.

6. **¿Cómo debería verse y comportarse nuestro producto?**  
   Debe ser visualmente atractivo, con una interfaz intuitiva y características interactivas que fomenten tanto la exploración de juegos como la interacción con otros gamers.

7. **El valor principal que un usuario quiere obtener de nuestra funcionalidad es:**  
   Recomendaciones de juegos altamente personalizadas que se ajusten a sus intereses específicos.

8. **Los usuarios también pueden obtener estos beneficios adicionales:**  
   Promociones exclusivas de juegos, acceso a una comunidad activa y conexiones con otros jugadores.

9. **El mayor riesgo para el usuario es:**  
   Que las recomendaciones de juegos no sean relevantes o que la experiencia de la comunidad no les aporte valor suficiente para seguir usando la plataforma.


**User Outcomes:**

**Descubrimiento de Nuevos Juegos:**  Los usuarios desean descubrir fácilmente videojuegos que coincidan con sus preferencias personales y estilos de juego. Este outcome se centra en proporcionar una experiencia de descubrimiento intuitiva y relevante que optimice su tiempo de entretenimiento y les exponga a títulos nuevos y emocionantes.

**Conexión Social entre Gamers:** Los gamers buscan una plataforma donde puedan interactuar con otros jugadores, compartir experiencias de juego y discutir títulos en tendencia. El éxito se mide por la actividad dentro de la comunidad y la cantidad de conexiones creadas entre jugadores con intereses similares.

**Promociones Exclusivas y Personalización:**  Los usuarios valoran el acceso a promociones exclusivas y la posibilidad de personalizar su experiencia dentro de la plataforma, ajustando las recomendaciones y la interfaz según sus preferencias. El éxito se evalúa por la satisfacción del usuario y su nivel de interacción con las características avanzadas.

---

**Business Outcomes:**

**Crecimiento de la Comunidad de Gamers:** Esperamos que el 15% de los usuarios que se registren en la plataforma Vortex utilicen activamente las funciones sociales dentro del primer mes de uso. El éxito se medirá por la cantidad de interacciones dentro de la comunidad y la retención de usuarios activos.

**Incremento de Ingresos por Suscripciones:** Esperamos que al menos el 20% de los usuarios iniciales se suscriban a los servicios premium de la plataforma dentro de los primeros seis meses, obteniendo acceso a características avanzadas y promociones exclusivas. Este éxito se medirá a través de la tasa de conversión de usuarios gratuitos a suscriptores de pago.

**Impulso a la Promoción de Juegos:** Con alianzas estratégicas con desarrolladores, se espera que al menos el 30% de los títulos promocionados en la plataforma experimenten un aumento significativo en el número de jugadores interesados dentro de los primeros tres meses. Este éxito se medirá por el aumento en las ventas y descargas de juegos promovidos en la plataforma.

---
**Features Assumptions:**

**1. Recomendaciones Personalizadas:**

**- Algoritmo de Recomendación:** Implementar un sistema avanzado de recomendaciones que sugiera juegos a los usuarios en función de sus preferencias de juego, hábitos y títulos previos jugados.

**- Promociones Exclusivas:** Ofrecer promociones exclusivas de juegos que se ajusten a los gustos individuales de cada usuario, incentivando la participación y la compra de nuevos títulos.

**2. Conexión Social entre Gamers:**

**- Comunidad de Gamers:** Desarrollar una funcionalidad que permita a los usuarios conectarse con otros jugadores, unirse a grupos según sus intereses de juegos y compartir experiencias.

**- Chat en Tiempo Real:** Incorporar un sistema de chat en tiempo real para facilitar la comunicación entre jugadores durante la recomendación de juegos y las interacciones dentro de la comunidad.

**3. Generación de Ingresos:**

**- Suscripción Premium:** Ofrecer una suscripción que brinde acceso a funciones avanzadas, como recomendaciones más personalizadas, acceso anticipado a promociones exclusivas y herramientas adicionales para gestionar sus juegos y conexiones.

**- Publicidad Personalizada para Desarrolladores:** Implementar un modelo de publicidad en la plataforma que permita a los desarrolladores promover sus juegos a audiencias segmentadas, con un enfoque en los intereses específicos de los usuarios.


#### 1.2.2.3. Lean UX Hypothesis Statements
**Creemos que** el sistema de recomendaciones personalizadas de videojuegos basado en preferencias y conexiones sociales proporcionará una experiencia más atractiva a los gamers. **Sabremos que** esto es cierto cuando el 60% de los usuarios interactúen con las recomendaciones y encuentren nuevos juegos para descargar o jugar.

**Creemos que** la posibilidad de que las empresas desarrolladoras promocionen sus títulos directamente en la plataforma proporcionará mayor visibilidad a los desarrolladores de videojuegos independientes. **Sabremos que** esto es cierto cuando las empresas vean un aumento del 25% en clics en los juegos promocionados a través de nuestra plataforma.

**Creemos que** permitir a los usuarios crear perfiles detallados y conectarse con amigos en la plataforma proporcionará una mayor interacción social a los gamers. **Sabremos que** esto es cierto cuando al menos el 40% de los usuarios interactúen regularmente con sus amigos y compartan recomendaciones de juegos.

**Creemos que** el sistema de suscripciones premium que ofrece acceso a funcionalidades avanzadas, como recomendaciones más precisas y acceso anticipado a lanzamientos de videojuegos, proporcionará un valor adicional a los gamers frecuentes. **Sabremos que** esto es cierto cuando el 20% de los usuarios opten por la suscripción premium en los primeros 6 meses.

**Creemos que** al ofrecer una estructura de ingresos donde el 90% del pago por cada videojuego va para el desarrollador y el 10% para la plataforma proporcionará un incentivo atractivo a los desarrolladores para publicar y promocionar sus juegos en nuestra plataforma. **Sabremos que** esto es cierto cuando al menos el 30% de los desarrolladores de videojuegos independientes elijan nuestra plataforma para vender sus títulos y generemos ingresos extra a partir de estas transacciones.

#### 1.2.2.4. Lean UX Canvas

<img src="/assets/chapter01/leanUX/canva.png" alt="lean UX canva" >

## 1.3. Segmentos Objetivos
En cuanto el segmento objetivo, es importante delimitar con a que sector nos vamos a dirigir, para poder ofrecer una mejor atención y cumplir con las necesidades de los usuarios, y así realizar una aplicación más funcional a lo que se está requiriendo.

Para ello, se ha definido dos segmentos objetivo: Gamers Entusiastas y Empresas Desarrolladoras de Videojuegos. A continuación, se detallan las características y descripciones de cada segmento:

<table>
  <tr>
    <th colspan="2">Gamers Entusiastas</th>
  </tr>
  <tr>
    <td><b>Segmento Objetivo / Características</b></td>
    <td><b>Descripción del segmento</b></td>
  </tr>
  <tr>
    <td><b>Geográfico</b></td>
    <td>
      <ul>
        <li><b>Ubicación principal:</b> Lima, Perú (considerando su alta densidad poblacional y acceso a internet)</li>
        <li><b>Potencial de expansión:</b> Otras ciudades importantes de Perú con una escena gamer activa (Arequipa, Trujillo, Cusco, etc.)</li>
        <li><b>Consideraciones geográficas:</b></li>
        <ul>
          <li>Acceso a internet de banda ancha</li>
          <li>Distribución de consolas y PCs para gaming</li>
          <li>Presencia de eventos y comunidades gamer locales</li>
        </ul>
      </ul>
    </td>
  </tr>
  <tr>
    <td><b>Demográfico</b></td>
    <td>
      <ul>
        <li><b>Edad:</b> 15-35 años (grupo con mayor afinidad a los videojuegos y adopción de nuevas tecnologías)</li>
        <li><b>Nivel socioeconómico:</b> Medio y medio-alto (capacidad adquisitiva para hardware, juegos y suscripciones)</li>
        <li><b>Nivel educativo:</b> Secundaria completa o superior (mayor comprensión de plataformas digitales y tendencias)</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td><b>Psicográfico</b></td>
    <td>
      <b>Estilo de vida:</b>
      <ul>
        <li><b>Apasionados por los videojuegos:</b> Dedican tiempo y recursos a esta actividad</li>
        <li><b>Conectados digitalmente:</b> Activos en redes sociales y plataformas online</li>
        <li><b>Sociales:</b> Disfrutan interactuar con otros jugadores y compartir experiencias</li>
      </ul>
      <b>Personalidad:</b>
      <ul>
        <li><b>Curiosos y abiertos a nuevas experiencias:</b> Buscan constantemente nuevos juegos y desafíos</li>
        <li><b>Competitivos:</b> Les gusta medir sus habilidades y superarse</li>
        <li><b>Valoran la calidad:</b> Prefieren juegos bien diseñados y experiencias inmersivas</li>
      </ul>
      <b>Valores y actitudes:</b>
      <ul>
        <li><b>Disposición a pagar por contenido premium:</b> Reconocen el valor de funciones exclusivas y mejoras</li>
        <li><b>Buscan comunidad:</b> Desean pertenecer a un grupo con intereses afines</li>
        <li><b>Aprecian la personalización:</b> Quieren recomendaciones y experiencias adaptadas a sus gustos</li>
      </ul>
    </td>
  </tr>
</table>

<table>
  <tr>
    <th colspan="2">Empresas Desarrolladoras de Videojuegos</th>
  </tr>
  <tr>
    <th>Segmento</th>
    <th>Descripción</th>
  </tr>
  <tr>
    <td><b>Geográfico</b></td>
    <td>
      <ul>
        <li><b>Ubicación:</b> Desarrolladoras de videojuegos de tamaño pequeño a mediano en Perú, con enfoque en Lima, y otras regiones donde la industria está creciendo.</li>
        <li><b>Expansión potencial:</b> Desarrolladoras de otras partes de Latinoamérica interesadas en el mercado peruano y en acceder a una base de usuarios activos.</li>
        <li><b>Acceso a la plataforma:</b> Necesitan un fácil acceso a la plataforma para gestionar campañas y analizar resultados en tiempo real.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td><b>Demográfico</b></td>
    <td>
      <ul>
        <li><b>Tamaño de la empresa:</b> Pequeñas y medianas empresas de desarrollo de videojuegos, que buscan formas eficientes y rentables de promocionar sus productos.</li>
        <li><b>Presupuesto:</b> Empresas con presupuestos de marketing limitados, que buscan maximizar el retorno de inversión en campañas.</li>
        <li><b>Tipo de desarrolladoras:</b> Estudios independientes o "indies", así como desarrolladoras medianas que buscan aumentar su visibilidad.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td><b>Psicográfico</b></td>
    <td>
      <b>Valores y necesidades:</b>
      <ul>
        <li><b>Innovadores:</b> Buscan nuevas y creativas maneras de alcanzar a su audiencia objetivo.</li>
        <li><b>Enfocados en el rendimiento:</b> Valoran plataformas que ofrezcan métricas claras y detalladas sobre el rendimiento de sus campañas.</li>
        <li><b>Dispuestos a experimentar:</b> Abiertos a probar nuevas herramientas y técnicas para mejorar la efectividad de sus campañas de marketing.</li>
      </ul>
      <b>Estilo de vida empresarial:</b>
      <ul>
        <li><b>Agilidad:</b> Necesitan plataformas que les permitan lanzar y ajustar campañas rápidamente.</li>
        <li><b>Comunicación directa:</b> Prefieren plataformas que faciliten la interacción directa con sus audiencias.</li>
        <li><b>Colaboración:</b> Dispuestos a colaborar con plataformas que ofrezcan un valor añadido, como análisis de datos o soporte en la gestión de campañas.</li>
      </ul>
    </td>
  </tr>
</table>
