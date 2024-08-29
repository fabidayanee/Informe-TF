# Capítulo III: Requirements Specification

## 3.1. To-Be Scenario Mapping

Luego de realizar el as-is con sus fases propuestas, para el to-be se realizaron nuevos procesos enfocados en mejorar las fases de los segmentos objetivos con nuestro proyecto. 

**_Segmento Objetivo 1: Abogados especializados en derecho médico_**
![alt text](<https://raw.githubusercontent.com/LexMedd/Informe-TF/Chapter-03/assets/imgs/TOBE%20scenario%20abogados.jpeg>)

**_Segmento Objetivo 2: Doctores que enfrentan problemas legales por mala praxis_**
![alt text](<https://raw.githubusercontent.com/LexMedd/Informe-TF/Chapter-03/assets/imgs/TOBE%20scenario%20doctores.jpeg>)

## 3.2. User Stories

Los User Stories describen las funciones de la aplicación adaptadas a las necesidades y prioridades de los usuarios, proporcionando una comprensión más completa de cómo se relacionan con la plataforma y qué esperan lograr con ella.

<table>
    <tr>
        <th>Epic / Story ID</th>
        <th>Título</th>
        <th>Descripción</th>
        <th>Criterios de Aceptación</th>
        <th>Relacionado con (Epic ID)</th>
    </tr>
    <tr>
        <td>EP01</td>
        <td>Funciones de usuario</td>
        <td>Como usuario, deseo tener funciones y opciones relacionadas a mi necesidad para manejar mis datos y acciones en la cuenta.</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>EP02</td>
        <td>Visualizacion de Apartados</td>
        <td>Como usuario, deseo tener opciones de detalles y búsqueda para visualizar los datos que me interesan en la plataforma.<</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>EP03</td>
        <td>Landing Page</td>
        <td>Como usuario de la plataforma, deseo visitar una Landing Page para informarme sobre LexMedd y lo que ofrece.</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>EP04</td>
        <td>Interacción con el usuario a tratar</td>
        <td>Como usuario, deseo tener funciones y opciones relacionadas a mi necesidad 
para tratar con él u opinar de sus servicios.</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>EP05</td>
        <td>Infraestructura y Seguridad</td>
        <td>Como administrador, quiero que la plataforma integre robustos sistemas de seguridad y manejo de datos, para proteger la información de los usuarios.</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>EP06</td>
        <td>Interacción y Accesibilidad</td>
        <td>Como desarrollador, quiero implementar interfaces y funcionalidades accesibles para mejorar la interacción del usuario con la plataforma.</td>
        <td></td>
        <td></td>
    </tr>
     <td>HU01</td>
        <td>Registro de un nuevo abogado especializado</td>
        <td>Como abogado especializado en derecho médico quiero registrarme en la plataforma LEXMED para ofrecer mis servicios.</td>
        <td>Scenario: Registro exitoso de abogado<br><br>GIVEN que el abogado accede a la página de registro,<br><br>WHEN completa todos los campos obligatorios y envía el formulario,<br><br>AND el sistema valida que los datos son correctos,<br><br>THEN el abogado debe recibir una confirmación de registro y acceso a su perfil.</td>
        <td>EP01</td>
    </tr>
    <tr>
        <td>HU02</td>
        <td>Solicitud de casos por parte de un abogado</td>
        <td>Como abogado especializado en derecho médico solicito recibir casos relacionados con mi área de expertise.</td>
        <td>Scenario: Solicitud de casos por área de expertise<br><br>GIVEN que el abogado está registrado y ha accedido a su perfil,<br><br>WHEN selecciona las áreas de expertise en las que desea recibir casos,<br><br>AND guarda sus preferencias,<br><br>THEN el sistema debe actualizar sus preferencias y mostrar los casos correspondientes en su panel de control.</td>
        <td>EP02</td>
    </tr>
    <tr>
        <td>HU03</td>
        <td>Subida de un caso médico</td>
        <td>Como médico quiero subir mi caso relacionado con una posible negligencia médica en la plataforma para que los abogados puedan verlo.</td>
        <td>Scenario: Subida de un caso médico<br><br>GIVEN que el médico ha iniciado sesión en la plataforma,<br><br>WHEN completa el formulario para subir un caso médico,<br><br>AND adjunta la documentación necesaria,<br><br>THEN el caso debe ser publicado en la plataforma y visible para los abogados especializados.</td>
        <td>EP01</td>
    </tr>
    <tr>
        <td>HU04</td>
        <td>Evaluación de casos por parte de los abogados</td>
        <td>Como abogado quiero evaluar casos médicos publicados en la plataforma para decidir si deseo tomar el caso.</td>
        <td>Scenario: Evaluación de casos médicos<br>
        <br>GIVEN que el abogado tiene acceso a su panel de control,<br>
        <br>WHEN revisa la lista de casos médicos disponibles,<br><br>AND selecciona un caso para revisar sus detalles,<br><br>THEN debe poder ver la información del caso y decidir si desea postularse para representarlo.</td>
        <td>EP01</td>
    </tr>
    <tr>
        <td>HU05</td>
        <td>Notificación al médico sobre el interés de un abogado</td>
        <td>Como médico quiero recibir una notificación cuando un abogado se interese en mi caso.</td>
        <td>Scenario: Notificación de interés en el caso<br>
        <br>GIVEN que un abogado se ha postulado para representar el caso del médico,<br>
        <br>WHEN el abogado envía su postulación,<br>
        <br>AND el sistema procesa la solicitud,<br>
        <br>THEN el médico debe recibir una notificación sobre el interés del abogado en su caso.</td>
        <td>EP01</td>
    </tr>
    <tr>
        <td>HU06</td>
        <td>Generación de reporte de casos y abogados</td>
        <td>Como administrador quiero generar un reporte de todos los casos médicos y abogados registrados en la plataforma.</td>
        <td>Scenario: Generación de reportes<br>
    <br>GIVEN que un abogado se ha postulado para representar el caso del médico,<br>
    <br>WHEN el abogado envía su postulación,<br>
    <br>AND el sistema procesa la solicitud,<br>
    <br>THEN el médico debe recibir una notificación sobre el interés del abogado en su caso.</td>
        <td>EP06</td>
    </tr>
    <tr>
    <td>HU07</td>
        <td>Actualización de perfil del abogado</td>
        <td>Como abogado quiero actualizar mi perfil con información adicional o correcciones.</td>
        <td>Scenario: Actualización de perfil<br>
    <br>GIVEN que el abogado ha iniciado sesión y accede a su perfil,<br>
    <br>WHEN realiza cambios en la información de su perfil,<br>
    <br>AND guarda los cambios,<br>
    <br>THEN el perfil debe actualizarse con la nueva información y reflejarse en la plataforma.</td>
        <td>EP01</td>
    </tr>
    <tr>
    <td>HU08</td>
        <td>Filtrado de casos por área de especialización</td>
        <td>Como abogado quiero filtrar los casos médicos en la plataforma según su área de especialización.</td>
        <td>Scenario: Filtrado de casos<br>
    <br>GIVEN que el abogado está en la sección de casos médicos,<br>
    <br>WHEN selecciona un área de especialización para filtrar,<br>
    <br>AND aplica el filtro,<br>
    <br>THEN el sistema debe mostrar solo los casos relevantes para esa área de especialización.</td>
        <td>EP02</td>
    </tr>
    <tr>
   <td>HU09</td>
    <td>Búsqueda de abogados por especialización</td>
    <td>Como médico quiero buscar abogados especializados en un área específica para su caso.</td>
    <td>Scenario: Búsqueda de abogados<br><br>GIVEN que el médico está en la sección de búsqueda de abogados,<br><br>WHEN ingresa un área de especialización en el buscador,<br><br>AND realiza la búsqueda,<br><br>THEN el sistema debe mostrar una lista de abogados especializados en esa área.</td>
    <td>EP02</td>
    </tr>
     <tr>
    <td>HU10</td>
    <td>Notificación de nuevos casos al abogado</td>
    <td>Como abogado quiero recibir una notificación cuando un nuevo caso relacionado con mi área de especialización es publicado.</td>
    <td>Scenario: Notificación de nuevos casos<br><br>GIVEN que el abogado ha seleccionado áreas de especialización,<br><br>WHEN se publica un nuevo caso en esas áreas,<br><br>AND el sistema envía una notificación al abogado,<br><br>THEN el abogado debe recibir la notificación con los detalles del nuevo caso.</td>
    <td>EP02</td>
  </tr>
  <tr>
    <td>HU11</td>
    <td>Postulación a un caso por parte de un abogado</td>
    <td>Como abogado quiero postularme para representar un caso específico publicado por un médico.</td>
    <td>Scenario: Postulación a un caso<br><br>GIVEN que el abogado está en la vista del caso médico,<br><br>WHEN decide postularse para el caso,<br><br>AND envía su postulación,<br><br>THEN el sistema debe registrar la postulación y notificar al médico.</td>
    <td>EP02</td>
  </tr>
  <tr>
    <td>HU12</td>
    <td>Confirmación de recepción de documentos del caso</td>
    <td>Como médico quiero confirmar que he recibido los documentos enviados por un abogado.</td>
    <td>Scenario: Confirmación de documentos<br><br>GIVEN que el abogado ha enviado documentos relacionados con el caso,<br><br>WHEN el médico accede a su panel de control,<br><br>AND revisa los documentos recibidos,<br><br>THEN el sistema debe permitir al médico confirmar la recepción de los documentos.</td>
    <td>EP04</td>
  </tr>
    <tr>
    <td>HU13</td>
        <td>Registro de un nuevo caso por un médico</td>
        <td>Como médico quiero crear un nuevo caso en la plataforma LEXMED para su revisión.</td>
        <td>Scenario: Registro de nuevo caso<br><br>GIVEN que el médico ha iniciado sesión en la plataforma,<br><br>WHEN completa el formulario de registro de caso,<br><br>AND adjunta los documentos necesarios,<br><br>THEN el caso debe ser publicado y visible para los abogados.</td>
        <td>EP01</td>
    </tr>
    <tr>
    <td>HU14</td>
        <td>Creación de la landing page</td>
        <td>Como usuario quiero acceder a una página de inicio que presenta información relevante sobre LEXMED y sus servicios.</td>
        <td>Scenario: Visualización de la landing page<br><br>GIVEN que un usuario visita la página de inicio,<br><br>WHEN carga la página,<br><br>AND visualiza los elementos de contenido como descripción de servicios, testimonios, y llamadas a la acción,<br><br>THEN la landing page debe cargar correctamente y mostrar toda la información de manera clara.</td>
        <td>EP06</td>
    </tr>
    <tr>
    <td>HU15</td>
        <td>Sección about us</td>
        <td>Como visitante de la landing page de LEXMED, quiero ver una sección de about us para informarme sobre la empresa que está brindando los servicios.</td>
        <td>Scenario: Visualización de una sección about us<br><br>GIVEN un visitante explora la landing page,<br><br>WHEN se encuentre navegando por la landing page,<br><br>THEN encuentra una sección about us que le brinda información acerca de la empresa cuyos servicios le interesan.</td>
        <td>EP03</td>
    </tr>
    <tr>
    <td>HU16</td>
        <td>Sección de Creadores</td>
        <td>Como visitante de la landing page de LEXMED, quiero ver una sección de creadores para facilitar tener el conocimiento de los creadores de la empresa.</td>
        <td>Scenario: Visualización de una sección creadores<br>
    <br>GIVEN un visitante accede a la landing page,
<br>
    <br>WHEN se encuentre navegando por la landing page,<br><br>
    THEN encuentra una sección creadores que le brinda información acerca de los creadores de la empresa.</td>
        <td>EP03</td>
    </tr>
    <tr>
    <td>HU17</td>
        <td>Sección de inicio</td>
        <td>Como visitante de la landing page de LEXMED, quiero ver una sección de inicio con una barra de navegación para poder desplazarme mejor por la landing page.</td>
        <td>Scenario: Visualización de una sección inicio<br>
    <br>GIVEN un visitante ingresa a la landing page,<br>
    <br>WHEN se encuentre navegando por la landing page,<br>
    <br>THEN encuentra una sección inicio que tenga una barra de navegación donde puede ver el logo para poder desplazarse mejor.</td>
        <td>EP03</td>
    </tr>
    <tr>
    <td>HU18</td>
        <td>Integración de pagos</td>
        <td>Como administrador, quiero integrar un sistema de pagos seguro para gestionar las suscripciones y compras en la plataforma.</td>
        <td>Scenario: Implementar un proceso de pago seguro para las suscripciones.<br><br>GIVEN el administrador ha elegido implementar un sistema de pagos seguro,<br><br>WHEN el administrador configura la información del método de pago y confirma la configuración,<br><br>AND el sistema verifica la validez de la información de pago,<br><br>THEN el sistema procesa la configuración de forma segura y actualiza el estatus del sistema de pagos en la base de datos.</td>
        <td>EP05</td>
    </tr>
    <td>HU19</td>
        <td>Base de datos de usuarios</td>
        <td>Como administrador, quiero implementar una base de datos segura y escalable, para proteger y gestionar eficazmente la información de los usuarios.</td>
        <td>Scenario: Acceder a datos de usuario para auditorías internas.<br>
    <br>GIVEN que el administrador necesita verificar la integridad de los datos de los usuarios,<br>
    <br>WHEN realiza una consulta en la base de datos,<br>
    <br>THEN la base de datos valida los permisos del administrador,<br>
    <br>AND proporciona los datos solicitados de manera rápida y segura.</td>
        <td>EP05</td>
    </tr>
    <td>HU20</td>
        <td>API para gestión de perfiles</td>
        <td>Como desarrollador, quiero APIs robustas para crear, editar y eliminar perfiles de usuario.</td>
        <td>Scenario: Un desarrollador necesita actualizar información de un perfil por motivos de seguridad.<br><br>GIVEN que un desarrollador necesita actualizar la información de un perfil de usuario,<br><br>WHEN el administrador modifica y guarda los cambios en el perfil,<br><br>AND el administrador confirma la operación,<br><br>THEN la API actualiza los datos en la base de datos,<br><br>AND notifica al administrador que la actualización fue exitosa.
    </td>
        <td>EP06</td>
    </tr>
    <td>HU21</td>
        <td>Logging de Actividades</td>
        <td>Como administrador, quiero un sistema de logging robusto para registrar la actividad en la plataforma, facilitando la auditoría y la detección temprana de problemas.</td>
        <td>Scenario: Registrar una actividad crítica para la auditoría de seguridad.<br><br>GIVEN el administrador lleva a cabo una acción crítica en la plataforma,<br><br>WHEN la acción es ejecutada,<br><br>THEN el sistema registra detalladamente la acción en los logs de seguridad,<br><br>AND notifica a los administradores de seguridad sobre la actividad registrada.</td>
        <td>EP05</td>
    </tr>
    <td>HU22</td>
        <td>API para búsqueda por filtros</td>
        <td>Como desarrollador, quiero crear una API para búsquedas por filtros, para mejorar la accesibilidad de la información.</td>
        <td>Scenario: Administrar búsquedas avanzadas para encontrar registros específicos de usuarios.<br>
    <br>GIVEN que el administrador necesita encontrar perfiles específicos basados en criterios complejos,<br>
    <br>WHEN utiliza la API de búsqueda por filtros en la interfaz de administración,<br>
    <br>THEN la API proporciona resultados precisos y rápidos, ayudando al administrador a gestionar eficientemente la información.</td>
        <td>EP06</td>
    </tr>
    <td>HU23</td>
        <td>Servicio de notificaciones</td>
        <td>Como desarrollador, quiero implementar un servicio de notificaciones, para mantener a los usuarios informados.</td>
        <td>Scenario: Notificar a los usuarios sobre una actualización de seguridad importante.<br><br>GIVEN que un desarrollador ha emitido una actualización de seguridad,<br><br>WHEN el sistema procesa la actualización,<br><br>AND identifica los usuarios afectados,<br><br>THEN el servicio de notificaciones envía automáticamente alertas,<br><br>AND los usuarios reciben las notificaciones en tiempo real.</td>
        <td>EP06</td>
    </tr>
    <td>HU24</td>
        <td>Soporte para múltiples navegadores</td>
        <td>Como desarrollador, quiero garantizar la compatibilidad en múltiples navegadores, para una experiencia de usuario uniforme.</td>
        <td>Scenario: Verificar y asegurar la compatibilidad de la plataforma en diferentes navegadores.<br><br>GIVEN que un desarrollador necesita asegurar que los administradores y usuarios acceden a la plataforma desde diversos navegadores,<br><br>WHEN navegan y realizan operaciones críticas,<br><br>THEN el sistema mantiene una funcionalidad consistente y segura, sin importar el navegador utilizado.</td>
        <td>EP06</td>
    </tr>
        <tr>
<td>HU25</td>
    <td>Configuración de la base de datos</td>
    <td>Como desarrollador, quiero diseñar y configurar la estructura de la base de datos para almacenar la información de los abogados, incluyendo campos como nombre, especialidad y ubicación.</td>
    <td>Scenario: Configuración de la base de datos<br><br>GIVEN el desarrollador quiere configurar la base de datos para almacenar la información de los abogados<br><br>WHEN define la estructura de la tabla 'abogados' con los campos requeridos como nombre, especialidad y ubicación,<br><br>THEN la base de datos está configurada correctamente para almacenar la información de los abogados.</td>
    <td>EP06</td>
  </tr>
  <tr>
    <td>HU26</td>
    <td>Implementación de la funcionalidad de búsqueda de abogados</td>
    <td>Como desarrollador, quiero agregar una función de búsqueda en la página de lista de abogados para que los usuarios puedan buscar abogados por nombre o especialidad.</td>
    <td>Scenario: Búsqueda de abogados<br><br>GIVEN el desarrollador quiere implementar la función de búsqueda de abogados en la aplicación,<br><br>WHEN desarrolla la función de búsqueda en la página de lista de abogados y configura los parámetros para buscar por nombre o especialidad,<br><br>THEN la búsqueda de abogados muestra resultados relevantes que coinciden con el término de búsqueda proporcionado.</td>
    <td>EP06</td>
  </tr>
    <tr>
    <td>HU27</td>
    <td>Creación y Gestión de la Entidad de Abogados</td>
    <td>Como desarrollador backend, quiero implementar la creación y gestión de la entidad de abogados en la base de datos para almacenar información detallada de los abogados.</td>
    <td>Scenario: Creación de Perfiles de Abogados<br><br>GIVEN el desarrollador quiere registrar nuevos abogados para almacenarlos en la base de datos de la plataforma,<br><br>WHEN se realiza una solicitud para crear un nuevo perfil de abogado, proporcionando información como nombre, especialidad, ubicación y otros detalles relevantes,<br><br>THEN se crea un nuevo registro en la base de datos que contiene la información completa del abogado.<br><br>Scenario: Actualización de Perfiles de Abogados<br><br>GIVEN el desarrollador quiere actualizar la información de un abogado existente en la plataforma para gestionar su información,<br><br>WHEN se realiza una solicitud para actualizar los detalles de un abogado, proporcionando el ID único del abogado y los campos que se desean modificar,<br><br>THEN el backend actualiza los datos del abogado correspondiente en la base de datos según los campos proporcionados.</td>
    <td>EP06</td>
    </tr>
    <tr>
    <td>HU28</td>
    <td>Creación y Gestión de Entidad de Usuario Médico/Estudiante</td>
    <td>Como desarrollador, quiero crear la entidad de usuario que represente tanto a médicos como a estudiantes de medicina en la plataforma, para asegurar que todos los atributos necesarios estén disponibles para cada tipo de usuario.
</td>
    <td>Scenario: Creación de la entidad de usuario<br><br>GIVEN el desarrollador quiere representar tanto a médicos como a estudiantes de medicina en el sistema para asegurar los atributos necesarios para cada tipo de usuario,<br><br>WHEN define y crea la entidad de usuario con atributos comunes como ID, nombre, especialidad, correo electrónico, contraseña, entre otros,<br><br>THEN la entidad de usuario está disponible en el sistema para ser utilizada en otras funcionalidades de la plataforma.<br><br>Scenario: Gestión de usuarios médicos/estudiantes<br><br>GIVEN el desarrollador quiere gestionar la información de médicos y estudiantes registrados para gestionar su información,<br><br>WHEN se implementa la funcionalidad para añadir, actualizar y eliminar usuarios a través de endpoints dedicados,<br><br>THEN los administradores pueden realizar operaciones CRUD (Crear, Leer, Actualizar, Eliminar) sobre la información de médicos y estudiantes de manera eficiente y segura.</td>
    <td>EP06</td>
    </tr>
    <tr>
    <td>HU29</td>
    <td>Gestión de Suscripciones</td>
    <td>Como desarrollador, quiero implementar la gestión de suscripciones para que los usuarios puedan ver, seleccionar y administrar sus planes de suscripción en la plataforma.</td>
    <td>Scenario: Manejo de Suscripciones<br><br>GIVEN el desarrollador backend necesita implementar la gestión de suscripciones en la plataforma,<br><br>WHEN desarrolla los endpoints necesarios en la API para visualizar, seleccionar y actualizar planes de suscripción,<br><br>THEN los usuarios pueden ver su suscripción actual, seleccionar nuevos planes si es necesario, y actualizar la información de pago de forma segura y eficiente.</td>
    <td>EP06</td>
    </tr>
    </tr>
    <td>HU30</td>
    <td>Creación y Gestión de Recursos Educativos</td>
    <td>Como desarrollador backend, quiero implementar la creación y gestión de recursos educativos en la base de datos para que los administradores puedan añadir, actualizar y eliminar recursos.</td>
    <td>Scenario: Creación de recursos educativos.
    <br><br>GIVEN el desarrollador necesita añadir un nuevo recurso educativo,
    <br><br>WHEN el desarrollador envía los detalles del recurso a través del endpoint de creación,
    <br><br>THEN el recurso educativo se almacena correctamente en la base de datos.
    <br><br>Scenario: Eliminación de recursos educativos
    <br><br>GIVEN el desarrollador necesita eliminar un recurso educativo,
    <br><br>WHEN el desarrollador envía una solicitud de eliminación a través del endpoint correspondiente,
    <br><br>THEN el recurso educativo se elimina correctamente de la base de datos.</td>
    <td>EP06</td>
    </tr>
</table>
    

