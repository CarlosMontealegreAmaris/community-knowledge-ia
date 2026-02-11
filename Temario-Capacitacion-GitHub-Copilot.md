# Capacitación GitHub Copilot
## Temario Completo

---

## 🧭 Índice

## 📚 PARTE 1: TEORÍA
- 1.1 ¿Qué es y qué NO es GitHub Copilot?
- 1.2 Modos de Interacción con GitHub Copilot
- 1.3 Tipos de Algoritmos/Modelos Disponibles
- 1.4 Beneficios y Casos de Uso Reales
- 1.5 Cómo Hacer un Buen Prompt
- 1.6 Otros Tipos de Herramientas Copilot
- 1.7 La IA como Asistente, NO como Piloto
- 1.8 Calidad, seguridad y uso responsable

## 🛠️ PARTE 2: PRÁCTICA
- 2.1–2.11 Ejercicios y flujos de trabajo

## 🎯 QUIZ - Kahoot

## 📝 Notas Finales

---

## 📚 PARTE 1: TEORÍA

### 1.1 ¿Qué es y qué NO es GitHub Copilot?

#### ¿Qué es GitHub Copilot?
- **Tecnología e ingeniería de la herramienta:**
  - Asistente de código impulsado por IA basado en modelos de lenguaje grandes (LLMs)
    - Utiliza tecnología de OpenAI (GPT-5.2) y Anthropic (Claude)
  - Entrenado con billones de líneas de código público
  - Comprende contexto del proyecto, archivos y patrones de código
  - Generación de código en tiempo real basada en lenguaje natural y código existente

#### ¿Qué NO es GitHub Copilot?
- **Mitos y malinterpretaciones:**
  - ❌ NO es un simple autocompletado de código
  - ❌ NO es un algoritmo tradicional de búsqueda y reemplazo
  - ❌ NO es una base de datos que copia código literalmente
  - ❌ NO reemplaza al desarrollador (es un asistente, no un piloto autónomo)
  - ❌ NO garantiza código 100% correcto sin revisión
  - ❌ NO funciona sin contexto ni guía apropiada

---

### 1.2 Modos de Interacción con GitHub Copilot

#### Los 4 Modos Principales:

**1. Ask (Preguntar)**
- Realizar preguntas directas sobre código, tecnologías o conceptos
- Obtener explicaciones de código existente
- Consultar mejores prácticas y patrones de diseño

**2. Agent (Agente)**
- Modo autónomo para tareas complejas
- El agente puede investigar, planificar y ejecutar múltiples pasos
- Ideal para refactorización, implementación de features completas

**3. Edit (Editar)**
- Modificación directa de código existente
- Sugerencias inline mientras escribes
- Refactorización y mejoras de código

**4. Plan (Planificar)**
- Generación de planes de implementación
- Desglose de tareas complejas en pasos
- Arquitectura y diseño de soluciones

---

### 1.3 Tipos de Algoritmos/Modelos Disponibles

#### Diferencias básicas entre modelos:

**GPT-5.2 (OpenAI)**
- Excelente comprensión de contexto y razonamiento
- Muy bueno para diseño/arquitectura, refactorizaciones y debugging complejo
- Respuestas detalladas y explicativas cuando se necesita

**Claude Sonnet 4.5 (Anthropic)**
- Muy buen equilibrio entre calidad y velocidad
- Buen seguimiento de instrucciones y consistencia en cambios
- Ideal para tareas de desarrollo diarias (features, refactors, tests)

**Claude Opus (Anthropic)**
- Enfoque en *pensamiento profundo* (razonamiento más cuidadoso y multi‑paso)
- Se usa para las tareas más retadoras: problemas ambiguos, decisiones de arquitectura, debugging difícil
- Útil cuando necesitas priorizar calidad y análisis por sobre rapidez

**Gemini 2.5 Pro (Google)**
- Fuerte en razonamiento y análisis
- Bueno para tareas complejas y generación de soluciones end‑to‑end
- Útil cuando se requiere explorar alternativas y comparar enfoques

---

### 1.4 Beneficios y Casos de Uso Reales

#### Beneficios en Productividad:
- **Ahorro de tiempo:** 30-55% más rápido en tareas de desarrollo
    - **¿De dónde sale este número?** Como referencia pública, GitHub reportó resultados de un **estudio controlado** donde desarrolladores completaron una tarea de programación **~55% más rápido** usando Copilot.
    - **Importante:** el impacto real varía según el tipo de tarea (boilerplate vs. lógica compleja), tu familiaridad con el stack, y qué tan claro es el contexto/instrucciones.
    - **Fuente oficial (GitHub):** https://github.blog/2022-09-07-research-quantifying-github-copilots-impact-on-developer-productivity-and-happiness/
- **Reducción de búsquedas:** Menos tiempo en Stack Overflow y documentación
- **Código boilerplate:** Generación automática de código repetitivo
    - **¿Qué es “boilerplate”?** Es el código “de base” que se repite mucho entre proyectos y que normalmente **no aporta lógica de negocio nueva**, pero es necesario para que todo funcione.
    - **Ejemplos típicos:** esqueletos de CRUD, DTOs/Modelos, mapeos (JSON ↔ objetos), validaciones simples, configuración de rutas/endpoints, logs, manejo de errores estándar, scaffolding de tests.
    - **Por qué ayuda:** Copilot acelera este tipo de trabajo mecánico, y tú te enfocas en requisitos, reglas de negocio y revisión de calidad.
- **Aprendizaje continuo:** Descubre nuevos patrones y técnicas

#### Casos de Uso Reales:
1. **Testing:** Generación de pruebas unitarias y casos de prueba
2. **Documentación:** Creación automática de comentarios y README
3. **Refactorización:** Modernización y optimización de código legacy
4. **APIs:** Implementación rápida de endpoints y servicios
5. **Debugging:** Identificación y corrección de errores
6. **Migración:** Conversión de código entre lenguajes/frameworks

#### Casos de uso de Agentes (en la empresa)

**🗂️ Project Management (Gestión de Proyectos)**
- Recopila actualizaciones del equipo
- Identifica hitos, dependencias y bloqueos
- Redacta reportes de avance
- **Rol típico:** TPM digital (Technical Program Manager)

