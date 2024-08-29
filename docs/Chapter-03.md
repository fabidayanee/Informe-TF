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
        <td>Registro de abogados especializados</td>
        <td>Como abogado, quiero registrarme en la plataforma para ofrecer mis servicios en casos de derecho médico.</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>EP02</td>
        <td>Búsqueda de abogados por especialidad médica</td>
        <td>Como médico, quiero buscar abogados especializados en el campo médico relacionado con mi caso para obtener la mejor representación.</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>EP03</td>
        <td>Solicitud de representación legal</td>
        <td>Como médico, quiero enviar una solicitud de representación a un abogado especializado para recibir asistencia en mi caso legal.</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>EP04</td>
        <td>Gestión de casos legales</td>
        <td>Como abogado, quiero gestionar mis casos asignados, incluyendo la actualización de avances y documentación, para llevar un control eficiente del proceso legal.</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
    <tr>
        <td>EP05</td>
        <td>Evaluación de casos médicos</td>
        <td>Descripción: Como abogado, quiero evaluar los detalles iniciales del caso proporcionado por el médico para determinar si puedo tomar el caso.</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>EP06</td>
        <td>Notificaciones automáticas de actualizaciones del caso</td>
        <td>Como médico, quiero recibir notificaciones automáticas sobre el progreso de mi caso para estar informado en todo momento.</td>
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
        <td>EP01</td>
    </tr>
    <tr>
        <td>HU03</td>
        <td>Subida de un caso médico</td>
        <td>Como médico quiero subir mi caso relacionado con una posible negligencia médica en la plataforma para que los abogados puedan verlo.</td>
        <td>Scenario: Subida de un caso médico<br><br>GIVEN que el médico ha iniciado sesión en la plataforma,<br><br>WHEN completa el formulario para subir un caso médico,<br><br>AND adjunta la documentación necesaria,<br><br>THEN el caso debe ser publicado en la plataforma y visible para los abogados especializados.</td>
        <td>EP02</td>
    </tr>
    <tr>
        <td>HU04</td>
        <td>Evaluación de casos por parte de los abogados</td>
        <td>Como abogado quiero evaluar casos médicos publicados en la plataforma para decidir si deseo tomar el caso.</td>
        <td>Scenario: Evaluación de casos médicos<br>
        <br>GIVEN que el abogado tiene acceso a su panel de control,<br>
        <br>WHEN revisa la lista de casos médicos disponibles,<br><br>AND selecciona un caso para revisar sus detalles,<br><br>THEN debe poder ver la información del caso y decidir si desea postularse para representarlo.</td>
        <td>EP03</td>
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
        <td>EP04</td>
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
        <td>EP04</td>
    </tr>
    

