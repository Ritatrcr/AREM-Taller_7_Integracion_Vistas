# 🛠️ Taller 7 - Integración de Vistas de Arquitectura Empresarial

## 📌 Descripción general

Este repositorio/documentación corresponde al **Taller 7 de Arquitectura Empresarial**, cuyo objetivo fue integrar diferentes vistas arquitectónicas en una narrativa visual coherente. El taller se desarrolló en dos momentos:

1. **Trabajo en clase con el caso base FarmApp**, una cadena de farmacias con e-commerce integrado.
2. **Aplicación al cliente real Elite Airsoft**, una empresa de entretenimiento táctico que necesita fortalecer su operación, reservas, trazabilidad, seguridad e infraestructura para crecer de forma controlada.

El propósito principal del taller fue demostrar cómo las vistas de **negocio, información, aplicaciones, infraestructura y seguridad** se conectan entre sí para soportar los objetivos del cliente y mejorar la toma de decisiones.

---

## 🎯 Objetivo del taller

Integrar las vistas arquitectónicas desarrolladas durante el curso en un modelo visual y documental que permita entender:

- Qué procesos generan valor para el negocio.
- Qué información es necesaria para operar y tomar decisiones.
- Qué aplicaciones soportan los procesos.
- Qué infraestructura permite disponibilidad, escalabilidad y continuidad.
- Qué controles de seguridad y gobierno protegen la operación.

---

# Parte 1 - Caso base de referencia: FarmApp

## 🧪 Contexto del caso

**FarmApp** es una cadena nacional de farmacias que combina puntos físicos con una plataforma de e-commerce. La empresa permite a sus clientes:

- Consultar disponibilidad de medicamentos.
- Realizar pedidos por app o web.
- Validar prescripciones cuando aplica.
- Hacer pagos digitales.
- Recibir recomendaciones y promociones personalizadas.
- Rastrear entregas.
- Sincronizar inventario, POS, CRM y logística.

Este caso fue trabajado durante la clase como ejercicio base para comprender cómo se integran las vistas arquitectónicas en una empresa con operación física y digital.

---

## 🧩 Vistas integradas en FarmApp

### 1. Vista de negocio

Representa los procesos principales del servicio:

- Consulta de disponibilidad.
- Compra online.
- Validación de prescripción.
- Pago digital.
- Despacho y rastreo.
- Fidelización y promociones.

### 2. Vista de información

Incluye las entidades necesarias para operar:

- Cliente.
- Producto.
- Inventario.
- Pedido.
- Prescripción.
- Pago.
- Descuento o promoción.

### 3. Vista de aplicaciones

Representa los sistemas que ejecutan el proceso:

- App móvil.
- Plataforma e-commerce.
- Sistema POS.
- CRM.
- Sistema de inventario.
- Sistema logístico.
- Pasarela de pagos.

### 4. Vista de infraestructura

Define la base tecnológica:

- Nube híbrida.
- Servidores regionales.
- API Gateway.
- Base de datos replicada.
- Broker de eventos.
- Monitoreo y observabilidad.

### 5. Vista de seguridad

Protege transversalmente el modelo:

- Control de acceso por rol.
- Cifrado de datos personales.
- Auditoría.
- Monitoreo de fraude.
- Cumplimiento y privacidad.
- Alertas operativas.

---

## 📄 Archivos de la Parte 1

| Archivo | Descripción |
|--------|-------------|
| `registro_trabajo_clase_taller7_farmapp.md` | Registro del trabajo realizado durante la sesión de clase. |
| `tablero-farmapp.drawio` | Tablero visual con la integración de vistas arquitectónicas del caso FarmApp. |

---

# Parte 2 - Aplicación al cliente real: Elite Airsoft

## 🧪 Contexto del cliente

**Elite Airsoft** es una empresa de entretenimiento táctico que ofrece experiencias de juego tipo airsoft. Su operación incluye reservas, atención a clientes, pagos, consentimientos, organización de partidas, control de asistencia y gestión operativa en campo.

Durante el análisis se identificó que el negocio está creciendo más rápido que su infraestructura operativa. El reto no consiste únicamente en recibir más reservas, sino en **controlar mejor una operación que está aumentando en volumen, complejidad y riesgo**.

---

## 🚨 Problema principal identificado

Elite Airsoft presenta una operación con alto componente manual y disperso:

