

# Sistema de Gestión de Pedidos y Ruteo de Reparto (SGPRR) - CIMES

> **Trabajo Práctico Integrador y Progresivo (TPI) - Entrega Consolidada N° 4**  
> **Carrera:** Tecnicatura Universitaria en Programación a Distancia (TUP AD)  
> **Institución:** Universidad Tecnológica Nacional (UTN)  
> **Asignatura:** Organización Empresarial  
> **Profesor:** Regner Roberto Fabián  
> **Alumno:** Cadenini Misael  

---

## 📋 Descripción del Sistema

El **Sistema de Gestión de Pedidos y Ruteo de Reparto (SGPRR)** es una solución informática concebida para optimizar la logística operativa de la distribuidora **CIMES**. El software aborda los siguientes ejes fundamentales del negocio:

* **Toma y Procesamiento de Pedidos:** Integración multicanal (formulario web y atención automatizada mediante WhatsApp Business API).
* **Ruteo de Reparto Optimizado:** Cálculo computacional de rutas óptimas mediante APIs de geolocalización (Google Maps / OpenStreetMap) para minimizar tiempos y costos de combustible.
* **Logística Inversa de Envases:** Seguimiento en tiempo real del saldo de envases retornables (bidones de agua y sifones de soda) entregados y retirados por cliente.
* **Gestión de Stock y Depósito:** Control dinámico de inventarios de productos terminados en planta de producción.

---

## 🔗 Enlaces Rápidos del Proyecto

* **Repositorio Público GitHub:** [https://github.com/mcadenini/sgprr-cimes](https://github.com/mcadenini/sgprr-cimes)
* **Tablero de Gestión Ágil (GitHub Projects / Jira):** [https://github.com/users/mcadenini/projects/1](https://github.com/users/mcadenini/projects/1)

---

## 🎯 Historias de Usuario (Backlog Ágil)

| ID | Historia de Usuario | Prioridad | Estado |
| :--- | :--- | :--- | :--- |
| **HU-01** | **Como** Chofer de Reparto, **quiero** recibir mi hoja de ruta optimizada en la app mobile, **para** recorrer menos kilómetros y ahorrar combustible. | Alta | `Done` |
| **HU-02** | **Como** Encargado de Depósito, **quiero** visualizar el saldo de envases retornables por cliente, **para** evitar pérdidas de bidones en calle. | Media | `In Progress` |
| **HU-03** | **Como** Operador Comercial, **quiero** registrar pedidos recibidos por WhatsApp directamente en la plataforma, **para** agilizar la carga manual. | Alta | `Done` |

---

## 🛠️ Flujo de Trabajo y Versionado (Git & GitHub)

El proyecto adopta una estrategia de versionado basada en **GitFlow**:

* `main`: Rama protegida destinada únicamente a entregas estables y producción final.
* `develop`: Rama de integración continua de características en desarrollo.
* `feature/*`: Ramas secundarias utilizadas para cada incremento funcional.

### Historial de Ramas y Convención de Commits
* `feature/foda-gantt`: Diagnóstico estratégico y planificación temporal.
* `feature/organigrama-dd`: Estructuración organizacional y Diccionario de Datos.
* `feature/bpmn-flow`: Diagramación y mapeo de procesos de negocio.
* `feature/agile-backlog`: Configuración del tablero e Historias de Usuario.

#### Convención de commits (Conventional Commits):
* `feat(bpmn): agregar compuertas logicas de excepcion`
* `docs(readme): consolidar entregas 1 a 3 en archivo principal`
* `fix(schema): ajustar tipos de datos en la entidad RUTA_DE_REPARTO`

---

## ⚙️ Indicadores de Control y Auditoría Técnica (KPIs)

1. **Tiempo Medio de Respuesta (TMR):** Cálculo de rutas para 50 pedidos diarios en un tiempo $\le 3,0$ segundos.
2. **Tasa de Retorno de Envases (TRE):** Ratios de recuperación de envases vacíos per cápita $\ge 95\%$.
3. **Efectividad en Primera Visita (EEV):** Entregas concretadas exitosamente al primer intento $\ge 90\%$.

---

## 🤖 Declaración de Transparencia y Uso Crítico de IA

En cumplimiento con los requerimientos académicos de la cátedra de **Organización Empresarial (UTN)**, se declara que se utilizaron asistentes de Inteligencia Artificial Generativa (*ChatGPT / Gemini / Claude*) bajo los siguientes parámetros de supervisión humana:

1. **Modelado de Procesos (BPMN):** Se utilizaron asistentes de IA para proponer la estructura base de *Pools* y *Lanes*. Las compuertas lógicas de decisión vinculadas a la logística inversa de envases y clientes ausentes fueron modificadas y corregidas manualmente según el modelo operativo real de CIMES.
2. **Diseño de Datos:** La IA colaboró en la selección de convenciones de nomenclaturas para bases de datos relacionales, realizándose ajustes humanos en los tipos de datos exactos (`Timestamp`, `Float`, `FK/PK`).
3. **Auditoría:** La veracidad, coherencia conceptual y adecuación de todo el contenido fueron revisadas e integradas bajo la responsabilidad directa del alumno.