**🎧 Customer Support (Soporte al Cliente)**
- Encuentra respuestas previas y casos similares
- Redacta nuevas soluciones y pasos de diagnóstico
- Resuelve consultas de forma autónoma (cuando es seguro hacerlo)
- **Rol típico:** asistente de base de conocimiento / knowledge base

**🔬 Research & Development (I+D)**
- Explora papers, patentes y documentación técnica
- Sintetiza tendencias y hallazgos clave
- Acelera fases tempranas de innovación (ideación y prototipado)
- **Rol típico:** analista técnico

**💼 Sales & Marketing (Ventas y Marketing)**
- Investiga competidores y posicionamiento
- Analiza estrategias comerciales y mensajes de mercado
- Recomienda planes de marketing y campañas
- **Rol típico:** analista de mercado

**👥 Human Resources (Recursos Humanos)**
- Redacta manuales, guías y políticas internas
- Ayuda a alinear contenidos con normativas y compliance
- Crea material de onboarding y capacitación
- **Rol típico:** asistente de talento

---

### 1.5 Cómo Hacer un Buen Prompt

#### ¿Qué es un prompt?
Un **prompt** es la **instrucción** que le das a la IA para que genere una respuesta útil (código, explicación, plan o cambios). En la práctica, es una combinación de **objetivo + contexto + requisitos + restricciones**: mientras más claro y específico sea, mejores resultados obtendrás.

#### ¿Qué idioma entiende mejor la IA?
- **Inglés:** Mayor precisión y vocabulario técnico
- **Español:** Funciona bien, especialmente en modelos recientes
- **Recomendación:** Usar términos técnicos en inglés dentro de prompts en español

#### Características de un Buen Prompt:

**✅ LO QUE DEBE TENER:**
- Contexto claro y específico
- Requisitos técnicos explícitos
- Lenguaje/framework a utilizar
- Ejemplos de entrada/salida esperados
- Restricciones o limitaciones

**❌ LO QUE NO DEBE TENER:**
- Ambigüedad o vaguedad
- Múltiples tareas no relacionadas en un mismo prompt
- Suposiciones implícitas sin contexto
- Instrucciones contradictorias

#### Ejemplos Reales:

**❌ Prompt Malo:**
```
crea una función
```

**✅ Prompt Bueno:**
```
Crea una función en TypeScript llamada 'calculateDiscount' que:
- Reciba precio original (number) y porcentaje de descuento (number)
- Valide que el descuento esté entre 0 y 100
- Retorne el precio final con descuento aplicado
- Lance una excepción si los parámetros son inválidos
- Incluya JSDoc con ejemplos de uso
```

**❌ Prompt Malo:**
```
arregla el código
```

**✅ Prompt Bueno:**
```
En el método getUserById(), corrige el siguiente problema:
- Actualmente retorna null cuando no encuentra el usuario
- Debe lanzar una excepción UserNotFoundException
- Debe loguear el intento de búsqueda antes de consultar la BD
- Mantener la firma del método sin cambios
```

---

### 1.6 Otros Tipos de Herramientas Copilot

#### GitHub Copilot CLI
- **Descripción:** Asistente de comandos en la terminal
- **Uso:** Sugerencias de comandos shell, git, npm, etc.
- **Licencia:** Incluida en GitHub Copilot Individual/Business/Enterprise
- **Instalación:** `gh extension install github/gh-copilot`

#### GitHub Copilot Chat (en IDEs)
- **Descripción:** Chat interactivo dentro del IDE
- **IDEs compatibles:** VS Code, Visual Studio, IntelliJ, Rider, etc.
- **Licencia:** GitHub Copilot Individual ($10/mes) o Business ($19/usuario/mes)
- **Características:** Chat contextual, explicación de código, generación de tests

#### Microsoft 365 Copilot
- **Descripción:** Asistente para aplicaciones Microsoft (Word, Excel, PowerPoint)
- **Diferencia:** NO es para desarrollo de software
- **Licencia:** Separada ($30/usuario/mes), requiere Microsoft 365 E3/E5
- **Uso:** Productividad en documentos, análisis de datos, presentaciones

#### Diferencias Clave:
| Herramienta | Propósito | Licencia | Contexto |
|-------------|-----------|----------|----------|
| Copilot (IDE) | Desarrollo de código | Individual/Business/Enterprise | Código fuente |
| Copilot CLI | Comandos de terminal | Incluida con Copilot | Shell/Terminal |
| Copilot Chat | Asistente conversacional | Incluida con Copilot | IDE/Código |
| M365 Copilot | Productividad Office | Separada | Documentos Office |

---

### 1.7 La IA como Asistente, NO como Piloto

#### Principios Fundamentales:

**🎯 Control y Supervisión:**
- El desarrollador SIEMPRE debe revisar el código generado
- La IA sugiere, el humano decide y valida
- No confiar ciegamente en las sugerencias

**🛡️ Responsabilidad del Desarrollador:**
- Entender el código antes de integrarlo
- Verificar seguridad y performance
- Validar cumplimiento de estándares del proyecto
- Ejecutar pruebas y code review

**⚖️ Balance Correcto:**
- ✅ Usar IA para acelerar tareas repetitivas
- ✅ Aprovechar sugerencias para aprender
- ✅ Validar y mejorar el código generado
- ❌ NO delegar decisiones de arquitectura completamente
- ❌ NO construir productos sin supervisión humana
- ❌ NO ignorar el contexto del negocio

**🎓 Mentalidad Correcta:**
> "GitHub Copilot es tu copiloto, no tu piloto. Tú sigues al mando del avión."

---

### 1.8 Calidad, seguridad y uso responsable

> Objetivo: acelerar el desarrollo sin comprometer calidad, seguridad ni privacidad.

#### Reglas del equipo (recomendadas)
- **Nunca pegues secretos en prompts:** tokens, API keys, passwords, certificados, cadenas de conexión, cookies, datos personales (PII) o información sensible del negocio.
- **Todo código generado pasa por revisión:** code review humano + pruebas antes de merge.
- **Cambios sensibles = explicación obligatoria:** si el cambio afecta autenticación, autorización, pagos, cifrado, logs, datos personales o performance crítico, pide que Copilot explique **supuestos, riesgos y trade-offs**.
- **Preferir cambios pequeños:** evita “big-bang refactors”. Itera en PRs más chicos y testeables.

