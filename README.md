1. Definición del Problema
En el ámbito de los servicios de salud pública, la gestión eficiente de los turnos asignados a los pacientes representa un desafío fundamental. Para las obras sociales, esta tarea se vuelve aún más crucial, ya que deben lidiar con una demanda constante y una población diversa que requiere atención médica.
El problema que enfrentan las obras sociales radica en la complejidad inherente al proceso de asignación y administración de turnos. A menudo, los pacientes se enfrentan a largos tiempos de espera, cancelaciones de último momento y una falta de transparencia en la programación, lo que genera frustración y dificulta el acceso a los servicios de salud.
Esta situación genera una serie de desafíos que deben ser abordados de manera integral. Por un lado, la necesidad de optimizar el flujo de pacientes y minimizar los tiempos de espera, a fin de garantizar una atención médica eficiente y oportuna. Por otro lado, la implementación de herramientas y procesos que permitan una mayor transparencia y comunicación entre los pacientes y la obra social, fomentando así la confianza y la satisfacción de los usuarios.
Para hacer frente a esta problemática, se hace necesario el desarrollo de un sistema de gestión de turnos que ofrezca soluciones integrales. Este mismo debe estar diseñado para automatizar y agilizar el proceso de asignación de turnos, minimizando los tiempos de espera y permitiendo una programación más flexible y adaptable a las necesidades de los pacientes.
Asimismo, el sistema de gestión de turnos debe integrar funcionalidades que faciliten la comunicación y el seguimiento de los procesos, brindando a los pacientes una mayor visibilidad sobre el estado de sus solicitudes y el desarrollo de sus atenciones médicas. De esta manera, se fomentará la transparencia y se fortalecerá la confianza entre los usuarios y la obra social.
En conclusión, la definición del problema de la gestión de turnos para obras sociales radica en la necesidad de implementar un sistema integral que optimice los procesos, mejore la comunicación y brinde una experiencia más satisfactoria para los pacientes. La adopción de este tipo de soluciones permitirá a las obras sociales mejorar la eficiencia de sus servicios, aumentar la satisfacción de los usuarios y contribuir a la mejora de la salud pública en su conjunto.




2. Objetivo
Desarrollar un sistema de gestión de turnos que permita a los pacientes y al personal de las obra sociales, clínicas, sanatorios,etc gestionar y visualizar los turnos de manera eficiente. El sistema debe reducir la carga administrativa, minimizar errores y mejorar la experiencia general tanto para los pacientes como para el personal de salud.
3. Alcance
El sistema abarcará:
    • Gestión de Turnos: Registro y asignación de turnos para pacientes y personal.
    • Visualización de Turnos: Acceso a un calendario o vista de agenda para verificar horarios y disponibilidad.
    • Notificaciones: Alertas y recordatorios para pacientes y personal sobre turnos y cambios.
    • Especialidades:  Generar las distintas especialidades de los profesionales.
El sistema no incluirá la gestión de otros aspectos administrativos como la facturación o la gestión de inventario.
4. Descripción del Sistema
Requisitos Funcionales
    1. Registro de Pacientes y Personal:
        ◦ Registro de datos básicos (nombre, contacto, tipo de usuario).
        ◦ Asignación de roles y permisos según el tipo de usuario (paciente, médico,).
    2. Gestión de Turnos:
        ◦ Creación, modificación y cancelación de turnos.
        ◦ Asignación automática o manual de turnos.
        ◦ Control de disponibilidad de horarios.
    3. Visualización de Turnos:
        ◦ Calendario interactivo para ver la disponibilidad de turnos.
        ◦ Filtros para buscar y visualizar turnos específicos.
    4. Notificaciones y Recordatorios:
        ◦ Envío de recordatorios por correo electrónico y mensajes SMS.
        ◦ Notificaciones de cambios o cancelaciones.
Requisitos del Hardware
    • Administrador:
        ◦ Procesador de al menos 4 núcleos.
        ◦ Memoria RAM de 16 GB.
        ◦ Espacio en disco de 100 GB (SSD recomendado).
    • Usuarios:
        ◦ Ordenadores o dispositivos móviles con acceso a Internet.
        ◦ Navegador web moderno (Chrome, Firefox, Edge).
