# 📄 Informe Técnico del Taller

## 🔖 Nombre del Taller

**Taller 7 - Integración de Vistas de Arquitectura Empresarial**

---

## 👥 Integrantes del equipo

- Nombre 1 (correo o usuario GitHub)
- Nombre 2
- Nombre 3
- Nombre 4

---

## 🧠 Descripción general del trabajo

El objetivo de este taller fue integrar las diferentes vistas arquitectónicas desarrolladas durante el curso en una narrativa visual coherente para el cliente real **Elite Airsoft**. La integración permitió conectar la vista de negocio, información, aplicaciones, infraestructura y seguridad en un solo modelo, mostrando cómo cada capa soporta el proceso crítico de la empresa: **la gestión de reservas y operación de eventos de airsoft**.

Elite Airsoft actualmente depende en gran parte de procesos manuales para gestionar reservas, pagos, consentimientos, disponibilidad de horarios, comunicación con clientes y control operativo. Por esta razón, el modelo propuesto busca representar una arquitectura futura más trazable, segura, escalable y centralizada, donde la operación no dependa únicamente de conversaciones dispersas o validaciones manuales, sino de una plataforma digital que permita tomar decisiones con datos y reducir riesgos operativos.

La actividad se desarrolló articulando los entregables previos del curso: análisis de procesos, diagnóstico AS-IS, propuesta TO-BE, brechas de infraestructura, seguridad, normativa y arquitectura de solución. El resultado final es un tablero visual que explica cómo la transformación digital de Elite Airsoft puede conectar la experiencia del cliente con la gestión interna, la infraestructura tecnológica y los controles de seguridad.

---

## 🔧 Proceso de desarrollo

El trabajo se realizó tomando como punto de partida el proceso más crítico de Elite Airsoft: **la reserva de experiencias de juego**. Este proceso fue seleccionado porque concentra varios problemas del negocio: atención manual, baja trazabilidad, manejo disperso de información, validación manual de pagos, dificultad para gestionar consentimientos, dependencia de operadores específicos y ausencia de una visión centralizada de la operación.

Primero se modeló la **vista de negocio**, identificando las etapas principales del servicio: solicitud de reserva, validación de disponibilidad, confirmación del pago, firma de consentimiento, check-in del jugador, ejecución de la experiencia, cierre del evento y fidelización del cliente. Esta vista permitió entender qué necesita controlar la empresa para operar con mayor eficiencia.

Después se construyó la **vista de información**, donde se definieron las entidades necesarias para soportar el proceso: cliente, reserva, pago, consentimiento, evento, horario, sede, inventario operativo, promociones e historial de participación. Esta capa es clave porque convierte una operación manual en una operación medible y auditable.

Posteriormente se integró la **vista de aplicaciones**, proponiendo componentes como una página web de reservas, un panel administrativo, un módulo de pagos, un módulo de consentimientos digitales, un CRM básico, un sistema de notificaciones y un dashboard gerencial. Estas aplicaciones permiten automatizar tareas que actualmente dependen de mensajes, hojas de cálculo o revisión manual.

Luego se modeló la **vista de infraestructura**, considerando una arquitectura simple pero escalable: hosting cloud, base de datos centralizada, almacenamiento de documentos, servicios de autenticación, backups, monitoreo y conexión segura desde dispositivos administrativos. La infraestructura fue pensada para una empresa en crecimiento, evitando una solución sobredimensionada, pero dejando una ruta clara hacia mayor escalabilidad.

Finalmente se integró la **vista de seguridad y gobierno**, incluyendo controles de acceso por rol, protección de datos personales, trazabilidad de acciones, control de consentimientos, respaldo de información, monitoreo de pagos y políticas mínimas de operación. Esta capa se ubicó como transversal, porque no debe funcionar como un componente aislado, sino como una condición permanente para operar de forma confiable.

Las herramientas utilizadas fueron:

- **draw.io / diagrams.net**, para construir el tablero visual integrado.
- **Markdown**, para documentar el informe técnico.
- Referentes de arquitectura empresarial y software como **TOGAF**, **ArchiMate**, **C4 Model** y **AWS Well-Architected Framework**.
- Entregables previos del curso sobre procesos, seguridad, normativa, infraestructura y propuesta de solución para Elite Airsoft.

---

## 🧩 Análisis del modelo propuesto

### Cómo se estructura el modelo entregado

El modelo se estructura en cinco vistas arquitectónicas conectadas entre sí:

