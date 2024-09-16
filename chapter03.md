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

# Capítulo III: Requirements Specification
## 3.1. To-Be Scenario Mapping
## 3.2. User Stories
Este documento presenta un conjunto de **User Stories** y **Epics** para la plataforma de videojuegos orientada tanto a **Gamers** como a **Desarrolladores de Videojuegos**. Se incluye el formato de historias de usuario, donde cada una tiene criterios de aceptación en el formato Gherkin, y se presentan tanto las historias para la interfaz del usuario final como las **Technical Stories** para el RESTful API.

<!-- EPIC 1 -->
<table>
  <tr>
    <th>EPIC ID</th>
    <th>01</th>
    <th>TITLE: Recomendaciones Personalizadas</th>
  </tr>
  <tr>
    <td colspan="3">
      <strong>Cómo</strong> gamer entusiasta,
      <strong>quiero</strong> recibir recomendaciones personalizadas de juegos basadas en mi historial de juegos y mis preferencias
      <strong>para</strong> descubrir juegos que puedan interesarme.
    </td>
  </tr>
</table>

<!-- USER STORY 1 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US01</th>
    <th>EPIC ID</th>
    <th>EPIC01</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Filtrado de Juegos por Género</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> poder filtrar juegos por género <strong>para</strong> encontrar rápidamente aquellos que me interesan.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Filtrado de juegos por género<br>
      <strong>Given</strong> que estoy en la sección de búsqueda,<br>
      <strong>When</strong> selecciono un género,<br>
      <strong>Then</strong> solo se muestran los juegos del género seleccionado.
    </td>
  </tr>
</table>

<!-- USER STORY 2 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US02</th>
    <th>EPIC ID</th>
    <th>EPIC01</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Recomendaciones Basadas en Género Favorito</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> recibir recomendaciones de juegos en mi género favorito <strong>para</strong> descubrir más juegos similares.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Recomendaciones basadas en género favorito<br>
      <strong>Given</strong> que he marcado un género como favorito,<br>
      <strong>When</strong> accedo a mi perfil,<br>
      <strong>Then</strong> veo una lista de juegos recomendados del mismo género.
    </td>
  </tr>
</table>

<!-- USER STORY 3 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US03</th>
    <th>EPIC ID</th>
    <th>EPIC01</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Recomendaciones Basadas en Popularidad entre Amigos</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> ver los juegos más populares entre mis amigos <strong>para</strong> descubrir qué están jugando.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Recomendaciones basadas en popularidad entre amigos<br>
      <strong>Given</strong> que tengo amigos en la plataforma,<br>
      <strong>When</strong> accedo a la sección de recomendaciones,<br>
      <strong>Then</strong> veo una lista de juegos populares entre mis amigos.
    </td>
  </tr>
</table>

<!-- USER STORY 4 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US04</th>
    <th>EPIC ID</th>
    <th>EPIC01</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Recomendaciones Basadas en Tiempo Jugado</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> que me recomienden juegos similares a aquellos en los que he invertido más tiempo <strong>para</strong> seguir disfrutando de ese tipo de juegos.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Recomendaciones basadas en tiempo jugado<br>
      <strong>Given</strong> que he jugado un juego por más de 10 horas,<br>
      <strong>When</strong> accedo a la sección de recomendaciones,<br>
      <strong>Then</strong> veo juegos similares en términos de género y mecánicas.
    </td>
  </tr>
</table>

<!-- USER STORY 5 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US05</th>
    <th>EPIC ID</th>
    <th>EPIC01</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Sistema de Revisión de Juegos</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> ver reseñas de otros jugadores antes de comprar un juego <strong>para</strong> tomar una mejor decisión de compra.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Ver reseñas de otros jugadores<br>
      <strong>Given</strong> que estoy viendo un juego en la tienda,<br>
      <strong>When</strong> accedo a la sección de reseñas,<br>
      <strong>Then</strong> puedo leer opiniones y valoraciones de otros jugadores.
    </td>
  </tr>
</table>

<!-- USER STORY 6 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US06</th>
    <th>EPIC ID</th>
    <th>EPIC01</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Búsqueda de Juegos por Palabra Clave</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> buscar juegos usando palabras clave <strong>para</strong> encontrar juegos específicos rápidamente.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Búsqueda por palabra clave<br>
      <strong>Given</strong> que estoy en la página de búsqueda,<br>
      <strong>When</strong> ingreso una palabra clave,<br>
      <strong>Then</strong> se muestran los juegos relacionados con esa búsqueda.
    </td>
  </tr>
