# 🗒️ Registro de Trabajo en Clase - Taller 7

## 📆 Fecha de la sesión

**16 de mayo de 2026**

---

## 👥 Integrantes presentes

- Rita Trindade da Cruz
- Brandon Merchan
- Daniel forero

---

## 🧠 Actividades realizadas en clase

Durante la sesión de clase se trabajó sobre el caso base de referencia **FarmApp**, una cadena nacional de farmacias con puntos físicos y plataforma de e-commerce. El objetivo principal fue integrar las vistas arquitectónicas desarrolladas en el curso: negocio, información, aplicaciones, infraestructura y seguridad.

El equipo discutió cómo una compra digital de medicamentos no es únicamente una transacción comercial, sino un proceso completo que conecta clientes, productos, inventario, pagos, prescripciones, despacho, CRM, sistemas POS, infraestructura cloud y controles de seguridad. A partir de esta discusión, se decidió organizar el modelo alrededor del flujo principal de valor:

**Consulta de disponibilidad → compra online → validación de prescripción → pago digital → despacho → rastreo → fidelización**

### Decisiones de modelado tomadas

- Se decidió usar una estructura por **capas arquitectónicas**, para mostrar claramente la relación entre negocio, información, aplicaciones, infraestructura y seguridad.
- La **vista de negocio** se organizó alrededor de los procesos más importantes: compra, prescripción, despacho, rastreo y promociones.
- La **vista de información** incluyó las entidades principales: cliente, producto, pedido, pago, prescripción, inventario y descuento.
- La **vista de aplicaciones** integró los sistemas internos y externos: app móvil, plataforma e-commerce, POS, CRM, inventario, logística y pasarela de pagos.
- La **vista de infraestructura** incluyó nube híbrida, servidores regionales, base de datos replicada, API Gateway, broker de eventos y monitoreo.
- La **vista de seguridad** se modeló como una capa transversal, porque protege todo el flujo y no solamente un sistema específico.
- Se decidió representar relaciones verticales entre capas para evidenciar cómo un proceso de negocio depende de datos, aplicaciones, infraestructura y controles.

### Herramientas utilizadas

- **draw.io / diagrams.net**, para construir el tablero visual digital.
- Discusión grupal para identificar relaciones entre capas.
- Boceto conceptual por capas antes de construir el diagrama final.
- Documentación del taller en formato Markdown.

### Parte del trabajo desarrollada en clase

Durante la clase se alcanzó a desarrollar:

- Identificación de las vistas arquitectónicas del caso FarmApp.
- Definición del flujo principal de negocio.
- Selección de entidades de información relevantes.
- Relación entre aplicaciones internas y externas.
- Propuesta inicial de infraestructura.
- Identificación de controles de seguridad transversales.
- Primer boceto del tablero integrado en draw.io.

---

## 🧩 Boceto inicial del modelo

> Archivo asociado al boceto/modelo digital: **tablero-farmapp.drawio**

El boceto inicial fue organizado como un tablero por capas. En la parte superior se ubicaron los objetivos de negocio de FarmApp, como servicio omnicanal, disponibilidad de inventario, trazabilidad de pedidos, pagos digitales y protección de datos personales.

Debajo se ubicaron las cinco vistas principales:

1. **Negocio:** procesos de compra, prescripción y despacho.
2. **Información:** entidades como cliente, producto, pedido, pago, inventario y descuento.
3. **Aplicaciones:** app móvil, plataforma e-commerce, POS, CRM, inventario, logística y pasarela de pagos.
4. **Infraestructura:** nube híbrida, servidores regionales, API Gateway, base de datos replicada, broker de eventos y monitoreo.
5. **Seguridad:** control de acceso por rol, cifrado, auditoría, monitoreo de fraude y cumplimiento.

El modelo permite visualizar que FarmApp necesita una arquitectura integrada para operar de forma consistente entre canales físicos y digitales.

---

## 🔁 Tareas definidas para complementar el taller

| Tarea asignada | Responsable | Fecha estimada |
|----------------|-------------|----------------|
| Ajustar el tablero final en draw.io | Nombre 1 | 17/05/2026 |
| Completar el informe técnico del taller | Nombre 2 | 17/05/2026 |
| Revisar relaciones entre negocio, datos y aplicaciones | Nombre 3 | 17/05/2026 |
| Complementar la investigación con referentes como TOGAF, ArchiMate y C4 | Nombre 4 | 18/05/2026 |
| Revisar ortografía, formato y coherencia final de la entrega | Todo el equipo | 18/05/2026 |

---

## 🧠 Conclusión de la sesión

La sesión permitió comprender que una arquitectura empresarial no debe analizarse por componentes aislados, sino como un sistema integrado. En FarmApp, cada proceso de negocio depende de información confiable, aplicaciones conectadas, infraestructura disponible y controles de seguridad adecuados.

El tablero propuesto ayuda a explicar cómo la plataforma de e-commerce, los puntos físicos, el inventario, el CRM, los pagos y la logística deben trabajar juntos para ofrecer una experiencia segura, trazable y consistente al cliente.

---

_Este documento resume el trabajo colaborativo realizado durante la sesión del Taller 7 en el curso AREM - Arquitectura Empresarial - Universidad de La Sabana._