Arquitectura
La arquitectura MVC separa la lógica de la aplicación en tres componentes interconectados: Modelo, Vista y Controlador. Esta separación permite una mejor organización del código, facilita el mantenimiento y permite la reutilización de componentes. 
    1. Componentes.
 Modelo:
        ◦ Representa los datos y la lógica de negocio de la aplicación. 
        ◦ Gestiona el acceso a la información, define las reglas de negocio y procesa los datos. 
        ◦ Componentes principales: 
            ▪ Entidades: Pacientes, Médicos, turnos.
            ▪ Servicios: Lógica de negocio para cada entidad. 
            ▪ Repositorios: Acceso a la base de datos. 
2.2 Vista 
        ◦ Presenta la información al usuario. 
        ◦ Interfaces de usuario para diferentes roles (médicos, enfermeras, administrativos, etc.). 
        ◦ Implementado con tecnologías web responsivas (HTML, CSS). 
        ◦ Componentes principales: 
            ▪ Plantillas: Estructuras base para las páginas. 
            ▪ Componentes: Elementos reutilizables de la interfaz (formularios, tablas, gráficos). 
            ▪ Páginas: Vistas específicas para cada funcionalidad. 
2.3 Controlador 
        ◦ Actúa como intermediario entre el Modelo y la Vista. 
        ◦ Procesa las solicitudes del usuario, interactúa con el Modelo y selecciona la Vista apropiada. 
        ◦ Componentes principales: 
            ▪ Controladores: Uno por cada entidad principal (Home
            ▪ Login,Especialidad,Medico,Paciente,Turno). 
            ▪ Middleware: Para autenticación, logging, manejo de errores, etc. 
            ▪ Rutas: Definen cómo se mapean las URLs a los controladores. 
    2. Flujo de datos 
        ◦ El usuario interactúa con la Vista (por ejemplo, solicita un turno con un especialista). 
        ◦ La Vista envía el turno al Controlador. 
        ◦ El Controlador procesa la solicitud, interactúa con el Modelo para obtener los datos necesarios. 
        ◦ El Modelo recupera los datos de la base de datos y aplica la lógica de negocio. 
        ◦ El Modelo devuelve los datos procesados al Controlador. 
        ◦ El Controlador selecciona la Vista apropiada y le pasa los datos. 
        ◦ La Vista renderiza los datos y presenta la información al usuario. 

    3. Beneficios para el sistema del Cliente:

        ◦ Separación de preocupaciones: Facilita el desarrollo y mantenimiento de diferentes aspectos de la aplicación 
        ◦ Reutilización de código: Los componentes pueden ser reutilizados en diferentes partes de la misma. 
        ◦ Flexibilidad: Permite cambiar la interfaz de usuario sin afectar la lógica de negocio y viceversa. 
        ◦ Escalabilidad: Facilita la adición de nuevas funcionalidades o la modificación de las existentes. 
        ◦ Testabilidad: La separación de componentes permite realizar pruebas unitarias más fácilmente. 




Esta arquitectura MVC proporcionará una base sólida y flexible para el sistema de gestión del sistema de turnos, permitiendo un desarrollo eficiente y un mantenimiento más sencillo a largo plazo.
Historias de Usuario
Número: 1
Usuario: Paciente
Nombre de la historia: Solicitar un turno
Descripción: Como paciente quiero solicitar un turno medico para una especialidad y horario especifica.
Validación: La aplicación muestra un calendario con fechas y horarios disponibles.  El paciente puede seleccionar el turno (eligiendo fecha hora y especialidad). La aplicación verifica disponibilidad. El paciente recibe una notificación con el detalle
Numero 2:
Nombre de la historia:  Modificar un Turno
Descripción: Como paciente, quiero poder cambiar la fecha u hora de un turno programado.
Validación: La aplicación muestra las citas programadas para el paciente. El mismo puede seleccionar un turno y solicitar el cambio de fecha u hora. El sistema verifica la disponibilidad y confirma el cambio de cita.
Numero 3:
Nombre de la historia: Eliminar un turno
Descripción: Como paciente quiero cancelar un turno en caso de que no pueda asistir.
Validación:  La aplicación muestra las citas programadas para el paciente. El paciente puede seleccionar una cita y solicitar la cancelación. El sistema confirma la cancelación de la cita. 
Numero 4:
Nombre de la historia: Dar de alta un profesional
Descripción:  Como usuario administrativo, quiero poder registrar un nuevo médico en la aplicación para que pueda atender a los pacientes.
Validación: La aplicación muestra un formulario para los datos del medico. La aplicación lo valida que exista un medico registrado .
Numero 5
Nombre de la Historia: Modificar datos de un médico 
Descripción: Como usuario administrativo, quiero poder actualizar la información de un médico registrado, en caso de que sus datos cambien. 
Validación:  La aplicación muestra una lista de médicos registrados. Al seleccionar un médico, se despliega un formulario con sus datos actuales. El usuario administrativo puede editar los campos necesarios y guardar los cambios.  El sistema actualiza la información del médico en la base de datos.
Numero 6