1. **Vista de negocio:** muestra los procesos centrales de Elite Airsoft, principalmente la reserva y operación del evento.
2. **Vista de información:** identifica los datos que deben capturarse, protegerse y utilizarse para operar mejor.
3. **Vista de aplicaciones:** presenta los sistemas que automatizan o soportan la operación.
4. **Vista de infraestructura:** representa la base tecnológica necesaria para que los sistemas funcionen de forma disponible y segura.
5. **Vista de seguridad y gobierno:** define los controles transversales que reducen riesgos, mejoran la trazabilidad y permiten cumplir obligaciones relacionadas con datos personales y consentimiento.

La lógica del modelo es descendente y transversal. La capa de negocio define qué necesita la empresa; la capa de información define qué datos se requieren; la capa de aplicaciones ejecuta los procesos; la infraestructura permite la operación técnica; y la seguridad protege todo el flujo.

---

### Cómo representa las necesidades del cliente

El modelo representa las necesidades reales de Elite Airsoft porque no se limita a proponer “más tecnología”, sino que conecta la tecnología con problemas concretos del negocio:

- La necesidad de **automatizar reservas** se responde con una página web/app y un panel administrativo.
- La necesidad de **reducir errores humanos** se responde con flujos digitales, validaciones y registros centralizados.
- La necesidad de **controlar pagos** se responde con integración a pasarela de pagos y conciliación de transacciones.
- La necesidad de **gestionar consentimientos** se responde con un módulo digital de aceptación, almacenamiento y consulta.
- La necesidad de **mejorar la trazabilidad** se responde con auditoría, logs y estados de reserva.
- La necesidad de **crecer de forma ordenada** se responde con infraestructura cloud, base de datos centralizada y dashboards gerenciales.
- La necesidad de **mejorar seguridad y normativa** se responde con roles, permisos, cifrado, backups y políticas de tratamiento de datos.

Desde una perspectiva de negocio, la arquitectura permite que Elite Airsoft pase de una operación reactiva y manual a una operación más controlada, medible y preparada para escalar. Desde una perspectiva técnica, la propuesta crea una base para integrar aplicaciones, datos e infraestructura sin depender de herramientas aisladas.

---

### Qué supuestos se tomaron

Para construir el modelo se tomaron los siguientes supuestos:

- Elite Airsoft recibe reservas por canales digitales como WhatsApp, redes sociales o llamadas.
- La validación de pagos se realiza en gran parte de forma manual.
- La empresa necesita registrar datos personales de clientes y, en algunos casos, información de acudientes o consentimientos.
- Existen horarios, cupos, sedes, instructores o recursos operativos que deben coordinarse.
- Actualmente no existe una plataforma totalmente centralizada para controlar reservas, pagos, consentimientos y reportes.
- La solución debe ser gradual, porque la empresa no necesariamente necesita una infraestructura compleja desde el primer momento.
- El negocio requiere una arquitectura que combine facilidad de uso, bajo costo inicial, seguridad y posibilidad de crecimiento.

---

## 📈 Diagrama final entregado

> Archivo asociado al modelo visual: **tablero-elite-airsoft.drawio**

El diagrama final representa la integración de las vistas arquitectónicas de Elite Airsoft. El proceso central del tablero es:

**Reserva digital → pago → consentimiento → check-in → operación del evento → cierre → fidelización**

Alrededor de este flujo se conectan las entidades de información, los módulos de aplicación, la infraestructura técnica y los controles de seguridad. El objetivo del diagrama es mostrar que la transformación digital no depende de un único sistema, sino de la articulación entre procesos, datos, tecnología y gobierno.

---

## 📋 Tabla de actores, entidades o componentes