- Reservas gestionadas por canales como WhatsApp, redes sociales o llamadas.
- Validación manual de pagos.
- Baja trazabilidad sobre cambios, asistencia y consentimientos.
- Dependencia de operadores específicos.
- Información distribuida en múltiples canales.
- Dificultad para consolidar datos de clientes y reportes.
- Riesgos normativos por tratamiento de datos personales y consentimientos.
- Escalabilidad limitada si aumenta la cantidad de reservas o sedes.

---

## 💡 Propuesta arquitectónica para Elite Airsoft

La solución propuesta consiste en una arquitectura integrada para digitalizar y controlar el proceso crítico:

**Reserva digital → pago → consentimiento → check-in → operación en campo → cierre → fidelización**

La arquitectura busca que Elite Airsoft pase de una operación manual y reactiva a una operación:

- Centralizada.
- Trazable.
- Segura.
- Escalable.
- Medible.
- Preparada para decisiones basadas en datos.

---

## 🧩 Vistas integradas en Elite Airsoft

### 1. Vista de negocio

Define el flujo que genera valor:

- Captación digital.
- Reserva de partida.
- Validación de pago.
- Consentimiento y datos.
- Check-in operativo.
- Operación en campo.
- Cierre y fidelización.

Esta vista responde a la pregunta:  
**¿Qué proceso debe controlar Elite Airsoft para crecer ordenadamente?**

---

### 2. Vista de información

Define los datos que sostienen la operación:

- Cliente o jugador.
- Reserva.
- Pago.
- Consentimiento.
- Inventario operativo.
- Evento o asistencia.
- Indicadores de negocio.

Esta vista responde a la pregunta:  
**¿Qué información necesita Elite Airsoft para operar con trazabilidad?**

---

### 3. Vista de aplicaciones

Define los sistemas necesarios:

- Web/App de reservas.
- Panel administrativo.
- Pasarela de pagos.
- Gestor documental de consentimientos.
- Módulo de inventario operativo.
- Check-in QR.
- CRM y BI.

Esta vista responde a la pregunta:  
**¿Qué aplicaciones permiten automatizar y controlar el proceso?**

---

### 4. Vista de infraestructura

Define la base técnica:

- Frontend cloud.
- Backend/API.
- Base de datos.
- Storage seguro.
- Webhooks o cola de eventos.
- Logs y monitoreo.
- Backups y recuperación.

Esta vista responde a la pregunta:  
**¿Dónde corre la solución y cómo puede escalar?**

---

### 5. Vista de seguridad y gobierno

Define los controles transversales:

- RBAC y perfiles de usuario.
- Cifrado y privacidad.
- Auditoría.
- Trazabilidad normativa.
- Conciliación antifraude.
- Gestión de incidentes.
- Continuidad operativa.

Esta vista responde a la pregunta:  
**¿Cómo se protege, audita y gobierna la operación?**

---

## 📄 Archivos de la Parte 2

| Archivo | Descripción |
|--------|-------------|
| `tablero-elite-airsoft-paleta-elite.drawio` | Tablero visual final de Elite Airsoft con paleta táctica alineada a la identidad visual del cliente. |
| `parte2_elite_airsoft_integracion.md` | Documento de integración de vistas para el cliente real. |
| `informe_tecnico_taller7_elite_airsoft.md` | Informe técnico completo del taller aplicado a Elite Airsoft. |
| `referencias_bibliograficas_taller7_elite_airsoft.md` | Referencias bibliográficas y técnicas utilizadas. |

---

# 🧠 Decisiones clave del taller

## Decisiones para FarmApp

- Se organizó el modelo por capas arquitectónicas.
- Se tomó como flujo principal la compra digital de medicamentos.
- Se conectaron procesos de negocio con entidades de información.
- Se identificaron aplicaciones internas y externas necesarias.
- Se representó seguridad como una capa transversal.

## Decisiones para Elite Airsoft

- Se definió la **reserva** como entidad núcleo de la operación.
- Se priorizó la digitalización de reservas, pagos y consentimientos.
- Se propuso separar el canal del cliente, el panel administrativo y la capa de datos.
- Se incluyó check-in QR para mejorar trazabilidad en campo.
- Se incorporó seguridad desde el inicio, no como una fase posterior.
- Se propuso una infraestructura cloud gradual, evitando sobredimensionar la solución.
- Se incluyeron dashboards para habilitar decisiones basadas en datos.

