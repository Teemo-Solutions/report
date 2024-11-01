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

### Gamers

<img src="/assets/chapter03/to-be-scenario-image/to-be-scenario-gamers.png" alt="to-be-scenario-gamers" />

### Desarrolladoras

<img src="/assets/chapter03/to-be-scenario-image/to-be-scenario-desarrolladoras.png" alt=""/>

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
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US23</th>
    <th>EPIC ID</th>
    <th>EPIC03</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Subir Actualizaciones de Juegos</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como desarrollador, <strong>quiero</strong> subir actualizaciones para mi juego publicado <strong>para</strong> corregir errores y mejorar la experiencia del usuario.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Subir una actualización para un juego<br>
      <strong>Given</strong> que el desarrollador ha publicado un juego,<br>
      <strong>When</strong> sube un parche o actualización,<br>
      <strong>Then</strong> el juego se actualiza para todos los usuarios.
    </td>
  </tr>
</table>
<!-- USER STORY 24 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US24</th>
    <th>EPIC ID</th>
    <th>EPIC03</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Creación de Torneos</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como desarrollador, <strong>quiero</strong> crear torneos para mi juego <strong>para</strong> fomentar la competencia entre los jugadores.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Crear torneos para un juego<br>
      <strong>Given</strong> que el desarrollador ha publicado un juego,<br>
      <strong>When</strong> crea un torneo en la plataforma,<br>
      <strong>Then</strong> los jugadores pueden unirse y competir por premios.
    </td>
  </tr>
</table>
<!-- USER STORY 25 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US25</th>
    <th>EPIC ID</th>
    <th>EPIC03</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Subir Juegos Indie a la Plataforma</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como desarrollador indie, <strong>quiero</strong> subir mis juegos a la plataforma <strong>para</strong> que puedan ser vistos y descargados por los jugadores.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Subir un juego indie<br>
      <strong>Given</strong> que tengo un juego indie terminado,<br>
      <strong>When</strong> subo los archivos y la descripción del juego,<br>
      <strong>Then</strong> el juego se publica en la plataforma para que los jugadores puedan verlo y descargarlo.
    </td>
  </tr>
</table>

<!-- USER STORY 26 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US26</th>
    <th>EPIC ID</th>
    <th>EPIC03</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Gestión de Información del Juego</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como desarrollador indie, <strong>quiero</strong> gestionar la información de mi juego <strong>para</strong> actualizar detalles, corregir errores o agregar contenido nuevo.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Actualizar información del juego<br>
      <strong>Given</strong> que mi juego está publicado,<br>
      <strong>When</strong> hago cambios en la descripción, imágenes o archivos del juego,<br>
      <strong>Then</strong> la información del juego se actualiza en la plataforma.
    </td>
  </tr>
</table>

<!-- USER STORY 27 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US27</th>
    <th>EPIC ID</th>
    <th>EPIC03</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Gestión de Precios y Ofertas</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como desarrollador indie, <strong>quiero</strong> establecer y gestionar precios y ofertas para mi juego <strong>para</strong> atraer a más jugadores y aumentar las ventas.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Gestionar precios y ofertas<br>
      <strong>Given</strong> que mi juego está publicado,<br>
      <strong>When</strong> establezco un precio o una oferta,<br>
      <strong>Then</strong> el precio y las ofertas se reflejan en la plataforma.
    </td>
  </tr>
</table>

<!-- USER STORY 28 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US28</th>
    <th>EPIC ID</th>
    <th>EPIC03</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Monitoreo de Descargas y Ventas</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como desarrollador indie, <strong>quiero</strong> monitorear las descargas y ventas de mi juego <strong>para</strong> analizar su desempeño en la plataforma.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Monitorear descargas y ventas<br>
      <strong>Given</strong> que mi juego está publicado,<br>
      <strong>When</strong> accedo a la sección de estadísticas,<br>
      <strong>Then</strong> puedo ver el número de descargas y ventas del juego.
    </td>
  </tr>
</table>

<!-- USER STORY 29 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US29</th>
    <th>EPIC ID</th>
    <th>EPIC03</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Responder a Reseñas de Jugadores</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como desarrollador indie, <strong>quiero</strong> responder a las reseñas de jugadores <strong>para</strong> interactuar con mi audiencia y abordar sus comentarios o problemas.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Responder a reseñas<br>
      <strong>Given</strong> que hay reseñas de mi juego,<br>
      <strong>When</strong> accedo a la sección de reseñas,<br>
      <strong>Then</strong> puedo responder a las reseñas de los jugadores.
    </td>
  </tr>
</table>

<!-- USER STORY 30 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US30</th>
    <th>EPIC ID</th>
    <th>EPIC03</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Generación de Reportes de Desempeño</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como desarrollador indie, <strong>quiero</strong> generar reportes sobre el desempeño de mi juego <strong>para</strong> obtener información detallada sobre cómo está siendo recibido por los jugadores.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Generar reportes de desempeño<br>
      <strong>Given</strong> que mi juego está publicado,<br>
      <strong>When</strong> solicito un reporte de desempeño,<br>
      <strong>Then</strong> recibo un reporte con información sobre descargas, ventas y comentarios de jugadores.
    </td>
  </tr>
</table>
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
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US31</th>
    <th>EPIC ID</th>
    <th>EPIC04</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Visualización de Métricas de Jugadores</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como desarrollador, <strong>quiero</strong> ver métricas detalladas sobre cómo los jugadores interactúan con mi juego <strong>para</strong> mejorar la experiencia del usuario.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Ver métricas de jugadores<br>
      <strong>Given</strong> que he publicado un juego,<br>
      <strong>When</strong> accedo a la sección de estadísticas,<br>
      <strong>Then</strong> veo datos sobre el tiempo jugado, número de jugadores y porcentaje de finalización.
    </td>
  </tr>