#### Privacidad / Enterprise (contexto rápido)
- La política exacta depende del plan (Individual/Business/Enterprise) y la configuración de tu organización.
- Como práctica, asume que **todo lo que pegues como prompt** puede quedar registrado en herramientas internas o logs de auditoría.
- Fuente oficial: Documentación de GitHub Copilot https://docs.github.com/copilot

#### Plantillas de prompts (reutilizables y agnósticas)

**Plantilla: Refactor (seguro y por pasos)**
```
Quiero refactorizar este componente/módulo sin cambiar el comportamiento.

Contexto:
- Objetivo del módulo:
- Restricciones (performance, compatibilidad, estilo, no nuevas dependencias):

Tarea:
1) Explica los smells/problemas actuales.
2) Propón un plan en 3-5 pasos con riesgos.
3) Aplica el paso 1 con cambios mínimos.
4) Indica cómo verificar (tests/comandos) y qué casos borde revisar.

Código/archivos relevantes:
- [pegar/adjuntar]
```

**Plantilla: Tests (unit/integration/e2e)**
```
Genera pruebas para [función/clase/endpoint/flujo] con estos requisitos:
- Tipos de pruebas: unit / integration / e2e (elige las que apliquen)
- Casos: happy path + edge cases + error cases
- Datos de ejemplo y mocks/fakes cuando sea necesario
- Nombres descriptivos (Given/When/Then)
- No inventes librerías: usa el stack actual del proyecto

Contexto del comportamiento esperado:
- Entradas válidas:
- Entradas inválidas:
- Salidas/efectos:
```

**Plantilla: Debugging (hipótesis y reproducción)**
```
Tengo este bug:
- Síntoma:
- Pasos para reproducir:
- Comportamiento esperado vs actual:
- Logs/stacktrace:

Tarea:
1) Genera 3 hipótesis ordenadas por probabilidad.
2) Para cada hipótesis, dime qué evidencia buscar y cómo.
3) Propón un fix mínimo.
4) Propón tests o verificaciones para evitar regresión.

Código/archivos relevantes:
- [pegar/adjuntar]
```

---

## 🛠️ PARTE 2: PRÁCTICA

### 2.1 Cómo Usar GitHub Copilot en Diferentes Entornos

#### Visual Studio Code
**Ventajas:**
- Integración nativa y fluida
- Chat inline y panel lateral
- Soporte completo de todos los lenguajes
- Actualizaciones frecuentes

**Características exclusivas:**
- Quick Chat (Ctrl+Shift+I / Cmd+Shift+I)
- Inline suggestions automáticas
- Copilot Edits (modificación multi-archivo)

#### Visual Studio (Windows/Mac)
**Ventajas:**
- Integración profunda con .NET
- Excelente para C#, F#, VB.NET
- IntelliSense mejorado con IA

**Características exclusivas:**
- Completado de clases completas
- Sugerencias en debugger
- Integración con Azure

#### IntelliJ IDEA (y JetBrains IDEs)
**Ventajas:**
- Ideal para Java, Kotlin, Scala
- Integración con refactorización de JetBrains
- Excelente para proyectos empresariales

**Características exclusivas:**
- Sugerencias en Live Templates
- Integración con análisis de código
- Soporte para frameworks JVM

#### GitHub Copilot CLI
**Ventajas:**
- Asistencia directa en terminal
- Sugerencias de comandos complejos
- Explicación de comandos existentes

**Uso:**
```bash
# Sugerir comando
gh copilot suggest "find large files"

# Explicar comando
gh copilot explain "tar -xzvf file.tar.gz"
```

---

### 2.2 Instalación y Requisitos

#### GitHub Copilot CLI

**Requisitos previos:**
- GitHub CLI instalado (`gh`)
- Suscripción activa de GitHub Copilot

**Instalación:**
```bash
# Instalar extensión
gh extension install github/gh-copilot

# Verificar instalación
gh copilot --version

# Autenticar (si es necesario)
gh auth login
```

**Uso básico:**
```bash
# Modo sugerencia
gh copilot suggest -t shell "comprimir carpeta recursivamente"

# Modo explicación
gh copilot explain "git rebase -i HEAD~3"
```

#### Visual Studio Code

**Requisitos:**
- VS Code versión **1.74.0** o superior (recomendado: última versión)
- Node.js 16+ (para algunas extensiones)

**Instalación:**
1. Abrir VS Code
2. Ir a Extensions (Ctrl+Shift+X)
3. Buscar "GitHub Copilot"
4. Instalar "GitHub Copilot" y "GitHub Copilot Chat"
5. Reiniciar VS Code
6. Autenticar con cuenta de GitHub

**Extensiones requeridas:**
- `GitHub.copilot` (Sugerencias de código)
- `GitHub.copilot-chat` (Chat interactivo)

#### Visual Studio (Windows)

**Requisitos:**
- Visual Studio **2022 versión 17.4** o superior
- Suscripción de GitHub Copilot activa

**Instalación:**
1. Abrir Visual Studio Installer
2. Modificar instalación actual
3. En "Individual components", buscar "GitHub Copilot"
4. Marcar la casilla y modificar
5. Abrir Visual Studio
6. Tools → Options → GitHub → Copilot
7. Sign in con cuenta de GitHub

#### IntelliJ IDEA (y JetBrains)

**Requisitos:**
- IntelliJ IDEA **2023.1** o superior (todas las ediciones)
- PyCharm, WebStorm, PhpStorm, Rider: versiones 2023.1+

**Instalación:**
1. Abrir IntelliJ IDEA
2. File → Settings (Ctrl+Alt+S)
3. Plugins → Marketplace
4. Buscar "GitHub Copilot"
5. Instalar y reiniciar IDE
6. Tools → GitHub Copilot → Login to GitHub
7. Autorizar en el navegador

---

### 2.3 El Archivo `.github/copilot-instructions.md`