| Nombre del elemento | Tipo | Descripción | Responsable |
|---------------------|------|-------------|-------------|
| Cliente / jugador | Actor | Persona que consulta disponibilidad, realiza una reserva y participa en la experiencia de juego. | Cliente |
| Acudiente | Actor | Responsable que autoriza la participación de un menor cuando aplique. | Cliente / Operación |
| Operador de reservas | Actor | Persona encargada de revisar solicitudes, validar información y apoyar la confirmación de reservas. | Elite Airsoft |
| Administrador | Actor | Usuario interno que supervisa reservas, pagos, reportes, horarios y configuración del sistema. | Elite Airsoft |
| Monitor / instructor | Actor | Persona que acompaña la experiencia en campo y verifica asistencia, seguridad operativa y ejecución del evento. | Elite Airsoft |
| Reserva | Entidad de información | Registro que contiene fecha, hora, número de jugadores, estado, canal y datos del cliente. | Sistema de reservas |
| Pago | Entidad de información | Registro de la transacción realizada por el cliente y su estado de validación. | Pasarela de pagos / Administración |
| Consentimiento | Entidad de información | Documento o aceptación digital asociada al cliente y a la actividad. | Sistema de consentimientos |
| Cliente | Entidad de información | Datos básicos del jugador, historial de reservas y preferencias comerciales. | CRM / Administración |
| Evento | Entidad de información | Actividad programada con fecha, cupo, sede, recursos y responsable operativo. | Operación |
| Inventario operativo | Entidad de información | Recursos necesarios para ejecutar la experiencia, como equipos, elementos de protección o disponibilidad logística. | Operación |
| Página web de reservas | Aplicación | Canal digital para consultar disponibilidad, registrar datos y solicitar una reserva. | Equipo técnico / Elite Airsoft |
| Panel administrativo | Aplicación | Herramienta interna para gestionar reservas, pagos, consentimientos, horarios y reportes. | Administración |
| Módulo de pagos | Aplicación | Componente que permite recibir y validar pagos electrónicos de forma trazable. | Pasarela de pagos / Sistema |
| Módulo de consentimientos | Aplicación | Componente que permite aceptar, almacenar y consultar consentimientos digitales. | Sistema / Administración |
| CRM básico | Aplicación | Sistema para consolidar clientes, historial de compras, segmentación y campañas. | Administración / Marketing |
| Dashboard gerencial | Aplicación | Vista de indicadores para analizar ventas, ocupación, reservas, asistencia y crecimiento. | Gerencia |
| Base de datos centralizada | Infraestructura | Repositorio principal donde se almacenan reservas, clientes, pagos, eventos y consentimientos. | Equipo técnico |
| Hosting cloud | Infraestructura | Entorno donde se despliega la aplicación web, panel y servicios asociados. | Equipo técnico |
| Almacenamiento documental | Infraestructura | Servicio para guardar consentimientos, soportes y documentos asociados a la operación. | Equipo técnico |
| Backups | Infraestructura | Copias de seguridad periódicas para recuperación ante pérdida de información. | Equipo técnico |
| Control de acceso por rol | Seguridad | Define qué puede ver o modificar cada usuario según su responsabilidad. | Administración / Equipo técnico |
| Auditoría de acciones | Seguridad | Registro de cambios relevantes en reservas, pagos, consentimientos y usuarios. | Sistema |
| Protección de datos personales | Seguridad / Normativa | Medidas para proteger información de clientes, contactos, acudientes y registros operativos. | Elite Airsoft |
| Monitoreo operativo | Seguridad / Operación | Seguimiento de disponibilidad, errores, pagos pendientes y eventos críticos. | Administración / Equipo técnico |

---

## 🔍 Investigación complementaria

### Tema investigado

**Buenas prácticas de documentación de arquitectura empresarial y software aplicadas a una empresa de servicios experienciales como Elite Airsoft.**

### Resumen

Para documentar la arquitectura de Elite Airsoft se tomaron como referencia enfoques ampliamente usados en arquitectura empresarial y arquitectura de software. **TOGAF** plantea que la arquitectura debe construirse considerando los intereses de distintos stakeholders y organizando la información en vistas que permitan entender la empresa desde varias perspectivas: negocio, datos, aplicaciones y tecnología. Esta idea se relaciona directamente con el taller porque Elite Airsoft no necesita solamente un diagrama técnico, sino una representación que conecte decisiones de negocio, operación diaria, seguridad, infraestructura y crecimiento.

También se revisó **ArchiMate**, un lenguaje de modelado empresarial que permite representar relaciones entre dominios como negocio, aplicaciones y tecnología. Su valor para este caso está en que ayuda a evitar que las capas se vean como elementos aislados. En Elite Airsoft, por ejemplo, una reserva no es solo una acción comercial: genera datos, activa aplicaciones, requiere infraestructura, necesita controles de seguridad y produce información útil para la gerencia.

Como complemento, se consideró el **C4 Model**, que permite explicar arquitectura de software por niveles de detalle: contexto, contenedores, componentes y código. Para este taller, el enfoque C4 ayuda a presentar la solución de forma entendible para públicos técnicos y no técnicos. A nivel de negocio, se puede explicar el sistema como una plataforma de reservas y operación; a nivel técnico, se puede descomponer en aplicación web, panel administrativo, base de datos, pasarela de pagos, módulo de consentimientos y servicios de notificación.

