# Instrucciones para Copilot Agent Mode

## 1. Comportamiento General

- No realices cambios sin aprobación explícita del usuario.
- Antes de modificar, explica:
    1. Archivo y líneas afectadas.
    2. Qué cambio se propone.
    3. Motivo y utilidad.
    4. Impacto en el proyecto.

## 2. Flujo de Trabajo

- Espera confirmación antes de aplicar cualquier cambio.
- Si el cambio afecta varios archivos, presenta primero un resumen y luego el detalle por archivo.
- Si detectas errores o mejoras, sugiere, no ejecutes automáticamente.

## 3. Perfil del Usuario

- Asume que el usuario es nuevo en el código base.
- Sé claro, detallado y evita suposiciones.

## 4. Estilo y Buenas Prácticas

- Aplica buenas prácticas de desarrollo.
- Mantén la coherencia con el estilo actual del proyecto.

## 5. Evaluación y Tiempos

- Analiza el código con calma y profundidad.
- Evita respuestas rápidas o superficiales.
- Si hay varias soluciones, evalúa cuál es la mejor para el estado actual del proyecto.

## 6. Cobertura de Pruebas

- Si se solicita ayuda con cobertura:
    - Garantiza cobertura total (100%) del código evaluado.
    - Considera casos normales, de borde y excepciones.
    - Usa pruebas existentes como referencia.
    - Verifica que las pruebas cubran el comportamiento esperado.
    - Sin compilar, valida que no haya errores de ejecución ni fallos por mocks incorrectos.

## 7. Reglas Obligatorias

- Cumple estas reglas en cada interacción con Copilot Agent Mode.
- Al iniciar cada sesión, lee y aplica el contenido de `.github/copilot-instructions.md` sin excepción.
- Documenta cada cambio realizado en un registro de cambios (`.github/CHANGELOG.md`) ubicado en la raíz del proyecto, especificando fecha, motivo y archivos afectados.

## 8. Comandos

- Cuando se detecte un comentario que diga "Ajustar estilo de codigo", hacer:
    - identar correctamente el codigo
    - eliminar imports no usados
    - ajustar espacios en blanco innecesarios
    - asegurar que las lineas no excedan 120 caracteres
    - simplificar el codigo
    - advertir si se superan las 500 lineas de codigo en un solo archivo

- Cuando se detecte un comentario que diga "Revisa nullPointer", hacer:
    - Analizar el codigo de la clase, para identificar si existen posibles nullPointerExceptions
    - Sugerir las modificaciones necesarias para evitar los nullPointerExceptions
    - Sugerir que valores son obligatorios para la clase
    - Sugerir controlar null en los metodos para evitar nullPointerExceptions

- Cuando se detecte un comentario que diga "crear dummi", hacer:
    - cree un archivo en la raiz llamado DUMMY.txt
    - agrege el numero total de clases que tiene el proyecto como total de clases = ###


## 9. Entorno de Desarrollo

- **Shell:** Todos los comandos deben ser compatibles con **Windows PowerShell**.
- **Gradle:** Siempre usar el wrapper de Gradle del proyecto: `.\gradlew` o `./gradlew`
    - Nunca usar `gradle` directamente.
    - Ejemplos de comandos comunes:
        - Compilar: `.\gradlew build`
        - Limpiar: `.\gradlew clean`
        - Ejecutar tests: `.\gradlew test`
        - Ver tareas: `.\gradlew tasks`
        - Compilar sin tests: `.\gradlew build -x test`
        - Listar proyectos: `.\gradlew projects`
    - **Ejecutar tests de módulos específicos:**
        - Primero verificar el nombre del proyecto con: `.\gradlew projects`
        - Luego ejecutar tests del módulo usando el formato: `.\gradlew :[nombre-del-proyecto]:test`
        - Para una clase específica: `.\gradlew :[nombre-del-proyecto]:test --tests "paquete.Clase"`
        - Ejemplo: `.\gradlew :driven-adapters-rest-adapter:test --tests "co.com.sura.p8.P8RepositoryAdapterTest"`
- **Sintaxis PowerShell:**
    - Usar `.\` para ejecutar archivos en el directorio actual
    - Usar `;` para separar comandos en una línea
    - Usar `&&` NO está disponible en PowerShell, usar `;` o ejecutar comandos por separado
    - Para variables de entorno: `$env:VARIABLE_NAME`
- **Navegación:**
    - Cambiar directorio: `cd ruta\al\directorio`
    - Listar archivos: `dir` o `ls`
    - Ver contenido de archivo: `Get-Content archivo.txt` o `cat archivo.txt`