Nombre de la historia: Registrar una nueva especialidad 

Descripción: Como usuario administrativo, quiero poder registrar una nueva especialidad médica en la aplicación , para que los pacientes puedan agendar turnos con los médicos correspondientes.

Validación: El sistema muestra un formulario para ingresar los datos de la nueva especialidad: nombre, descripción, etc.
La aplicación valida que no exista una especialidad registrada con el mismo nombre.
Al completar el registro, la nueva especialidad queda disponible para ser asignada a los médicos.
El sistema actualiza la lista de especialidades disponibles en el módulo de turnos.

Numero 7
 
Nombre de la historia: Modificar una especialidad existente 

Descripción: Como usuario administrativo, quiero poder actualizar los datos de una especialidad médica registrada, en caso de que haya cambios. 

Validación:  El sistema muestra una lista de las especialidades registradas. Al seleccionar una especialidad, se despliega un formulario con sus datos actuales. El usuario administrativo puede editar los campos necesarios y guardar los cambios. El sistema actualiza la información de la especialidad en la base de datos. La aplicación actualiza la lista de especialidad disponibles en el modulo de turnos

Numero 8

Nombre de la historia: Asignar una especialidad a un médico.

Descripción: Como usuario administrativo, quiero poder asignar una o más especialidades a un médico, para que los pacientes puedan agendar citas con él. 

Validación: La aplicación muestra una lista de los médicos registrados. Al seleccionar un médico, se despliega un formulario con sus datos y las especialidades asignadas.  El usuario administrativo puede agregar o eliminar especialidades para ese médico. La aplicación actualiza la información del médico y las especialidades asignadas y actualiza la disponibilidad del medico en el modulo de turnos.


Diseño de Interfaz Gráfica
    • Pantalla de Inicio:
        ◦ Botones para acceso de paciente, médico, especialidad y turnos.

    • Calendario de Turnos:
        ◦ Vista mensual/semanal/día con opción para agregar o modificar turnos.
        ◦ Filtros para búsqueda por fecha, tipo de servicio o personal.
    • Panel de Usuario:
        ◦ Información de perfil.
        ◦ Historial de turnos y próximos turnos.

DISEÑO DE LA BASE DE DATOS.
    • Tablas Principales:

        1. Usuarios:
            ▪ id_usuario 
            ▪ nombre
            ▪ contacto
            ▪ rol (paciente, médico,)
        2. Turnos:
            ▪ id_turno 
            ▪ id_usuario 
            ▪ fecha
            ▪ hora_inicio
            ▪ hora_fin
.
3. Medico
                    ◦ id__medico
                    ◦ nombre
                    ◦ apellido
                    ◦ Direccion
                    ◦ Telefono
                    ◦ EMAIL
                    ◦ Horario atencion desde
                    ◦ Horario atencion fin

	     4.Paciente
                    ◦ id__paciente
                    ◦ nombre
                    ◦ apellido
                    ◦ Direccion
                    ◦ Telefono
                    ◦ EMAIL

Tecnologias

Backend:

    • ASP.NET Core: Framework de desarrollo web multiplataforma utilizado para la implementación del backend de la aplicación. 
    • C#: Lenguaje de programación utilizado para el código del backend. 
    • Entity Framework Core: Framework de acceso a datos utilizado para interactuar con la base de datos. 
Frontend:
    • Razor: Motor de vistas utilizado para la creación de las interfaces de usuario. 
    • HTML: Lenguaje de marcado utilizado para la estructura de las páginas web. 
    • CSS: Hojas de estilo utilizadas para el diseño y presentación de la interfaz gráfica. 
    • JavaScript: Utilizado para agregar interactividad y funcionalidad del lado del cliente. 
    • Bootstrap: Framework CSS utilizado para facilitar el diseño responsivo y la creación de interfaces de usuario. 
    • Font Awesome: Biblioteca de iconos utilizada para mejorar la apariencia visual de la aplicación. 
    • SQL SERVER: Sistema de gestión de bases de datos relacional utilizado como motor de base de datos para esta 