Finalmente, se revisó el enfoque de **AWS Well-Architected Framework**, especialmente por sus pilares de excelencia operativa, seguridad, fiabilidad, eficiencia, optimización de costos y sostenibilidad. Aunque Elite Airsoft no requiere una arquitectura empresarial compleja desde el inicio, estos pilares sirven como guía para proponer una solución realista: segura, disponible, monitoreable, de costo controlado y preparada para crecer.

---

## 🧠 Decisiones clave del modelo

| Decisión | Justificación técnica | Justificación de negocio |
|---------|------------------------|---------------------------|
| Centralizar reservas en una plataforma digital | Permite manejar estados, disponibilidad, pagos y registros desde una misma base de datos. | Reduce errores, mejora tiempos de respuesta y evita pérdida de información. |
| Incluir consentimientos digitales | Permite almacenar evidencia trazable y consultar documentos cuando sea necesario. | Disminuye riesgos normativos y mejora la confianza del cliente. |
| Usar control de acceso por rol | Limita acciones según perfil: administrador, operador, monitor o gerencia. | Reduce manipulación indebida de información y mejora la gobernabilidad. |
| Integrar pagos electrónicos | Permite registrar transacciones y estados de pago automáticamente. | Reduce validaciones manuales y mejora el control financiero. |
| Implementar dashboard gerencial | Consolida datos operativos en indicadores. | Permite tomar decisiones sobre horarios, demanda, promociones y crecimiento. |
| Usar infraestructura cloud escalable | Facilita despliegue, backups, monitoreo y crecimiento gradual. | Evita inversiones iniciales excesivas y permite crecer por etapas. |
| Registrar auditoría de acciones | Permite saber quién hizo cambios y cuándo. | Mejora trazabilidad y control interno. |

---

## 🧩 Reflexión crítica sobre la coherencia de la arquitectura

La arquitectura propuesta es coherente porque parte de una necesidad real del negocio y no de una solución tecnológica aislada. El problema principal de Elite Airsoft no es únicamente “no tener una página web”, sino operar con poca trazabilidad, alta dependencia manual y baja centralización de información. Por eso, la solución integra procesos, datos, aplicaciones, infraestructura y seguridad.

Una fortaleza del modelo es que permite explicar la transformación digital de Elite Airsoft en lenguaje técnico y de negocio. Para la gerencia, el valor está en mejorar control, ventas, experiencia del cliente y toma de decisiones. Para el equipo operativo, el valor está en reducir tareas manuales y tener información clara. Para el equipo técnico, el valor está en contar con una arquitectura modular que puede crecer sin rehacer todo desde cero.

La principal precaución es no intentar implementar toda la arquitectura al mismo tiempo. La solución debe ejecutarse por fases: primero reservas, pagos y consentimientos; luego dashboard, CRM y automatización avanzada; finalmente analítica, campañas y escalabilidad multi-sede. Si la implementación se hace de forma gradual, la arquitectura mantiene coherencia con la capacidad operativa y financiera de la empresa.

En conclusión, el modelo propuesto articula correctamente las vistas arquitectónicas porque cada capa responde a una necesidad específica y, al mismo tiempo, todas se conectan alrededor del proceso crítico de reservas. Esto permite que Elite Airsoft avance hacia una operación más segura, medible, profesional y escalable.

---

## 📚 Referencias

- [1] The Open Group. *TOGAF Standard*. https://www.opengroup.org/togaf
- [2] The Open Group. *ArchiMate Enterprise Architecture Modeling Language*. https://www.opengroup.org/archimate-forum/archimate-overview
- [3] Brown, Simon. *The C4 Model for Visualising Software Architecture*. https://c4model.com/
- [4] Amazon Web Services. *AWS Well-Architected Framework*. https://aws.amazon.com/architecture/well-architected/
- [5] Amazon Web Services. *Operational Excellence Pillar - AWS Well-Architected Framework*. https://docs.aws.amazon.com/wellarchitected/latest/operational-excellence-pillar/welcome.html
- [6] Object Management Group. *Business Process Model and Notation BPMN*. https://www.omg.org/spec/BPMN/

---

_Este documento hace parte de la entrega del Taller 7 del curso AREM (Arquitectura Empresarial) - Universidad de La Sabana._