</table>

<!-- USER STORY 7 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US07</th>
    <th>EPIC ID</th>
    <th>EPIC01</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Acceso a Demos de Juegos</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> poder acceder a demos de juegos antes de comprarlos <strong>para</strong> probar si me gustan antes de hacer una compra.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Acceso a demos de juegos<br>
      <strong>Given</strong> que estoy en la página de un juego,<br>
      <strong>When</strong> hay una demo disponible,<br>
      <strong>Then</strong> puedo descargarla y jugarla.
    </td>
  </tr>
</table>

<!-- USER STORY 8 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US08</th>
    <th>EPIC ID</th>
    <th>EPIC01</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Modo Offline para Juegos Indie</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> que algunos juegos indie sean jugables en modo offline <strong>para</strong> poder jugar incluso sin conexión a internet.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Jugar en modo offline<br>
      <strong>Given</strong> que estoy jugando un juego indie compatible,<br>
      <strong>When</strong> pierdo la conexión a internet,<br>
      <strong>Then</strong> puedo continuar jugando en modo offline.
    </td>
  </tr>
</table>

<!-- USER STORY 9 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US09</th>
    <th>EPIC ID</th>
    <th>EPIC01</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Recomendaciones Basadas en Juegos Anteriores</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer entusiasta, <strong>quiero</strong> recibir recomendaciones de juegos basadas en los juegos que he jugado anteriormente <strong>para</strong> descubrir nuevos juegos que se ajusten a mis gustos.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Recomendaciones basadas en historial de juegos<br>
      <strong>Given</strong> que he jugado varios juegos,<br>
      <strong>When</strong> accedo a la sección de recomendaciones,<br>
      <strong>Then</strong> veo una lista de juegos recomendados que se basan en mi historial de juegos previos.
    </td>
  </tr>
</table>

<!-- USER STORY 10 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US24</th>
    <th>EPIC ID</th>
    <th>EPIC01</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Recomendaciones Basadas en Preferencias de Género</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer entusiasta, <strong>quiero</strong> recibir recomendaciones de juegos basadas en mis preferencias de género <strong>para</strong> encontrar juegos que coincidan con mis intereses.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Recomendaciones basadas en preferencias de género<br>
      <strong>Given</strong> que he definido mis géneros de juegos preferidos,<br>
      <strong>When</strong> accedo a la sección de recomendaciones,<br>
      <strong>Then</strong> veo una lista de juegos recomendados que pertenecen a mis géneros preferidos.
    </td>
  </tr>
</table>
<br>

---

<!-- EPIC 2 -->
<table>
  <tr>
    <th>EPIC ID</th>
    <th>02</th>
    <th>TITLE: Experiencia Social en la Plataforma</th>
  </tr>
  <tr>
    <td colspan="3">
      <strong>Cómo</strong> gamer,
      <strong>quiero</strong> poder conectarme con amigos y ver qué juegos están jugando
      <strong>para</strong> compartir mis experiencias y descubrir nuevos juegos a través de mi red social.
    </td>
  </tr>
</table>

<!-- USER STORY 11 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US11</th>
    <th>EPIC ID</th>
    <th>EPIC02</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Invitación a Amigos para Jugar</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> invitar a mis amigos a jugar un juego conmigo <strong>para</strong> compartir experiencias de juego.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Invitar amigos a un juego<br>
      <strong>Given</strong> que estoy en la página de un juego,<br>
      <strong>When</strong> selecciono "Invitar a un amigo",<br>
      <strong>Then</strong> mis amigos reciben una notificación de invitación para unirse.
    </td>
  </tr>
</table>

<!-- USER STORY 12 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US12</th>
    <th>EPIC ID</th>
    <th>EPIC02</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Chat en Tiempo Real</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> un sistema de chat en tiempo real <strong>para</strong> comunicarme con mis amigos mientras jugamos juntos.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Sistema de chat en tiempo real<br>
      <strong>Given</strong> que estoy en una partida con amigos,<br>
      <strong>When</strong> accedo al chat,<br>
      <strong>Then</strong> puedo comunicarme con ellos en tiempo real.
    </td>
  </tr>
</table>