</table>
<!-- USER STORY 32 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US32</th>
    <th>EPIC ID</th>
    <th>EPIC04</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Análisis de Comportamiento de Jugadores</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como desarrollador, <strong>quiero</strong> analizar el comportamiento de los jugadores <strong>para</strong> identificar puntos de fricción en mi juego.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Analizar el comportamiento de los jugadores<br>
      <strong>Given</strong> que el desarrollador accede al panel de estadísticas,<br>
      <strong>When</strong> revisa las métricas de nivel de dificultad o tasa de abandono,<br>
      <strong>Then</strong> puede identificar puntos de mejora en el diseño del juego.
    </td>
  </tr>
</table>
<!-- USER STORY 33 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US33</th>
    <th>EPIC ID</th>
    <th>EPIC04</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Visualización de Datos de Uso del Juego</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como desarrollador, <strong>quiero</strong> visualizar datos detallados sobre el uso del juego <strong>para</strong> entender mejor cómo los jugadores interactúan con mi juego.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Ver datos de uso del juego<br>
      <strong>Given</strong> que tengo acceso a las métricas de mi juego,<br>
      <strong>When</strong> accedo a la sección de datos de uso,<br>
      <strong>Then</strong> puedo ver información detallada sobre el tiempo de juego, frecuencia de uso y otras métricas.
    </td>
  </tr>
</table>

<!-- USER STORY 34 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US34</th>
    <th>EPIC ID</th>
    <th>EPIC04</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Análisis de Puntos de Fricción</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como desarrollador, <strong>quiero</strong> analizar los puntos de fricción en el juego <strong>para</strong> identificar y solucionar problemas que afectan la experiencia del usuario.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Analizar puntos de fricción<br>
      <strong>Given</strong> que tengo acceso a los datos de uso del juego,<br>
      <strong>When</strong> reviso los datos de nivel de dificultad y tasas de abandono,<br>
      <strong>Then</strong> puedo identificar áreas problemáticas y realizar ajustes para mejorar el juego.
    </td>
  </tr>
</table>
<!-- USER STORY 35 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US35</th>
    <th>EPIC ID</th>
    <th>EPIC04</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Seguimiento de Progreso de Jugadores</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como desarrollador, <strong>quiero</strong> hacer un seguimiento del progreso de los jugadores <strong>para</strong> comprender cómo están avanzando en el juego y ajustar la dificultad si es necesario.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Seguir el progreso de los jugadores<br>
      <strong>Given</strong> que tengo acceso a las estadísticas del juego,<br>
      <strong>When</strong> reviso el progreso de los jugadores,<br>
      <strong>Then</strong> puedo ver datos sobre el nivel alcanzado, logros obtenidos y tiempo dedicado.
    </td>
  </tr>
</table>
<!-- USER STORY 36 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US36</th>
    <th>EPIC ID</th>
    <th>EPIC04</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Análisis de Tendencias de Juego</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como desarrollador, <strong>quiero</strong> analizar las tendencias de juego <strong>para</strong> identificar qué características o niveles están siendo más populares entre los jugadores.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Analizar tendencias de juego<br>
      <strong>Given</strong> que tengo acceso a las métricas de mi juego,<br>
      <strong>When</strong> reviso las tendencias y preferencias de los jugadores,<br>
      <strong>Then</strong> puedo identificar qué características son más apreciadas y qué aspectos podrían necesitar mejoras.
    </td>
  </tr>
</table>
<!-- USER STORY 37 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US37</th>
    <th>EPIC ID</th>
    <th>EPIC04</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Comparación de Métricas entre Juegos</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como desarrollador, <strong>quiero</strong> comparar las métricas de diferentes juegos <strong>para</strong> entender qué elementos contribuyen al éxito de un juego en comparación con otros.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Comparar métricas de juegos<br>
      <strong>Given</strong> que tengo métricas de varios juegos,<br>
      <strong>When</strong> accedo a la herramienta de comparación,<br>
      <strong>Then</strong> puedo ver un análisis comparativo de datos como tiempo de juego, tasas de finalización y otros indicadores clave.
    </td>
  </tr>
</table>

<!-- USER STORY 38 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US38</th>
    <th>EPIC ID</th>
    <th>EPIC04</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Evaluación de la Retención de Jugadores</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como desarrollador, <strong>quiero</strong> evaluar la retención de jugadores <strong>para</strong> entender qué tan bien está manteniendo el interés de los jugadores en mi juego a lo largo del tiempo.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Evaluar retención de jugadores<br>
      <strong>Given</strong> que tengo acceso a las métricas de retención,<br>
      <strong>When</strong> reviso las tasas de retención en diferentes periodos,<br>
      <strong>Then</strong> puedo identificar cómo varía la retención y qué acciones podrían mejorar la permanencia de los jugadores.
    </td>
  </tr>
</table>

<!-- USER STORY 39 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US39</th>
    <th>EPIC ID</th>
    <th>EPIC04</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Reporte de Feedback de Jugadores</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como desarrollador, <strong>quiero</strong> generar reportes de feedback de jugadores <strong>para</strong> obtener una visión general de las opiniones y sugerencias de los usuarios sobre el juego.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Generar reportes de feedback<br>
      <strong>Given</strong> que los jugadores dejan comentarios y sugerencias,<br>
      <strong>When</strong> solicito un reporte de feedback,<br>
      <strong>Then</strong> recibo un informe que resume las principales opiniones y sugerencias de los jugadores.
    </td>
  </tr>
</table>

