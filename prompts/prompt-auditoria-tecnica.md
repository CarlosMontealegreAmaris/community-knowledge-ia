@project
# 🛡️ Modo Auditoría Técnica - Copilot Agent

## 🎯 Objetivo
Realizar una auditoría exhaustiva del estado actual del proyecto, analizando todas las clases, módulos y componentes del código fuente. El agente debe actuar como auditor técnico experto en arquitectura de software, buenas prácticas y mantenibilidad.

## 📂 Ubicación
Este archivo debe estar ubicado en `.github/audit.md`.

## 🧠 Instrucciones para el Agente

1. **Activar modo auditoría técnica.**
2. **Analizar profundamente el código fuente del proyecto.**
3. **No realizar ningun cambio en el codigo**
4. **Generar un informe detallado con los siguientes criterios:**

---

### 🔍 Evaluacion de patrones de diseño
- **Criterio:**
Validar cuales son necesarios y no se estan aplicando, omitir los que no apliquen al proyecto.
- **Creacionales:** 
Singleton – Garantiza que una clase tenga una única instancia y proporciona un punto de acceso global.
Factory Method – Define una interfaz para crear un objeto, pero permite que las subclases decidan qué clase instanciar.
Abstract Factory – Proporciona una interfaz para crear familias de objetos relacionados sin especificar sus clases concretas.
Builder – Separa la construcción de un objeto complejo de su representación, permitiendo crear diferentes representaciones.
Prototype – Permite copiar objetos existentes sin hacer el código dependiente de sus clases.
- **Estructurales:** 
Adapter – Permite que interfaces incompatibles trabajen juntas.
Bridge – Separa una abstracción de su implementación para que ambas puedan variar independientemente.
Composite – Compone objetos en estructuras de árbol para representar jerarquías parte-todo.
Decorator – Añade responsabilidades a un objeto dinámicamente.
Facade – Proporciona una interfaz simplificada a un conjunto de interfaces en un subsistema.
Flyweight – Usa el almacenamiento compartido para soportar grandes cantidades de objetos de forma eficiente.
Proxy – Proporciona un sustituto o marcador de posición para otro objeto para controlar el acceso a él.
- **Comportamiento:** 
Chain of Responsibility – Permite que varios objetos tengan la oportunidad de manejar una solicitud.
Command – Encapsula una solicitud como un objeto, permitiendo parametrizar clientes con diferentes solicitudes.
Interpreter – Define una representación para una gramática y un intérprete que usa esa representación.
Iterator – Proporciona una forma de acceder secuencialmente a los elementos de una colección sin exponer su representación interna.
Mediator – Define un objeto que encapsula cómo interactúan un conjunto de objetos.
Memento – Permite capturar y restaurar el estado interno de un objeto sin violar su encapsulamiento.
Observer – Define una dependencia uno-a-muchos entre objetos para que cuando uno cambie, todos sus dependientes sean notificados.
State – Permite a un objeto alterar su comportamiento cuando su estado interno cambia.
Strategy – Define una familia de algoritmos, encapsula cada uno y los hace intercambiables.
Template Method – Define el esqueleto de un algoritmo en una operación, dejando algunos pasos a las subclases.
Visitor – Permite definir nuevas operaciones sobre una estructura de objetos sin cambiar las clases de los objetos.

### 🔍 Criterios de Auditoría

- **Antipatrones detectados:** resumen de porcentaje actual de antipatrones presentes en el codigo basados en:
God Object / God Class
Una clase que hace demasiado, concentra demasiadas responsabilidades y viola el principio de responsabilidad única.
Spaghetti Code
Código desorganizado, sin estructura clara, difícil de leer y mantener. Suele tener muchas dependencias cruzadas y poca modularidad.
Lava Flow
Código obsoleto o sin uso que permanece en el sistema por miedo a eliminarlo. Nadie sabe si es necesario, pero nadie se atreve a tocarlo.
Golden Hammer
Uso excesivo de una única solución o tecnología para todos los problemas, incluso cuando no es adecuada.
Cut-and-Paste Programming
Reutilización de código mediante copia directa, lo que genera duplicación y dificulta el mantenimiento.
Poltergeist
Clases que solo existen para pasar datos entre otras clases, sin lógica propia. Suele ocurrir con controladores o servicios mal diseñados.
Boat Anchor
Componentes o librerías que ya no se usan pero siguen en el proyecto, generando peso innecesario y posibles vulnerabilidades.
Dead Code
Código que nunca se ejecuta o que no tiene efecto, pero sigue presente en el repositorio.
Hard Coding
Valores fijos en el código (como rutas, credenciales, configuraciones), lo que dificulta la escalabilidad y la seguridad.
Magic Numbers / Strings
Uso de números o cadenas sin contexto ni explicación, en lugar de constantes con nombres significativos.
Uso excesivo de IF
resuelven toda la logica con declaraciones if
- **Acoplamiento de adaptadores:** Calcular el porcentaje de acoplamento que tienen los adaptadores.
- **Control de excepciones:** Calcular el porcentaje de flujos que controlan sus propias excepciones con onerrorresume o otros controladores de error.
- **Observacion:** Calcular el porcentaje de flujos que tienen observacion una libreria de logs.
- **Código que requiere ajustes:** Estimar el porcentaje de código que no sigue buenas prácticas.
- **Arquitectura:** Revisar las tecnologias y calular el porcentaje de aplicabilidad de arquiectura
- **Estimación de esfuerzo:** Calcular el tiempo aproximado necesario para resolver vulnerabilidades y refactorizar el código.
- **Riesgos por versiones obsoletas:** Identificar librerías con versiones antiguas y sus riesgos asociados.
- **Cumplimiento con reglas de Sonar:** Estimar el porcentaje de código que cumple con reglas de calidad de SonarQube.
- **Mantenibilidad actual:** Calcular el índice de mantenibilidad basandose en el analisis previos de malas practicas y antipatrones.
- **Pruebas unitarias:** Analizar la cobertura real de pruebas unitarias del proyecto, calcular el porcentaje de cobertura, agregar a los tiempos el esfuerzo de llegar al ochenta porciento de cobertura.

---

### 📤 Resultado Esperado

El agente debe generar un informe en formato Markdown dentro de `.github/audit-report.md` con:
- Gráficos o tablas si es necesario.
- Recomendaciones específicas por módulo.
- Priorización de problemas críticos.
- Ser critico con el proyecto que se revisa
- Tomarse el tiempo necesario para generar la auditoria, no dar respuestas rapidas
- Resaltar la importancia de las pruebas unitarias