<!-- USER STORY 13 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US13</th>
    <th>EPIC ID</th>
    <th>EPIC02</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Compartir Reseñas de Juegos</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> compartir reseñas de los juegos que he jugado <strong>para</strong> ayudar a otros jugadores a decidir si quieren probarlos.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Compartir reseñas de juegos<br>
      <strong>Given</strong> que he jugado un juego,<br>
      <strong>When</strong> accedo a la sección de reseñas,<br>
      <strong>Then</strong> puedo escribir y publicar mi opinión sobre el juego.
    </td>
  </tr>
</table>

<!-- USER STORY 14 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US14</th>
    <th>EPIC ID</th>
    <th>EPIC02</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Creación de Comunidades de Juego</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> unirme a comunidades de jugadores de un mismo juego <strong>para</strong> compartir estrategias y experiencias.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Unirse a comunidades de jugadores<br>
      <strong>Given</strong> que accedo a la página de un juego,<br>
      <strong>When</strong> selecciono la opción de "Unirme a la comunidad",<br>
      <strong>Then</strong> puedo interactuar con otros jugadores en foros dedicados.
    </td>
  </tr>
</table>

<!-- USER STORY 15 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US15</th>
    <th>EPIC ID</th>
    <th>EPIC02</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Personalización de Perfil de Jugador</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> personalizar mi perfil en la plataforma <strong>para</strong> reflejar mis gustos y mostrar mi progreso en los juegos.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Personalización del perfil<br>
      <strong>Given</strong> que estoy en mi perfil,<br>
      <strong>When</strong> selecciono la opción de personalización,<br>
      <strong>Then</strong> puedo cambiar mi avatar, descripción y mostrar mis logros en los juegos.
    </td>
  </tr>
</table>

<!-- USER STORY 16 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US16</th>
    <th>EPIC ID</th>
    <th>EPIC02</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Visualización de Rankings de Jugadores</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> ver mi posición en el ranking de jugadores de un juego <strong>para</strong> comparar mi progreso con el de otros jugadores.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Ver posición en el ranking<br>
      <strong>Given</strong> que estoy jugando un juego,<br>
      <strong>When</strong> accedo a la sección de rankings,<br>
      <strong>Then</strong> puedo ver mi posición en relación con otros jugadores.
    </td>
  </tr>
</table>

<!-- USER STORY 17 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US17</th>
    <th>EPIC ID</th>
    <th>EPIC02</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Sistema de Logros</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> desbloquear logros en los juegos que juego <strong>para</strong> mejorar mi experiencia y ganar recompensas.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Desbloquear logros<br>
      <strong>Given</strong> que estoy jugando un juego,<br>
      <strong>When</strong> alcanzo ciertos hitos,<br>
      <strong>Then</strong> se desbloquean logros que se reflejan en mi perfil.
    </td>
  </tr>
</table>

<!-- USER STORY 18 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US18</th>
    <th>EPIC ID</th>
    <th>EPIC02</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Notificaciones en Tiempo Real</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> recibir notificaciones en tiempo real cuando mis amigos comiencen a jugar un nuevo juego <strong>para</strong> unirme a ellos de inmediato.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Recibir notificaciones de amigos<br>
      <strong>Given</strong> que estoy conectado a la plataforma,<br>
      <strong>When</strong> un amigo comienza un juego,<br>
      <strong>Then</strong> recibo una notificación con la opción de unirme.
    </td>
  </tr>
</table>

<!-- USER STORY 19 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US24</th>
    <th>EPIC ID</th>
    <th>EPIC01</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Recomendaciones Basadas en Preferencias de Género</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer entusiasta, <strong>quiero</strong> recibir recomendaciones de juegos basadas en mis preferencias de género <strong>para</strong> encontrar juegos que coincidan con mis intereses.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Recomendaciones basadas en preferencias de género<br>
      <strong>Given</strong> que he definido mis géneros de juegos preferidos,<br>
      <strong>When</strong> accedo a la sección de recomendaciones,<br>
      <strong>Then</strong> veo una lista de juegos recomendados que pertenecen a mis géneros preferidos.
    </td>
  </tr>
</table>