<!-- USER STORY 40 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US40</th>
    <th>EPIC ID</th>
    <th>EPIC04</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Análisis de Participación en Eventos del Juego</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como desarrollador, <strong>quiero</strong> analizar la participación en eventos dentro del juego <strong>para</strong> evaluar el impacto de estos eventos en la actividad de los jugadores y su engagement.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario:</strong> Analizar participación en eventos<br>
      <strong>Given</strong> que he organizado eventos dentro del juego,<br>
      <strong>When</strong> reviso las métricas de participación,<br>
      <strong>Then</strong> puedo ver datos sobre la cantidad de jugadores que participaron y el impacto en la actividad general del juego.
    </td>
  </tr>
</table>

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

<!-- USER STORY 41 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US41</th>
    <th>EPIC ID</th>
    <th>EPIC05</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Publicar Logros en la Comunidad</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> poder publicar mis logros en una sección dedicada de la comunidad, <strong>para</strong> compartir mis éxitos con otros jugadores y recibir retroalimentación.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario 1: Publicar un logro</strong><br>
      <strong>Given</strong> que estoy en la sección de logros,<br>
      <strong>When</strong> subo una imagen o descripción de mi logro,<br>
      <strong>Then</strong> el logro se publica en la comunidad.<br><br>
      <strong>Scenario 2: Visualización del logro</strong><br>
      <strong>Given</strong> que un logro ha sido publicado,<br>
      <strong>When</strong> otros jugadores acceden a la sección de logros,<br>
      <strong>Then</strong> pueden ver el logro publicado.
    </td>
  </tr>
</table>

<!-- USER STORY 42 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US42</th>
    <th>EPIC ID</th>
    <th>EPIC05</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Comentar en Logros de Otros Jugadores</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> poder comentar en los logros publicados por otros jugadores,<strong> para</strong> ofrecer retroalimentación y celebrar sus éxitos.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario 1: Publicar un comentario</strong><br>
      <strong>Given</strong> que estoy viendo un logro publicado por otro jugador,<br>
      <strong>When</strong> escribo un comentario y lo envío,<br>
      <strong>Then</strong> el comentario se muestra debajo del logro.<br><br>
      <strong>Scenario 2: Responder a comentarios</strong><br>
      <strong>Given</strong> que un comentario está en un logro,<br>
      <strong>When</strong> escribo una respuesta al comentario,<br>
      <strong>Then</strong> la respuesta se muestra debajo del comentario original.
    </td>
  </tr>
</table>

<!-- USER STORY 43 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US43</th>
    <th>EPIC ID</th>
    <th>EPIC05</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Dar "Me Gusta" a Logros</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> poder dar "me gusta" a los logros publicados por otros jugadores,<strong> para</strong> mostrar mi apreciación por sus éxitos.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario 1: Dar "Me Gusta"</strong><br>
      <strong>Given</strong> que estoy viendo un logro en la comunidad,<br>
      <strong>When</strong> hago clic en el botón "me gusta",<br>
      <strong>Then</strong> el número de "me gusta" del logro aumenta.<br><br>
      <strong>Scenario 2: Ver "Me Gusta"</strong><br>
      <strong>Given</strong> que un logro tiene "me gusta",<br>
      <strong>When</strong> otros jugadores ven el logro,<br>
      <strong>Then</strong> pueden ver el número total de "me gusta".
    </td>
  </tr>
</table>

<!-- USER STORY 44 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US44</th>
    <th>EPIC ID</th>
    <th>28</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Notificaciones de Nuevos Logros</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> recibir notificaciones cuando amigos o seguidores publiquen nuevos logros,<strong> para</strong> estar al tanto de sus éxitos y comentar o dar "me gusta" en sus publicaciones.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario 1: Recibir Notificación</strong><br>
      <strong>Given</strong> que un amigo publica un nuevo logro,<br>
      <strong>When</strong> la publicación se realiza,<br>
      <strong>Then</strong> recibo una notificación en mi perfil.<br><br>
      <strong>Scenario 2: Acceder a Notificaciones</strong><br>
      <strong>Given</strong> que he recibido notificaciones,<br>
      <strong>When</strong> accedo a la sección de notificaciones,<br>
      <strong>Then</strong> puedo ver una lista de los nuevos logros publicados por mis amigos y seguidores.
    </td>
  </tr>
</table>
<!-- USER STORY 45 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US45</th>
    <th>EPIC ID</th>
    <th>28</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Filtrar Logros por Tipo</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> filtrar los logros compartidos por tipo (ej. más difíciles, más recientes), <strong>para</strong> encontrar logros específicos que me interesen.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario 1: Aplicar Filtro</strong><br>
      <strong>Given</strong> que estoy en la sección de logros,<br>
      <strong>When</strong> selecciono un filtro de tipo,<br>
      <strong>Then</strong> solo se muestran los logros que coinciden con el filtro aplicado.<br><br>
      <strong>Scenario 2: Resetear Filtros</strong><br>
      <strong>Given</strong> que he aplicado un filtro,<br>
      <strong>When</strong> selecciono la opción de resetear filtros,<br>
      <strong>Then</strong> se muestran todos los logros sin filtrado.
    </td>
  </tr>
</table>
<!-- USER STORY 46 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US46</th>
    <th>EPIC ID</th>
    <th>28</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Mostrar Logros Destacados</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> ver una sección de logros destacados,<strong> para</strong> reconocer los logros más impresionantes y destacados en la comunidad.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario 1: Ver Logros Destacados</strong><br>
      <strong>Given</strong> que estoy en la sección de logros,<br>
      <strong>When</strong> accedo a la sección de logros destacados,<br>
      <strong>Then</strong> veo una lista de los logros que han sido seleccionados como destacados.<br><br>
      <strong>Scenario 2: Destacar un Logro</strong><br>
      <strong>Given</strong> que un logro ha sido publicado,<br>
      <strong>When</strong> el logro recibe una cantidad significativa de "me gusta" o comentarios,<br>
      <strong>Then</strong> puede ser destacado por los administradores.
    </td>
  </tr>