#### ¿Qué es?
Un archivo de configuración que define reglas, estándares y contexto específico del proyecto para GitHub Copilot.

#### ¿Para qué sirve?
- Establecer convenciones de código del proyecto
- Definir arquitectura y patrones a seguir
- Especificar tecnologías y versiones utilizadas
- Configurar reglas de negocio específicas
- Crear comandos personalizados reutilizables

#### ¿Qué se puede poner ahí?

**Estructura recomendada:**
```markdown
# Instrucciones para GitHub Copilot

## Contexto del Proyecto
[Descripción del proyecto, tecnologías, arquitectura]

## Estándares de Código
[Convenciones de nomenclatura, formato, estructura]

## Tecnologías y Versiones
[Stack tecnológico específico]

## Reglas de Negocio
[Lógica específica del dominio]

## Comandos Personalizados
[Atajos y comandos con slash /]

## Restricciones
[Lo que NO se debe hacer]
```

#### Beneficios de tenerlo configurado:
- ✅ **Consistencia:** Todo el equipo recibe sugerencias alineadas
- ✅ **Contexto automático:** Copilot entiende el proyecto sin repetir instrucciones
- ✅ **Productividad:** Reduce tiempo explicando el mismo contexto
- ✅ **Calidad:** Código generado cumple estándares del proyecto
- ✅ **Onboarding:** Nuevos desarrolladores reciben guía automática

#### ¿Cómo GitHub Copilot entiende estas instrucciones?
- El archivo se lee automáticamente en cada interacción
- Funciona como contexto permanente en el chat y sugerencias
- Se combina con el contexto del archivo actual
- Las reglas se aplican a todas las sugerencias de código

#### Ejemplo real:
```markdown
# Instrucciones para GitHub Copilot

## Contexto del Proyecto
Este es un proyecto Spring Boot 3.2 con Java 17.
Arquitectura hexagonal con DDD.
Base de datos PostgreSQL 15.

## Estándares de Código
- Usar Lombok para reducir boilerplate
- Nombres de variables en camelCase
- Nombres de clases en PascalCase
- Máximo 500 líneas por archivo
- Máximo 120 caracteres por línea
- Siempre usar Optional en lugar de null

## Testing
- JUnit 5 para pruebas unitarias
- Mockito para mocks
- TestContainers para pruebas de integración
- Cobertura mínima: 80%

## Restricciones
- NO usar @Autowired en campos, usar constructor injection
- NO usar tipos raw de colecciones
- NO usar System.out.println, usar logger
```

---

### 2.4 Crear Agente Personalizado Reutilizable

#### ¿Qué es un Agente Personalizado?
Un agente con instrucciones predefinidas que puede ser reutilizado en múltiples proyectos sin necesidad de configurar `copilot-instructions.md` en cada repositorio.

#### ¿Cómo crearlo?

**Opción 1: Archivo de Instrucciones Global**

Crear archivo en directorio del usuario:
- **Windows:** `%USERPROFILE%\.github\copilot-instructions.md`
- **macOS/Linux:** `~/.github/copilot-instructions.md`

**Opción 2: Configuración en VS Code**

```json
// settings.json
{
  "github.copilot.advanced": {
    "customInstructions": "Eres un experto en desarrollo backend con Spring Boot..."
  }
}
```

#### Ejemplo de Agente Reutilizable:

**Archivo:** `.github/copilot-global-instructions.md`
```markdown
# Agente de Desarrollo Backend

## Perfil del Agente
Experto en desarrollo backend, arquitectura limpia, y mejores prácticas.

## Reglas Generales
1. Siempre priorizar legibilidad sobre brevedad
2. Seguir principios SOLID
3. Aplicar patrones de diseño cuando sea apropiado
4. Escribir código autodocumentado
5. Incluir manejo de errores robusto

## Testing
- Aplicar TDD cuando sea posible
- Cobertura mínima del 80%
- Tests unitarios descriptivos con Given-When-Then
- Mocks solo cuando sea necesario

## Documentación
- JavaDoc/JSDoc para APIs públicas
- README actualizado con cada feature
- Changelog con formato estándar

## Seguridad
- Validar todas las entradas
- Sanitizar outputs
- Usar prepared statements
- Nunca hardcodear credenciales
```

#### Ventajas:
- ✅ No repetir configuración en cada proyecto
- ✅ Consistencia entre todos tus proyectos
- ✅ Fácil de actualizar y mantener
- ✅ Compartible con el equipo vía Git

---

### 2.5 Archivo CHANGELOG.md

#### ¿Qué es un CHANGELOG?
Documento que registra todos los cambios notables realizados en un proyecto de forma cronológica.

#### ¿Para qué sirve?
- Historial de cambios del proyecto
- Documentación de decisiones técnicas
- Trazabilidad de bugs y features
- Comunicación con el equipo
- Referencia para code reviews

#### ¿Por qué es bueno tener una bitácora de cambios?
- 📝 **Transparencia:** Todo el equipo sabe qué cambió y por qué
- 🔍 **Debugging:** Identificar cuándo se introdujo un bug
- 📊 **Métricas:** Analizar velocidad de desarrollo
- 🎯 **Contexto:** Entender decisiones pasadas
- 🤝 **Colaboración:** Facilita el trabajo en equipo

#### Formato Recomendado:

```markdown
# Changelog

Todos los cambios notables en este proyecto serán documentados en este archivo.

El formato está basado en [Keep a Changelog](https://keepachangelog.com/es-ES/1.0.0/),
y este proyecto adhiere a [Semantic Versioning](https://semver.org/lang/es/).

## [Unreleased]

### Added
- Nueva funcionalidad de notificaciones push

### Changed
- Optimización de consultas a base de datos

### Fixed
- Corrección de bug en autenticación OAuth

## [1.2.0] - 2025-11-06

### Motivo
Simplificar la configuración de SonarQube para solucionar problemas de reconocimiento de cobertura y generalizar la detección de reportes de cobertura.

### Archivos afectados
- `sonar-project.properties`
- `build config` (configuración de cobertura)
- `README.md` (actualización de documentación)

### Added
- Configuración automática de paths de cobertura
- Soporte para múltiples módulos

### Changed
- Ruta de reportes de cobertura de específica a pattern
- Actualización de versión de SonarQube Scanner a 4.8

### Fixed
- Problema de detección de cobertura en builds CI/CD
- Warnings de propiedades deprecadas

## [1.1.0] - 2025-10-15

### Motivo
Implementar sistema de caché para mejorar performance de APIs.

### Archivos afectados
- `src/main/java/config/CacheConfig.java` (nuevo)
- `src/main/java/service/UserService.java`
- `src/main/java/service/ProductService.java`

### Added
- Implementación de Redis como caché distribuido
- Anotaciones @Cacheable en servicios críticos
- Configuración de TTL por tipo de dato

### Performance
- Reducción de 60% en tiempo de respuesta de endpoint /api/users
- Disminución de carga en base de datos en 40%

## [1.0.0] - 2025-09-01

### Motivo
Lanzamiento inicial del sistema de gestión de inventario.

### Added
- CRUD completo de productos
- Sistema de autenticación con JWT
- APIs RESTful documentadas con Swagger
- Tests unitarios con 85% de cobertura
- CI/CD con GitHub Actions
```

#### Estructura de una Entrada:

```markdown
## [Versión] - Fecha

### Motivo
[Por qué se hizo este cambio]

### Archivos afectados
- `ruta/archivo1.java`
- `ruta/archivo2.ts`

### Added (Agregado)
- Nuevas características

### Changed (Cambiado)
- Cambios en funcionalidad existente

### Deprecated (Deprecado)
- Características que serán removidas

### Removed (Removido)
- Características eliminadas

### Fixed (Corregido)
- Bugs solucionados

### Security (Seguridad)
- Vulnerabilidades corregidas
```

#### Cómo usar GitHub Copilot para mantener el CHANGELOG:

```
Prompt: "Actualiza el CHANGELOG.md con los cambios de este commit:
- Agregué validación de email en UserController
- Corregí bug de timezone en reportes
- Actualicé dependencia de Spring Boot a 3.2.1"
```

---

### 2.6 Modos y Símbolos de Contexto

#### Símbolos de Contexto en GitHub Copilot Chat:

#### `@workspace`
**Descripción:** Contexto de TODO el workspace/proyecto
**Uso:**
```
@workspace ¿Dónde está definida la clase UserService?
@workspace explica la arquitectura del proyecto
@workspace encuentra todos los endpoints REST
```

#### `@project`
**Descripción:** Contexto del proyecto actual (si hay múltiples)
**Uso:**
```
@project ¿qué patrones de diseño estamos usando?
@project lista todos los servicios disponibles
```

#### `#file` o `#`
**Descripción:** Referencia a un archivo específico
**Uso:**
```
Explica el código de #UserController.java
¿Qué hace la función main en #app.ts?
Refactoriza #legacy-service.py para usar async/await
```

#### `/` (Comandos Slash)
**Descripción:** Comandos predefinidos para tareas comunes
**Comandos disponibles:**
- `/explain` - Explica código seleccionado
- `/fix` - Corrige problemas en código
- `/tests` - Genera pruebas unitarias
- `/help` - Muestra ayuda
- `/clear` - Limpia el chat

**Uso:**
```
/explain
[selecciona código]

/tests
Genera tests para esta función con casos edge

/fix
El error está en la línea 45
```

#### Selección de Código (Highlighting)
**Descripción:** Resaltar código en el editor para darlo como contexto
**Cómo usar:**
1. Selecciona el código en el editor
2. Abre Copilot Chat
3. Haz tu pregunta (el código seleccionado se incluye automáticamente)

**Ejemplos:**
```
[Seleccionar función completa]
"¿Cómo puedo optimizar esta función?"

[Seleccionar bloque try-catch]
"Mejora el manejo de errores aquí"

[Seleccionar clase completa]
"/tests genera tests unitarios completos"
```

#### `@file` (Cargar archivo directamente)
**Descripción:** Carga contenido de archivo específico
**Uso:**
```
@file:src/config/database.js ¿cuál es la configuración de conexión?
@file:README.md resume el proyecto
```

#### Combinaciones Poderosas:

```
@workspace #UserService.java encuentra todos los lugares donde se usa
```

```
@project /tests para las clases en el paquete com.example.service
```

```
[Seleccionar código] /explain en español y con diagramas
```

#### Ejemplo Práctico Completo:

```
Pregunta: @workspace tenemos un problema de performance en 
#OrderService.java línea 145. Analiza el método calculateTotal() 
y sugiere optimizaciones considerando que la base de datos 
está en #database-config.yml
```

---

### 2.7 Comandos Personalizados en `copilot-instructions.md`

#### ¿Para qué sirven los comandos personalizados?
- Automatizar tareas repetitivas con un solo comando
- Estandarizar procesos del equipo
- Ahorrar tiempo al no repetir las mismas instrucciones
- Asegurar consistencia en refactorizaciones

#### ¿Cómo definir un comando?

**Sintaxis en `.github/copilot-instructions.md`:**
```markdown
## Comandos Personalizados

### /ajustar-estilo
Cuando se detecte un comentario que diga "Ajustar estilo de codigo", hacer:
- Identar correctamente el código
- Eliminar imports no usados
- Ajustar espacios en blanco innecesarios
- Asegurar que las líneas no excedan 120 caracteres
- Simplificar el código cuando sea posible
- Advertir si se superan las 500 líneas de código en un solo archivo

### /crear-test
Cuando se solicite "/crear-test", generar:
- Prueba unitaria con JUnit 5
- Usar @DisplayName descriptivo
- Incluir casos: happy path, edge cases, error cases
- Mocks con Mockito cuando sea necesario
- Assertions con AssertJ
- Cobertura del 100% del método

### /documentar
Cuando se pida "/documentar", añadir:
- JavaDoc completo con @param, @return, @throws
- Ejemplos de uso en el JavaDoc
- Comentarios inline solo si el código no es autoexplicativo
- Actualizar README.md si es un cambio significativo

### /review
Cuando se solicite "/review", analizar:
- Cumplimiento de principios SOLID
- Posibles bugs o edge cases no manejados
- Performance y optimizaciones
- Seguridad (inyección, validación, etc.)
- Legibilidad y mantenibilidad
- Sugerencias de refactoring

### /commit-msg
Cuando se pida "/commit-msg", generar mensaje de commit:
- Formato: tipo(alcance): descripción
- Tipos: feat, fix, docs, style, refactor, test, chore
- Descripción en español, imperativo, max 72 caracteres
- Incluir breaking changes si aplica
```