<!-- USER STORY 20 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US25</th>
    <th>EPIC ID</th>
    <th>EPIC02</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Seguimiento de Actividad de Amigos</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> seguir la actividad de mis amigos en la plataforma <strong>para</strong> ver qué juegos están jugando y compartir nuestras experiencias.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Ver actividad de amigos<br>
      <strong>Given</strong> que estoy en mi perfil de usuario,<br>
      <strong>When</strong> accedo a la sección de amigos,<br>
      <strong>Then</strong> puedo ver qué juegos están jugando mis amigos y cuándo se conectaron por última vez.
    </td>
  </tr>
</table>
<br>

---

<!-- EPIC 3 -->
<table>
  <tr>
    <th>EPIC ID</th>
    <th>03</th>
    <th>TITLE: Publicación y Gestión de Juegos</th>
  </tr>
  <tr>
    <td colspan="3">
      <strong>Cómo</strong> desarrollador,
      <strong>quiero</strong> publicar y gestionar mis juegos en la plataforma
      <strong>para</strong> que lleguen a una audiencia más amplia de gamers interesados en juegos independientes.
    </td>
  </tr>
</table>

<!-- USER STORY 21 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US21</th>
    <th>EPIC ID</th>
    <th>EPIC03</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Publicar Juego Indie</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como desarrollador, <strong>quiero</strong> poder publicar mi juego indie en la plataforma <strong>para</strong> llegar a una audiencia más amplia.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Publicar un juego indie<br>
      <strong>Given</strong> que he desarrollado un juego indie,<br>
      <strong>When</strong> subo los archivos del juego y los detalles de la descripción,<br>
      <strong>Then</strong> el juego se publica en la sección de juegos indie.
    </td>
  </tr>
</table>

<!-- USER STORY 22 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US22</th>
    <th>EPIC ID</th>
    <th>EPIC03</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Actualización de Juegos Indie</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como desarrollador, <strong>quiero</strong> poder actualizar la información de mi juego indie <strong>para</strong> corregir errores o agregar nuevas características.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Actualizar un juego indie<br>
      <strong>Given</strong> que he publicado un juego,<br>
      <strong>When</strong> hago cambios en la descripción o archivos del juego,<br>
      <strong>Then</strong> la información se actualiza en tiempo real en la plataforma.
    </td>
  </tr>
</table>

<!-- USER STORY 23 -->
<!-- USER STORY 24 -->
<!-- USER STORY 25 -->
<!-- USER STORY 26 -->
<!-- USER STORY 27 -->
<!-- USER STORY 28 -->
<!-- USER STORY 29 -->
<!-- USER STORY 30 -->

<br>

---

<!-- EPIC 4 -->

<table>
  <tr>
    <th>EPIC ID</th>
    <th>04</th>
    <th>TITLE: Análisis de Métricas de Juego</th>
  </tr>
  <tr>
    <td colspan="3">
      <strong>Cómo</strong> desarrollador,
      <strong>quiero</strong> tener acceso a métricas detalladas sobre el comportamiento de los jugadores en mis juegos
      <strong>para</strong> poder ajustar y mejorar la experiencia de usuario.
    </td>
  </tr>
</table>

<!-- USER STORY 31 -->
<!-- USER STORY 32 -->
<!-- USER STORY 33 -->
<!-- USER STORY 34 -->
<!-- USER STORY 35 -->
<!-- USER STORY 36 -->
<!-- USER STORY 37 -->
<!-- USER STORY 38 -->
<!-- USER STORY 39 -->
<!-- USER STORY 40 -->

<br>

---

<!-- EPIC 5 -->
<table>
  <tr>
    <th>EPIC ID</th>
    <th>05</th>
    <th>TITLE: Comunidad para Compartir Logros</th>
  </tr>
  <tr>
    <td colspan="3">
      <strong>Cómo</strong> gamer,
      <strong>quiero</strong> contar con una comunidad donde pueda compartir mis logros y éxitos en los juegos
      <strong>para</strong> celebrar mis avances, recibir reconocimiento y conectarme con otros jugadores que comparten mis intereses.
    </td>
  </tr>
</table>

<!-- USER STORY 40 -->
<!-- USER STORY 41 -->
<!-- USER STORY 42 -->
<!-- USER STORY 43 -->
<!-- USER STORY 44 -->
<!-- USER STORY 45 -->
<!-- USER STORY 46 -->
<!-- USER STORY 47 -->
<!-- USER STORY 48 -->
<!-- USER STORY 49 -->
<!-- USER STORY 50 -->

## 3.3. Impact Mapping
## 3.4. Product Backlog