</table>
<!-- USER STORY 47 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US47</th>
    <th>EPIC ID</th>
    <th>28</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Crear y Gestionar Grupos de Logros</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> crear y gestionar grupos temáticos de logros,<strong> para</strong> compartir logros específicos dentro de grupos de interés y participar en competiciones.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario 1: Crear un Grupo</strong><br>
      <strong>Given</strong> que quiero crear un grupo de logros,<br>
      <strong>When</strong> defino el nombre y la descripción del grupo,<br>
      <strong>Then</strong> el grupo es creado y aparece en la lista de grupos.<br><br>
      <strong>Scenario 2: Unirse a un Grupo</strong><br>
      <strong>Given</strong> que hay grupos de logros disponibles,<br>
      <strong>When</strong> selecciono un grupo y solicito unirme,<br>
      <strong>Then</strong> puedo unirme al grupo y participar en las actividades.
    </td>
  </tr>
</table>
<!-- USER STORY 48 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US48</th>
    <th>EPIC ID</th>
    <th>28</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Comparar Logros con Amigos</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> comparar mis logros con los de mis amigos,<strong> para</strong> ver cómo me desempeño en comparación con ellos y encontrar motivación para mejorar.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario 1: Comparar Logros</strong><br>
      <strong>Given</strong> que estoy en la sección de comparación de logros,<br>
      <strong>When</strong> selecciono amigos para comparar,<br>
      <strong>Then</strong> veo una comparación de los logros entre yo y mis amigos.<br><br>
      <strong>Scenario 2: Ver Progreso Comparativo</strong><br>
      <strong>Given</strong> que estoy comparando logros,<br>
      <strong>When</strong> veo la comparación,<br>
      <strong>Then</strong> puedo ver gráficos o estadísticas que muestren el progreso comparativo.
    </td>
  </tr>
</table>
<!-- USER STORY 49 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US49</th>
    <th>EPIC ID</th>
    <th>28</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Gestionar Privacidad de Logros</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> gestionar la privacidad de mis logros,<strong> para</strong> decidir quién puede ver mis logros y quién no.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario 1: Configurar Privacidad</strong><br>
      <strong>Given</strong> que estoy configurando la privacidad de mis logros,<br>
      <strong>When</strong> selecciono opciones de privacidad,<br>
      <strong>Then</strong> mis logros se muestran según las configuraciones elegidas.<br><br>
      <strong>Scenario 2: Editar Privacidad</strong><br>
      <strong>Given</strong> que he publicado un logro,<br>
      <strong>When</strong> cambio las configuraciones de privacidad del logro,<br>
      <strong>Then</strong> los cambios se reflejan de inmediato.
    </td>
  </tr>
</table>
<!-- USER STORY 50 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US50</th>
    <th>EPIC ID</th>
    <th>28</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Incluir Medallas y Recompensas</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como gamer, <strong>quiero</strong> recibir medallas y recompensas por compartir logros importantes,<strong> para</strong> sentirme motivado y reconocer mis propios éxitos.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario 1: Ganar Medallas</strong><br>
      <strong>Given</strong> que he publicado un logro significativo,<br>
      <strong>When</strong> el logro es aprobado,<br>
      <strong>Then</strong> recibo una medalla o recompensa asociada al logro.<br><br>
      <strong>Scenario 2: Mostrar Medallas</strong><br>
      <strong>Given</strong> que he recibido medallas,<br>
      <strong>When</strong> otros jugadores visitan mi perfil,<br>
      <strong>Then</strong> pueden ver las medallas y recompensas que he ganado.
    </td>
  </tr>
</table>

<!-- EPIC 06 -->
<table>
  <tr>
    <th>EPIC ID</th>
    <th>06</th>
    <th>TITLE: Accesibilidad de la Landing Page</th>
  </tr>
  <tr>
    <td colspan="3">
      <strong>Cómo</strong> visitante de la Landing Page, 
      <strong>quiero</strong> que la información sobre la aplicación sea fácil de entender 
      <strong>para</strong> poder comprender rápidamente su propósito.
    </td>
  </tr>
</table>

<!-- USER STORIE 51 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US51</th>
    <th>EPIC ID</th>
    <th>EP06</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Adaptabilidad y compatibilidad de la Landing Page</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como visitante de la Landing Page, <strong>quiero</strong> que el contenido se adapte al tamaño de la pantalla del dispositivo desde el que accede <strong>para</strong> obtener la información de manera ordenada.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario 1: Adaptabilidad a diferentes tamaños de pantalla</strong><br>
      <strong>Given</strong> el visitante se encuentra en la landing page,<br>
      <strong>When</strong> ingresa al sitio web,<br>
      <strong>Then</strong> la landing page debe poseer un contenido que se ajuste automáticamente al tamaño de la pantalla.<br><br>
      <strong>Scenario 2: Compatibilidad con navegadores principales</strong><br>
      <strong>Given</strong> el visitante se encuentra en la landing page,<br>
      <strong>When</strong> utiliza su navegador de preferencia,<br>
      <strong>Then</strong> la landing page debe ser compatible.
    </td>
  </tr>
</table>

<!-- USER STORIE 52 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US52</th>
    <th>EPIC ID</th>
    <th>EP06</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Encontrar información del propósito de la aplicación</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como visitante de la Landing Page, <strong>quiero</strong> encontrar fácilmente la información que explique el propósito de la aplicación <strong>para</strong> comprender cómo puede ser útil para mí.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario 1: Visibilidad del propósito de la aplicación</strong><br>
      <strong>Given</strong> el visitante se encuentra en la landing page,<br>
      <strong>When</strong> explora la página principal,<br>
      <strong>Then</strong> la landing page debe poseer información clara y concisa para el visitante.<br><br>
      <strong>Scenario 2: Acceso rápido a los planes de la aplicación</strong><br>
      <strong>Given</strong> el visitante se encuentra en la sección de planes de la landing page,<br>
      <strong>When</strong> hace clic en un botón de “Más información”,<br>
      <strong>Then</strong> la landing page debe dirigirlo a una sección que detalle las características y precios del plan seleccionado.
    </td>
  </tr>