#### Ejemplo de Uso:

**Escenario 1: Ajustar estilo**
```java
// Código mal formateado
public class UserService{
private UserRepository userRepository;
public User findById(Long id){return userRepository.findById(id).orElseThrow(()->new NotFoundException("User not found"));}
}
```

**Comando en Copilot Chat:**
```
Ajustar estilo de codigo
```

**Resultado:**
```java
public class UserService {
    private UserRepository userRepository;
    
    public User findById(Long id) {
        return userRepository.findById(id)
            .orElseThrow(() -> new NotFoundException("User not found"));
    }
}
```

**Escenario 2: Crear tests**
```
/crear-test para el método calculateDiscount en ProductService
```

**Resultado (ejemplo corto):**
```java
@DisplayName("ProductService - calculateDiscount")
class ProductServiceTest {

    @Test
    void shouldCalculateDiscount() {
        // Given: price=100, discount=20
        // When: result = calculateDiscount(price, discount)
        // Then: result == 80
    }

    @Test
    void shouldRejectInvalidDiscount() {
        // Given: discount fuera de rango (ej: 150)
        // When/Then: lanza excepción
    }
}
```

**Idea clave:** en un proyecto real agregarías más casos (0%, 100%, negativos, redondeo, nulls, etc.), pero el patrón Given/When/Then se mantiene.

#### Beneficios de los Comandos Personalizados:

✅ **Ahorro de tiempo:** Un comando vs. explicar el mismo proceso cada vez
✅ **Consistencia:** Todos en el equipo usan las mismas reglas
✅ **Calidad:** Se siguen estándares automáticamente
✅ **Onboarding:** Nuevos miembros aprenden los comandos disponibles
✅ **Productividad:** Focus en lógica de negocio, no en tareas repetitivas

---

### 2.8 Ejercicio Práctico: Demo Completa

#### Objetivo:
Demostrar el uso de configuraciones en `copilot-instructions.md`, comandos personalizados y control de código.

#### Escenario:
Crear un servicio REST para gestión de productos con todas las mejores prácticas.

#### Paso 1: Configurar `copilot-instructions.md`

```markdown
# Instrucciones GitHub Copilot - Proyecto Demo

## Contexto
API REST con Spring Boot 3.2, Java 17, PostgreSQL.
Arquitectura en capas: Controller → Service → Repository.

## Estándares
- Lombok para reducir boilerplate
- ResponseEntity para respuestas HTTP
- DTO pattern para transferencia de datos
- Manejo centralizado de excepciones con @ControllerAdvice
- Validación con Jakarta Validation
- OpenAPI 3.0 para documentación

## Testing
- JUnit 5 + Mockito
- Cobertura mínima: 80%
- Tests de integración con TestContainers

## Comandos Personalizados

### /crear-controller
Crear controlador REST con:
- @RestController y @RequestMapping
- Métodos CRUD completos (GET, POST, PUT, DELETE)
- ResponseEntity con códigos HTTP apropiados
- Validación con @Valid
- OpenAPI annotations (@Operation, @ApiResponse)

### /crear-service
Crear servicio con:
- @Service annotation
- Inyección por constructor
- Manejo de Optional
- Excepciones de negocio personalizadas
- Logs con SLF4J

### /crear-test-completo
Generar suite completa de tests:
- Tests unitarios de service (con mocks)
- Tests de integración de controller (MockMvc)
- Casos: happy path, validaciones, errores
```

#### Paso 2: Implementación con Copilot

**2.1 Crear entidad:**
```
Prompt: "Crea una entidad Product con id, name, description, 
price, stock, createdAt. Usa Lombok y JPA annotations"
```

**2.2 Crear repositorio:**
```
Prompt: "Crea ProductRepository que extienda JpaRepository"
```

**2.3 Crear DTO:**
```
Prompt: "Crea ProductDTO y ProductRequestDTO con validaciones 
Jakarta: name required max 100, price positive, stock non-negative"
```

**2.4 Crear servicio:**
```
Prompt: "/crear-service ProductService con métodos: 
findAll, findById, create, update, delete"
```

**2.5 Crear controlador:**
```
Prompt: "/crear-controller ProductController en /api/products"
```

**2.6 Crear tests:**
```
Prompt: "/crear-test-completo para ProductService"
```

#### Paso 3: Control de Calidad

**3.1 Revisar código:**
```
[Seleccionar ProductService.java]
Prompt: "/review"
```

**3.2 Ajustar estilo:**
```
Prompt: "Ajustar estilo de codigo en todos los archivos del paquete"
```

**3.3 Documentar:**
```
Prompt: "/documentar ProductService y ProductController"
```

#### Paso 4: Verificación

**4.1 Ejecutar tests:**
```bash
# Ejecuta la suite de tests de tu proyecto
# (ej: mvn test, gradle test, npm test, dotnet test, pytest)
<tu comando de tests aquí>
```

**4.2 Verificar cobertura:**
```bash
# Ejecuta tests con cobertura y abre el reporte generado
# (la herramienta depende de tu stack)
<tu comando de cobertura aquí>
```

**4.3 Generar mensaje de commit:**
```
Prompt: "/commit-msg para estos cambios"

Resultado:
feat(products): implementar CRUD completo de productos

- Agregar entidad Product con JPA
- Crear ProductService con lógica de negocio
- Implementar ProductController REST API
- Añadir DTOs con validaciones Jakarta
- Tests unitarios y de integración (85% cobertura)
- Documentación OpenAPI
```

---

### 2.9 Detección y Corrección de Errores

#### Detectar Errores con GitHub Copilot

**Método 1: Análisis de código existente**
```
[Seleccionar método con bug]
Prompt: "Analiza este código y encuentra posibles errores o bugs"
```