---

# 🧩 Comparación entre FarmApp y Elite Airsoft

| Aspecto | FarmApp | Elite Airsoft |
|--------|---------|---------------|
| Tipo de negocio | Farmacias con e-commerce | Entretenimiento táctico / experiencias |
| Proceso crítico | Compra y despacho de medicamentos | Reserva y operación de partidas |
| Canal principal | App/web + puntos físicos | Web/app + canales digitales |
| Información clave | Producto, cliente, pedido, pago, prescripción | Cliente, reserva, pago, consentimiento, evento |
| Riesgo principal | Datos personales, pagos, prescripciones | Datos personales, consentimientos, pagos, operación en campo |
| Aplicaciones clave | E-commerce, POS, CRM, inventario, logística | Reservas, panel admin, pagos, consentimientos, check-in QR |
| Infraestructura | Nube híbrida, BD replicada, servidores regionales | Cloud gradual, API, BD, storage, monitoreo, backups |
| Seguridad | RBAC, cifrado, fraude, privacidad | RBAC, auditoría, consentimiento, antifraude, continuidad |

---

# 🗂️ Estructura recomendada del repositorio

```text
Taller-7-Integracion-Vistas/
│
├── README.md
│
├── farmapp/
│   ├── registro_trabajo_clase_taller7_farmapp.md
│   └── tablero-farmapp.drawio
│
├── elite-airsoft/
│   ├── tablero-elite-airsoft-paleta-elite.drawio
│   ├── parte2_elite_airsoft_integracion.md
│   ├── informe_tecnico_taller7_elite_airsoft.md
│   └── referencias_bibliograficas_taller7_elite_airsoft.md
│
└── anexos/
    └── capturas-diagramas/
```

---

# 🛠️ Cómo usar los archivos

## Abrir los diagramas `.drawio`

1. Ingresar a [diagrams.net](https://www.diagrams.net/).
2. Seleccionar **File → Open From → Device**.
3. Cargar el archivo `.drawio`.
4. Revisar o editar el tablero.
5. Exportar como imagen o PDF si se requiere para la entrega.

## Editar los documentos `.md`

Los archivos Markdown pueden abrirse con:

- Visual Studio Code.
- GitHub.
- Typora.
- Obsidian.
- Cualquier editor de texto.

También pueden convertirse a PDF si el docente solicita entrega en formato formal.

---

# 📈 Valor del taller

Este taller permite demostrar que una arquitectura empresarial no es solamente un diagrama técnico. Es una forma de explicar cómo la tecnología, los datos, los procesos y la seguridad se conectan para lograr objetivos de negocio.

En el caso de **FarmApp**, la arquitectura permite entender la integración entre comercio digital, farmacias físicas, inventario, CRM, pagos y logística.

En el caso de **Elite Airsoft**, la arquitectura permite visualizar cómo el negocio puede pasar de una operación manual a una operación digital, trazable y preparada para escalar.

---

# 🔍 Referentes utilizados

Para el desarrollo del taller se tomaron como referencia marcos y buenas prácticas de arquitectura empresarial, modelado, seguridad e infraestructura:

- TOGAF.
- ArchiMate.
- C4 Model.
- BPMN.
- AWS Well-Architected Framework.
- OWASP Top 10.
- ISO/IEC 27001.
- Ley 1581 de 2012 sobre protección de datos personales en Colombia.
- Decreto 1377 de 2013.
- Modelo de Seguridad y Privacidad de la Información de MinTIC.

---

# ✅ Conclusión

El Taller 7 permitió integrar diferentes vistas arquitectónicas en dos escenarios: un caso académico base y un cliente real. La comparación entre FarmApp y Elite Airsoft demuestra que, aunque los negocios son distintos, ambos necesitan una arquitectura coherente donde los procesos, los datos, las aplicaciones, la infraestructura y la seguridad trabajen de forma articulada.

Para **Elite Airsoft**, la arquitectura propuesta representa una ruta clara hacia una operación más profesional, segura y escalable. El modelo no se limita a implementar tecnología, sino que busca resolver problemas reales del negocio: falta de trazabilidad, alta manualidad, validación dispersa de pagos, gestión informal de consentimientos y poca capacidad para tomar decisiones con datos.

---

_Este README hace parte de la entrega académica del Taller 7 del curso AREM - Arquitectura Empresarial - Universidad de La Sabana._