</table>

<!-- USER STORY 53 -->
<table>
  <tr>
    <th>USER STORY ID</th>
    <th>US53</th>
    <th>EPIC ID</th>
    <th>EP06</th>
  </tr>
  <tr>
    <th>TITLE</th>
    <td colspan="3">Acceso a Soporte Técnico</td>
  </tr>
  <tr>
    <th>DESCRIPTION</th>
    <td colspan="3">Como visitante de la Landing Page, <strong>quiero</strong> tener fácil acceso a soporte técnico <strong>para</strong> resolver cualquier duda o problema relacionado con la aplicación.</td>
  </tr>
  <tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
      <strong>Scenario 1: Acceso a soporte en tiempo real</strong><br>
      <strong>Given</strong> el visitante accede a la landing page,<br>
      <strong>When</strong> busca ayuda en la sección de soporte,<br>
      <strong>Then</strong> la página ofrece la opción de contactar con un agente en tiempo real o buscar en una base de conocimientos.
    </td>
  </tr>
</table>

<!-- EPIC 07 -->
<table>
<tr>
    <th>EPIC ID</th>
    <th>07</th>
</tr>
<tr>
    <th>TITLE</th>
    <td colspan="3">Gestión de APIS del Backend para Funcionalidades del Usuario</td>
</tr>
<tr>
    <th>DESCRIPTION</th>
    <td colspan="3">
        <strong>Cómo</strong> visitante de la aplicación web, 
        <strong>quiero</strong> que las funcionalidades de login, registro, perfil, juegos favoritos y suscripción estén disponibles a través de APIs bien definidas,
        <strong>para</strong> asegurar una comunicación eficiente con el frontend y que los datos se presenten en el formato JSON esperado.
    </td>
</tr>
</table>

<!-- USER STORY 54 -->
<table>
<tr>
    <th>USER STORY ID</th>
    <th>US54</th>
</tr>
<tr>
    <th>EPIC ID</th>
    <th>EP07</th>
</tr>
<tr>
    <th>TITLE</th>
    <td colspan="3">API para Login de Usuarios</td>
</tr>
<tr>
    <th>DESCRIPTION</th>
    <td colspan="3">
        <strong>Como</strong> usuario de la aplicación, 
        <strong>quiero</strong> poder autenticarme ingresando mis credenciales, 
        <strong>para</strong> acceder a mis datos personales de forma segura.
    </td>
</tr>
<tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
        <strong>Scenario 1: Autenticación de usuario exitosa</strong><br>
        <strong>Given</strong> el usuario ingresa su email y contraseña correctos,<br>
        <strong>When</strong> realiza una solicitud de login a la API,<br>
        <strong>Then</strong> recibe un token de autenticación en formato JSON.<br><br>
</tr>
</table>

<!-- USER STORY 55 -->
<table>
<tr>
    <th>USER STORY ID</th>
    <th>US55</th>
</tr>
<tr>
    <th>EPIC ID</th>
    <th>EP07</th>
</tr>
<tr>
    <th>TITLE</th>
    <td colspan="3">API para Registro de Nuevos Usuarios</td>
</tr>
<tr>
    <th>DESCRIPTION</th>
    <td colspan="3">
        <strong>Como</strong> nuevo usuario de la aplicación, 
        <strong>quiero</strong> poder registrarme proporcionando mis datos básicos, 
        <strong>para</strong> crear una cuenta y acceder a las funcionalidades de la aplicación.
    </td>
</tr>
<tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
        <strong>Scenario: Registro de usuario exitoso</strong><br>
        <strong>Given</strong> el usuario ingresa sus datos de registro válidos,<br>
        <strong>When</strong> envía la solicitud de registro a la API,<br>
        <strong>Then</strong> la cuenta se crea y la API devuelve un mensaje de confirmación en JSON.
    </td>
</tr>
</table>

<!-- USER STORY 56 -->
<table>
<tr>
    <th>USER STORY ID</th>
    <th>US56</th>
</tr>
<tr>
    <th>EPIC ID</th>
    <th>EP07</th>
</tr>
<tr>
    <th>TITLE</th>
    <td colspan="3">API para Perfil de Usuario</td>
</tr>
<tr>
    <th>DESCRIPTION</th>
    <td colspan="3">
        <strong>Como</strong> usuario autenticado, 
        <strong>quiero</strong> poder ver y actualizar mi perfil, 
        <strong>para</strong> mantener mi información personal actualizada en la aplicación.
    </td>
</tr>
<tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
        <strong>Scenario: Actualización de perfil exitosa</strong><br>
        <strong>Given</strong> el usuario está autenticado y accede a su perfil,<br>
        <strong>When</strong> envía datos actualizados a la API de perfil,<br>
        <strong>Then</strong> la API actualiza la información y devuelve la confirmación en JSON.
    </td>
</tr>
</table>

<!-- USER STORY 57 -->
<table>
<tr>
    <th>USER STORY ID</th>
    <th>US57</th>
</tr>
<tr>
    <th>EPIC ID</th>
    <th>EP07</th>
</tr>
<tr>
    <th>TITLE</th>
    <td colspan="3">API para Juegos Favoritos</td>
</tr>
<tr>
    <th>DESCRIPTION</th>
    <td colspan="3">
        <strong>Como</strong> usuario autenticado, 
        <strong>quiero</strong> poder gestionar mis juegos favoritos, 
        <strong>para</strong> acceder rápidamente a los juegos que más me interesan.
    </td>