**Método 2: Comando /fix**
```
[Seleccionar código problemático]
/fix
```

**Método 3: Descripción del problema**
```
Prompt: "En UserService.updateUser() se lanza NullPointerException 
cuando el email es null. Analiza y corrige el método"
```

#### Ejemplo Práctico:

**Código con bug:**
```java
public void processOrder(Order order) {
    if (order.getItems().size() > 0) {
        BigDecimal total = BigDecimal.ZERO;
        for (Item item : order.getItems()) {
            total = total.add(item.getPrice());
        }
        order.setTotal(total);
        orderRepository.save(order);
    }
}
```

**Prompt para Copilot:**
```
Analiza este método y encuentra errores potenciales:
1. NullPointerException
2. Problemas con BigDecimal
3. Validaciones faltantes
```

**Copilot identifica:**
```
❌ No valida si order es null
❌ No valida si order.getItems() es null
❌ No considera cantidad de items (solo suma precio unitario)
❌ No maneja caso de orden sin items
❌ No valida si price de item es null
❌ No usa transacciones
```

**Código corregido:**
```java
@Transactional
public void processOrder(Order order) {
    if (order == null) {
        throw new IllegalArgumentException("Order cannot be null");
    }
    
    List<Item> items = order.getItems();
    if (items == null || items.isEmpty()) {
        throw new IllegalStateException("Order must have at least one item");
    }
    
    BigDecimal total = items.stream()
        .map(item -> {
            if (item.getPrice() == null) {
                throw new IllegalStateException("Item price cannot be null");
            }
            int quantity = item.getQuantity() != null ? item.getQuantity() : 1;
            return item.getPrice().multiply(BigDecimal.valueOf(quantity));
        })
        .reduce(BigDecimal.ZERO, BigDecimal::add);
    
    order.setTotal(total);
    orderRepository.save(order);
}
```

---

### 2.10 Pruebas Unitarias y Cobertura de Código

#### Generar Pruebas Unitarias con Copilot

**Método 1: Comando /tests**
```
[Seleccionar método o clase]
/tests
```

**Método 2: Prompt específico**
```
Prompt: "Genera tests unitarios para ProductService.createProduct() 
incluyendo: caso exitoso, validación de campos, manejo de duplicados, 
excepciones de BD. Usa JUnit 5, Mockito y AssertJ"
```

#### Ejemplo Completo:

**Clase a testear (simplificada):**
```java
public class ProductService {
    public Product createProduct(ProductRequestDTO request) {
        // 1) Validar request
        // 2) Revisar duplicados
        // 3) Guardar y retornar
        return new Product();
    }
}
```

**Prompt:**
```
Genera suite completa de tests para createProduct con:
- Happy path
- Validación de duplicados
- Edge cases (stock en 0, precio mínimo)
- Excepciones de repositorio
- Cobertura 100%
```

**Test generado (ejemplo 1 caso):**
```java
class ProductServiceTest {
    @Test
    void shouldCreateProduct() {
        // Given: request válido
        // When: createProduct(request)
        // Then: retorna producto y no falla
    }
}
```

**Otros casos que normalmente agregas:** duplicado (debe fallar), validaciones (nombre vacío, precio negativo), stock 0, y errores del repositorio/BD.

#### Verificar Cobertura de Código (agnóstico a tecnología)

- Usa la herramienta de cobertura de tu stack (la opción exacta cambia según lenguaje y framework).
- Ejecuta los tests con cobertura, revisa qué líneas/ramas quedaron sin cubrir, y agrega pruebas donde tenga sentido.
- Define un umbral mínimo en CI (por ejemplo 80%) para evitar regresiones.

**Usar Copilot para mejorar cobertura (genérico):**
```
Prompt: "El reporte de cobertura muestra 65% en ProductService. Genera tests adicionales para alcanzar 85%, priorizando casos borde y manejo de errores"
```

---

### 2.11 TDD con Inteligencia Artificial

#### ¿Qué es TDD?
**Test-Driven Development:** Escribir tests ANTES de implementar el código.

#### Ciclo TDD:
1. 🔴 **Red:** Escribir test que falla
2. 🟢 **Green:** Escribir código mínimo para que pase
3. 🔵 **Refactor:** Mejorar el código manteniendo tests verdes

#### Cómo hacer TDD con GitHub Copilot:

#### Paso 1: Definir requisitos
```
Prompt: "Necesito implementar calculadora de impuestos con estas reglas:
- Productos de primera necesidad: 0% IVA
- Productos generales: 16% IVA
- Productos de lujo: 30% IVA
- Descuento por mayoreo: si cantidad >= 10, 5% descuento adicional

Genera los casos de prueba primero siguiendo TDD"
```

#### Paso 2: Copilot genera los tests (RED)
```java
@DisplayName("TaxCalculator Tests")
class TaxCalculatorTest {

    @Test
    void shouldApplyTaxToGeneralProduct() {
        // Given: price=100, type=GENERAL
        // When: calculate(type, price, qty=1)
        // Then: 116.00
    }

    @Test
    void shouldApplyBulkDiscountFor10OrMore() {
        // Given: price=100, type=GENERAL, qty=10
        // When
        // Then: aplica descuento adicional
    }
}
```

**Ejecutar tests → Todos FALLAN ❌ (porque no existe la implementación)**

#### Paso 3: Implementar código mínimo (GREEN)
```
Prompt: "Implementa TaxCalculator para que pasen todos los tests"
```

```java
public class TaxCalculator {
    
    public BigDecimal calculate(ProductType type, BigDecimal price, int quantity) {
        BigDecimal taxRate = switch (type) {
            case BASIC -> BigDecimal.ZERO;
            case GENERAL -> new BigDecimal("0.16");
            case LUXURY -> new BigDecimal("0.30");
        };

        BigDecimal total = price.multiply(BigDecimal.ONE.add(taxRate));
        if (quantity >= 10) {
            total = total.multiply(new BigDecimal("0.95"));
        }

        return total.setScale(2, RoundingMode.HALF_UP);
    }
}
```

**Ejecutar tests → Todos PASAN ✅**