</tr>
<tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
        <strong>Scenario: Agregar un juego a favoritos</strong><br>
        <strong>Given</strong> el usuario está autenticado y selecciona un juego,<br>
        <strong>When</strong> envía una solicitud a la API para agregar el juego a favoritos,<br>
        <strong>Then</strong> el juego se añade a la lista de favoritos y la API devuelve la confirmación.<br><br>
</tr>
</table>

<!-- USER STORY 58 -->
<table>
<tr>
    <th>USER STORY ID</th>
    <th>US58</th>
</tr>
<tr>
    <th>EPIC ID</th>
    <th>EP07</th>
</tr>
<tr>
    <th>TITLE</th>
    <td colspan="3">API para Gestión de Suscripciones</td>
</tr>
<tr>
    <th>DESCRIPTION</th>
    <td colspan="3">
        <strong>Como</strong> usuario de la aplicación, 
        <strong>quiero</strong> gestionar mi suscripción, 
        <strong>para</strong> acceder a los beneficios de mi plan y renovar cuando sea necesario.
    </td>
</tr>
<tr>
    <th>ACCEPTANCE CRITERIA</th>
    <td colspan="3">
        <strong>Scenario: Renovación de suscripción exitosa</strong><br>
        <strong>Given</strong> el usuario desea renovar su suscripción,<br>
        <strong>When</strong> realiza una solicitud de renovación a la API,<br>
        <strong>Then</strong> la suscripción se renueva y la API devuelve la confirmación en JSON.
    </td>
</tr>
</table>


## 3.3. Impact Mapping

### Gamers

<img src="/assets/chapter03/impact-mapping-image/Impact-Mapping-gamers.png" alt="impact-mapping-gamers" />

### Desarrolladoras de Videojuegos

<img src="/assets/chapter03/impact-mapping-image/Impact-Mapping-desarrolladoras.png" alt="impact-mapping-desarrolladoras" />

## 3.4. Product Backlog