#### Paso 4: Refactorizar (REFACTOR)
```
Prompt: "Refactoriza TaxCalculator para:
- Extraer constantes mágicas
- Mejorar legibilidad
- Añadir validaciones
Mantén los tests pasando"
```

**Refactor típico (sin tanto código):**
- Extraer constantes (tasas, umbrales).
- Separar validaciones, cálculo de impuestos y descuento.
- Mejorar nombres y eliminar “números mágicos”.
- Mantener los tests en verde como red de seguridad.

**Ejecutar tests → Todos PASAN ✅**

#### Ventajas de TDD con IA:
- ✅ IA genera casos de prueba completos (incluso edge cases que podrías olvidar)
- ✅ Implementación guiada por requisitos claros
- ✅ Refactorización segura (tests como red de seguridad)
- ✅ Documentación viva (tests como especificación)
- ✅ Mayor confianza en el código

---

## 😄 DATOS CURIOSOS

### 🚨 No descuides el chat, siempre hay aprobación que dar

![Meme conceptual: Desarrollador durmiendo mientras GitHub Copilot espera aprobación]

**Lección:** GitHub Copilot sugiere, pero TÚ decides. No aceptes sugerencias a ciegas.

---

### 🤖 Curiosidades sobre GitHub Copilot

1. **📊 GitHub Copilot se entrena con código público**
   - Aprende de millones de repositorios en GitHub
   - Por eso conoce frameworks populares mejor que los obscuros

2. **🧠 No memoriza código, lo genera**
   - Usa modelos de lenguaje, no búsqueda en bases de datos
   - Similar a cómo tu cerebro genera frases nuevas

3. **⚡ Procesa contexto en milisegundos**
   - Analiza archivos abiertos, código actual, y dependencias
   - Por eso es importante mantener tu workspace organizado

4. **🌍 Políglota natural**
   - Soporta más de 40 lenguajes de programación
   - Puede traducir código entre lenguajes

5. **📈 Mejora con el tiempo**
   - Los modelos se actualizan regularmente
   - Tu feedback ayuda a mejorar las sugerencias

6. **🎯 Contexto es rey**
   - Mejor contexto = mejores sugerencias
   - Por eso `copilot-instructions.md` es tan poderoso

7. **👥 55% de código más rápido**
   - Estudios muestran incremento promedio de productividad
   - Algunos desarrolladores reportan hasta 70% en tareas específicas

8. **🔒 Respeta privacidad en Enterprise**
   - Modo Enterprise no usa tu código para entrenamiento
   - Datos no se comparten con OpenAI

9. **💡 Predice tu intención**
   - Analiza patrones en tu forma de codificar
   - Se adapta a tu estilo personal

10. **🎮 Hasta puede programar en lenguajes esotéricos**
    - Brainfuck, Malbolge, Whitespace...
    - ¡Aunque no lo recomendamos para producción!

---

### 🎭 Memes y Realidades

**Expectativa vs Realidad:**
- **Expectativa:** "Copilot escribirá todo mi código"
- **Realidad:** "Copilot me ahorra escribir boilerplate y me da ideas"

**La regla 80/20:**
- Copilot hace el 80% del trabajo tedioso
- Tú haces el 20% crítico que requiere criterio

**Síndrome del "acepto sin leer":**
- No seas ese desarrollador que acepta todas las sugerencias
- Code review aplica también para código generado por IA

---

## 🎯 QUIZ - Kahoot

### Sugerencia de 10 Preguntas con 4 Opciones

#### Pregunta 1: ¿Qué es GitHub Copilot?
- A) Un algoritmo de búsqueda de código
- B) Un asistente de código impulsado por IA ✅
- C) Un compilador inteligente
- D) Una herramienta de debugging

#### Pregunta 2: ¿Cuál NO es un modo de interacción con Copilot?
- A) Ask
- B) Agent
- C) Deploy ✅
- D) Edit

#### Pregunta 3: ¿Cuál es el propósito del archivo copilot-instructions.md?
- A) Configurar el compilador
- B) Definir reglas y contexto para Copilot ✅
- C) Documentar el proyecto para usuarios finales
- D) Almacenar logs de Copilot

#### Pregunta 4: ¿Qué símbolo se usa para referenciar un archivo en Copilot Chat?
- A) @file
- B) #file ✅
- C) /file
- D) $file

#### Pregunta 5: En TDD, ¿cuál es el orden correcto?
- A) Código → Test → Refactor
- B) Refactor → Test → Código
- C) Test → Código → Refactor ✅
- D) Test → Refactor → Código

#### Pregunta 6: ¿Qué comando de Copilot genera pruebas unitarias?
- A) /test
- B) /tests ✅
- C) /unit
- D) /testing

#### Pregunta 7: ¿Cuál es la cobertura de código mínima recomendada?
- A) 50%
- B) 65%
- C) 80% ✅
- D) 100%

#### Pregunta 8: ¿Qué NO debe contener un buen prompt?
- A) Contexto claro
- B) Requisitos específicos
- C) Ambigüedad y vaguedad ✅
- D) Ejemplos de uso

#### Pregunta 9: ¿Cuál es el rol del desarrollador al usar Copilot?
- A) Piloto que delega todo
- B) Copiloto que supervisa y valida ✅
- C) Pasajero que no interviene
- D) Mecánico que solo arregla errores

#### Pregunta 10: ¿Para qué sirve el archivo CHANGELOG.md?
- A) Configurar dependencias
- B) Documentar cambios y decisiones técnicas ✅
- C) Almacenar credenciales
- D) Configurar el IDE

---

## 📝 Notas Finales

### Recursos Adicionales:
- 📖 [Documentación oficial de GitHub Copilot](https://docs.github.com/copilot)
- 🎓 [GitHub Copilot Learning Path](https://learn.microsoft.com/training/github/)
- 💬 [Comunidad y Forum](https://github.community/)

### Próximos Pasos:
1. Configurar GitHub Copilot en tu IDE
2. Crear tu primer `copilot-instructions.md`
3. Practicar con ejercicios TDD
4. Compartir aprendizajes con tu equipo

---

**¡Feliz codificación con GitHub Copilot! 🚀**