<table>
  <tr>
    <th>Orden</th>
    <th>User Story Id</th>
    <th>Título</th>
    <th>Descripción</th>
    <th>Story Points</th>
  </tr>
  <tr>
    <td>1</td>
    <td>US01</td>
    <td>Filtrado de Juegos por Género</td>
    <td>Como gamer, quiero poder filtrar juegos por género para encontrar rápidamente aquellos que me interesan.</td>
    <td>2</td>
  </tr>
  <tr>
    <td>2</td>
    <td>US15</td>
    <td>Búsqueda de Juegos por Palabra Clave</td>
    <td>Como gamer, quiero buscar juegos usando palabras clave, para encontrar juegos específicos rápidamente.</td>
    <td>2</td>
  </tr>
  <tr>
    <td>3</td>
    <td>US11</td>
    <td>Sistema de Revisión de Juegos</td>
    <td>Como gamer, quiero ver reseñas de otros jugadores antes de comprar un juego, para tomar una mejor decisión de compra.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>4</td>
    <td>US16</td>
    <td>Acceso a Demos de Juegos</td>
    <td>Como gamer, quiero poder acceder a demos de juegos antes de comprarlos, para probar si me gustan antes de hacer una compra.</td>
    <td>3</td>
  </tr>
  <tr>
    <td rowspan="3">5</td>
    <td rowspan="3">US02</td>
    <td rowspan="3">Recomendaciones Basadas en Género Favorito</td>
    <td>Como gamer, quiero recibir recomendaciones de juegos en mi género favorito para descubrir más juegos similares.</td>
    <td rowspan="2">3</td>
  </tr>
  <tr>
    <td>Como gamer, quiero que me recomienden juegos similares a aquellos en los que he invertido más tiempo, para seguir disfrutando de ese tipo de juegos.</td>
  </tr>
  <tr>
    <td>Como gamer, quiero ver los juegos más populares entre mis amigos para descubrir qué están jugando.</td>
    <td>5</td>

  <tr>
    <td rowspan="2">6</td>
    <td rowspan="2">US04</td>
    <td rowspan="2">Recomendaciones Basadas en Tiempo Jugado</td>
    <td>Como gamer, quiero que me recomienden juegos similares a aquellos en los que he invertido más tiempo, para seguir disfrutando de ese tipo de juegos.</td>
    <td rowspan="2">5</td>
  </tr>
  <tr>
    <td>Como gamer, quiero ver los juegos más populares entre mis amigos para descubrir qué están jugando.</td>
  </tr>
  <tr>
    <td>7</td>
    <td>US03</td>
    <td>Recomendaciones Basadas en Popularidad entre Amigos</td>
    <td>Como gamer, quiero ver los juegos más populares entre mis amigos para descubrir qué están jugando.</td>
    <td>5</td>
  </tr>
  <tr>
    <td>8</td>
    <td>US22</td>
    <td>Modo Offline para Juegos Indie</td>
    <td>Como gamer, quiero que algunos juegos indie sean jugables en modo offline, para poder jugar incluso sin conexión a internet.</td>
    <td>5</td>
  </tr>
  <tr>
    <td>9</td>
    <td>US05</td>
    <td>Invitación a Amigos para Jugar</td>
    <td>Como gamer, quiero invitar a mis amigos a jugar un juego conmigo, para compartir experiencias de juego.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>10</td>
    <td>US06</td>
    <td>Chat en Tiempo Real</td>
    <td>Como gamer, quiero un sistema de chat en tiempo real, para comunicarme con mis amigos mientras jugamos juntos.</td>
    <td>5</td>
  <tr>
    <td>11</td>
    <td>US14</td>
    <td>Creación de Comunidades de Juego</td>
    <td>Como gamer, quiero unirme a comunidades de jugadores de un mismo juego, para compartir estrategias y experiencias.</td>
    <td>5</td>
  </tr>
  <tr>
    <td>12</td>
    <td>US17</td>
    <td>Personalización de Perfil de Jugador</td>
    <td>Como gamer, quiero personalizar mi perfil en la plataforma para reflejar mis gustos y mostrar mi progreso en los juegos.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>13</td>
    <td>US19</td>
    <td>Visualización de Rankings de Jugadores</td>
    <td>Como gamer, quiero ver mi posición en el ranking de jugadores de un juego, para comparar mi progreso con el de otros jugadores.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>14</td>
    <td>US20</td>
    <td>Sistema de Logros</td>
    <td>Como gamer, quiero desbloquear logros en los juegos que juego, para mejorar mi experiencia y ganar recompensas.</td>
    <td>5</td>
  </tr>
  <tr>
    <td>15</td>
    <td>US21</td>
    <td>Notificaciones en Tiempo Real</td>
    <td>Como gamer, quiero recibir notificaciones en tiempo real cuando mis amigos comiencen a jugar un nuevo juego, para unirme a ellos de inmediato.</td>
    <td>5</td>
  </tr>
    <tr>
    <td>16</td>
    <td>US07</td>
    <td>Compartir Reseñas de Juegos</td>
    <td>Como gamer, quiero compartir reseñas de los juegos que he jugado, para ayudar a otros jugadores a decidir si quieren probarlos.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>17</td>
    <td>US08</td>
    <td>Publicar Juego Indie</td>
    <td>Como desarrollador, quiero poder publicar mi juego indie en la plataforma, para llegar a una audiencia más amplia.</td>
    <td>8</td>
  </tr>
  <tr>
    <td>18</td>
    <td>US12</td>
    <td>Subir Actualizaciones de Juegos</td>
    <td>Como desarrollador, quiero subir actualizaciones para mi juego publicado, para corregir errores y mejorar la experiencia del usuario.</td>
    <td>5</td>
  </tr>
  <tr>
    <td>19</td>
    <td>US09</td>
    <td>Actualización de Juegos Indie</td>
    <td>Como desarrollador, quiero poder actualizar la información de mi juego indie para corregir errores o agregar nuevas características.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>20</td>
    <td>US18</td>
    <td>Notificaciones en Tiempo Real</td>
    <td>Como gamer, quiero recibir notificaciones en tiempo real cuando mis amigos comiencen a jugar un nuevo juego, para unirme a ellos de inmediato.</td>
    <td>8</td>
  </tr>
    <tr>
    <td>21</td>
    <td>US10</td>
    <td>Visualización de Métricas de Jugadores</td>
    <td>Como desarrollador, quiero ver métricas detalladas sobre cómo los jugadores interactúan con mi juego, para mejorar la experiencia del usuario.</td>
    <td>8</td>
  </tr>
  <tr>
    <td>22</td>
    <td>US13</td>
    <td>Análisis de Comportamiento de Jugadores</td>
    <td>Como desarrollador, quiero analizar el comportamiento de los jugadores para identificar puntos de fricción en mi juego.</td>
    <td>8</td>
  </tr>
  <tr>
    <td>23</td>
    <td>US30</td>
    <td>Generación de Reportes de Desempeño</td>
    <td>Como desarrollador indie, quiero generar reportes sobre el desempeño de mi juego para obtener información detallada sobre cómo está siendo recibido por los jugadores.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>24</td>
    <td>US31</td>
    <td>Visualización de Métricas de Jugadores</td>
    <td>Como desarrollador, quiero ver métricas detalladas sobre cómo los jugadores interactúan con mi juego para mejorar la experiencia del usuario.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>25</td>
    <td>US32</td>
    <td>Análisis de Comportamiento de Jugadores</td>
    <td>Como desarrollador, quiero analizar el comportamiento de los jugadores para identificar puntos de fricción en mi juego.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>26</td>
    <td>US33</td>
    <td>Visualización de Datos de Uso del Juego</td>
    <td>Como desarrollador, quiero visualizar datos detallados sobre el uso del juego para entender mejor cómo los jugadores interactúan con mi juego.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>27</td>
    <td>US34</td>
    <td>Análisis de Puntos de Fricción</td>
    <td>Como desarrollador, quiero analizar los puntos de fricción en el juego para identificar y solucionar problemas que afectan la experiencia del usuario.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>28</td>
    <td>US35</td>
    <td>Seguimiento de Progreso de Jugadores</td>
    <td>Como desarrollador, quiero hacer un seguimiento del progreso de los jugadores para comprender cómo están avanzando en el juego y ajustar la dificultad si es necesario.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>29</td>
    <td>US36</td>
    <td>Análisis de Tendencias de Juego</td>
    <td>Como desarrollador, quiero analizar las tendencias de juego para identificar qué características o niveles están siendo más populares entre los jugadores.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>30</td>
    <td>US37</td>
    <td>Comparación de Métricas entre Juegos</td>
    <td>Como desarrollador, quiero comparar las métricas de diferentes juegos para entender qué elementos contribuyen al éxito de un juego en comparación con otros.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>31</td>
    <td>US38</td>
    <td>Evaluación de la Retención de Jugadores</td>
    <td>Como desarrollador, quiero evaluar la retención de jugadores para entender qué tan bien está manteniendo el interés de los jugadores en mi juego a lo largo del tiempo.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>32</td>
    <td>US39</td>
    <td>Reporte de Feedback de Jugadores</td>
    <td>Como desarrollador, quiero generar reportes de feedback de jugadores para obtener una visión general de las opiniones y sugerencias de los usuarios sobre el juego.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>33</td>
    <td>US40</td>
    <td>Análisis de Participación en Eventos del Juego</td>
    <td>Como desarrollador, quiero analizar la participación en eventos dentro del juego para evaluar el impacto de estos eventos en la actividad de los jugadores y su engagement.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>34</td>
    <td>US41</td>
    <td>Publicar Logros en la Comunidad</td>
    <td>Como gamer, quiero poder publicar mis logros en una sección dedicada de la comunidad, para compartir mis éxitos con otros jugadores y recibir retroalimentación.</td>
    <td>2</td>
  </tr>
  <tr>
    <td>35</td>
    <td>US42</td>
    <td>Comentar en Logros de Otros Jugadores</td>
    <td>Como gamer, quiero poder comentar en los logros publicados por otros jugadores, para ofrecer retroalimentación y celebrar sus éxitos.</td>
    <td>2</td>
  </tr>
    <tr>
    <td>36</td>
    <td>US23</td>
    <td>Subir Actualizaciones de Juegos</td>
    <td>Como desarrollador, quiero subir actualizaciones para mi juego publicado para corregir errores y mejorar la experiencia del usuario.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>37</td>
    <td>US24</td>
    <td>Creación de Torneos</td>
    <td>Como desarrollador, quiero crear torneos para mi juego para fomentar la competencia entre los jugadores.</td>
    <td>1</td>
  </tr>
  <tr>
    <td>38</td>
    <td>US25</td>
    <td>Subir Juegos Indie a la Plataforma</td>
    <td>Como desarrollador indie, quiero subir mis juegos a la plataforma para que puedan ser vistos y descargados por los jugadores.</td>
    <td>5</td>
  </tr>
  <tr>
    <td>39</td>
    <td>US26</td>
    <td>Gestión de Información del Juego</td>
    <td>Como desarrollador indie, quiero gestionar la información de mi juego para actualizar detalles, corregir errores o agregar contenido nuevo.</td>
    <td>5</td>
  </tr>
  <tr>
    <td>40</td>
    <td>US27</td>
    <td>Gestión de Precios y Ofertas</td>
    <td>Como desarrollador indie, quiero establecer y gestionar precios y ofertas para mi juego para atraer a más jugadores y aumentar las ventas.</td>
    <td>4</td>
  </tr>
  <tr>
    <td>41</td>
    <td>US28</td>
    <td>Monitoreo de Descargas y Ventas</td>
    <td>Como desarrollador indie, quiero monitorear las descargas y ventas de mi juego para analizar su desempeño en la plataforma.</td>
    <td>4</td>
  </tr>
  <tr>
    <td>42</td>
    <td>US29</td>
    <td>Responder a Reseñas de Jugadores</td>
    <td>Como desarrollador indie, quiero responder a las reseñas de jugadores para interactuar con mi audiencia y abordar sus comentarios o problemas.</td>
    <td>1</td>
  </tr>
  <tr>
    <td>43</td>
    <td>US44</td>
    <td>Notificaciones de Nuevos Logros</td>
    <td>Como gamer, quiero recibir notificaciones cuando amigos o seguidores publiquen nuevos logros, para estar al tanto de sus éxitos y comentar o dar "me gusta" en sus publicaciones.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>44</td>
    <td>US45</td>
    <td>Filtrar Logros por Tipo</td>
    <td>Como gamer, quiero filtrar los logros compartidos por tipo (ej. más difíciles, más recientes), para encontrar logros específicos que me interesen.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>45</td>
    <td>US46</td>
    <td>Mostrar Logros Destacados</td>
    <td>Como gamer, quiero ver una sección de logros destacados, para reconocer los logros más impresionantes y destacados en la comunidad.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>46</td>
    <td>US47</td>
    <td>Crear y Gestionar Grupos de Logros</td>
    <td>Como gamer, quiero crear y gestionar grupos temáticos de logros, para compartir logros específicos dentro de grupos de interés y participar en competiciones.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>47</td>
    <td>US48</td>
    <td>Comparar Logros con Amigos</td>
    <td>Como gamer, quiero comparar mis logros con los de mis amigos, para ver cómo me desempeño en comparación con ellos y encontrar motivación para mejorar.</td>
    <td>2</td>
  </tr>
  <tr>
    <td>48</td>
    <td>US49</td>
    <td>Gestionar Privacidad de Logros</td>
    <td>Como gamer, quiero gestionar la privacidad de mis logros, para decidir quién puede ver mis logros y quién no.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>49</td>
    <td>US50</td>
    <td>Incluir Medallas y Recompensas</td>
    <td>Como gamer, quiero recibir medallas y recompensas por compartir logros importantes, para sentirme motivado y reconocer mis propios éxitos.</td>
    <td>2</td>
  </tr>
  <tr>
    <td>43</td>
    <td>US43</td>
    <td>Dar "Me Gusta" a Logros</td>
    <td>Como gamer, quiero poder dar "me gusta" a los logros publicados por otros jugadores, para mostrar mi apreciación por sus éxitos.</td>
    <td>3</td>
  </tr>
  <tr>
  <td>51</td>
  <td>US51</td>
  <td>Adaptabilidad y compatibilidad de la Landing Page</td>
  <td>Como visitante de la Landing Page, quiero que el contenido se adapte al tamaño de la pantalla del dispositivo desde el que accede para obtener la información de manera ordenada.</td>
  <td>5</td>
  </tr>
  <tr>
  <td>52</td>
  <td>US52</td>
  <td>Encontrar información del propósito de la aplicación</td>
  <td>Como visitante de la Landing Page, quiero encontrar fácilmente la información que explique el propósito de la aplicación para comprender cómo puede ser útil para mí.</td>
  <td>3</td>
  </tr>
  <tr>
  <td>53</td>
  <td>US53</td>
  <td>Acceso a Soporte Técnico</td>
  <td>Como visitante de la Landing Page, quiero tener fácil acceso a soporte técnico para resolver cualquier duda o problema relacionado con la aplicación.</td>
  <td>2</td>
  </tr>
</table>

