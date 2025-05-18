> Detalla en esta sección los prompts principales utilizados durante la creación del proyecto, que justifiquen el uso de asistentes de código en todas las fases del ciclo de vida del desarrollo. Esperamos un máximo de 3 por sección, principalmente los de creación inicial o los de corrección o adición de funcionalidades que consideres más relevantes.
> Puedes añadir adicionalmente la conversación completa como link o archivo adjunto si así lo consideras

## Índice

1. [Descripción general del producto](#1-descripción-general-del-producto)
2. [Arquitectura del sistema](#2-arquitectura-del-sistema)
3. [Modelo de datos](#3-modelo-de-datos)
4. [Especificación de la API](#4-especificación-de-la-api)
5. [Historias de usuario](#5-historias-de-usuario)
6. [Tickets de trabajo](#6-tickets-de-trabajo)
7. [Pull requests](#7-pull-requests)

---

## 1. Descripción general del producto

**Prompt 1:**

```
quiero tener una interfaz o aplicación, tal vez en nodejs en mi M1 que se conecte a llm local.
Mi aplicación se conectará a confluence y creará documentación de mi proyecto.

La idea es desde cualquier otra computadora en la que se trabaje en cursor abrir el chat e indicar que use mi aplicación en mi otra computadora (M1 que tiene un LLM localmente) con cualquier requerimiento

Entonces desde la computadora de trabajo (en cursor) indicar que analice el archivo actual, se conectará a mi aplicación y esta generará documentación como diagramas y descripción del componente, similar a lo que hace coderabbitai. Esta documentación será una nueva página en confluence y como resultado al inicio del archivo actual se colocará el id de la nueva página.

Tiene sentido?
No generes código, quiero que me indiques si es factible
```

**Prompt 2:**

```
ok, ahora con este contexto necesito que seas un experto Product Manager con experiencia en definición de proyectos, delimitación y entrega de proyectos exitosos.

Necesito documentación en markdown que cubra: producto, arquitectura, modelo de datos, API, historias de usuario y tickets de trabajo. El proyecto es una aplicación Node.js que conecta a un LLM local para automatizar la generación de documentación de proyectos en Confluence. Analiza código desde cualquier computador usando Cursor, genera documentación y crea una nueva página de Confluence, devolviendo el ID de la página para insertarlo en el código original.
```

**Prompt 3:**

```
si, para este proyecto necesito que generes cierta documentación.
Formato markdown
Paso a paso
Delimitar este proyecto a 36 horas, apoyándome en la IA
El objetivo del proyecto es desarrollar un producto de software básico de inicio a fin, apoyado en IA en todas las fases del ciclo de vida:

Documentación del producto (general y funcionalidades clave, arquitectura, modelo de datos, API Spec) y del proceso (historias de usuario y tickets de trabajo)
Suite de tests completa
Construir un backend con acceso a base de datos
Construir frontend
Definición de la infraestructura y despliegue
Bien detallado
Quiero que llenes este documento@readme.md a exepción del numeral 7
```

**Prompt 4:**

```
ok, vamos a ir paso por paso.
Enfoquémonos en el paso 1 solamente.
Agrega más detalle en este paso:
Qué incluirá `git clone [URL_REPOSITORIO]`?
qué se instalará?

por otro lado, que pasos se ejecutarán con esta instrucción?
`npm run setup-llm`
en dónde se ejecutará? en la M1, en mi máquina local?
Necesito más detalles
Asegúrate de que el proyecto sea 100% ejecutable

¿Podrías actualizar la sección 1 del readme.md con: descripción del producto, objetivos, características, interfaz de usuario, instrucciones de instalación y notas de validación de calidad?
```

**Prompt 5:**

```
Agrega estas instrucciones en la documentación del paso 1
Recuerda que nos estamos enfocando solo en el paso 1 por ahora
```

**Prompt 6:**

```
¿Podrías actualizar la sección 1.2 del readme.md enfocándote en la documentación de la lógica del código, sin optimizaciones, patrones, roles o permisos? ¿Cómo se validará la calidad de la documentación y en relación a qué criterios?
```

**Prompt 7:**

```
porqué vas a incluir docker? y será en la M1?
todo esto dará tiempo para 36 horas?
```

**Prompt 8:**

```
qué significa ` - Prompts básicos`?
qué incluye el flujo básico?
qué significa esto?
```

**Prompt 9:**

```
Quiero que se genere una buena documentación, de calidad y precisa. Modifica el punto 1.4
```

**Prompt 10:**

```
¿El texto "#### Ejemplo de Documentación de Lógica:" se incluirá en el @readme.md? No creo que sea parte de la documentación.
```

**Prompt 11:**

```
ok, actualiza el punto 1 del @readme.md con esta información
```

**Prompt 12:**

```
modifica este paso, no veo que esté relacionado con la documentación.
Quiero generar documentación de la lógica no optimizaciones ni patrones, roles, permisos, etc

Cómo vas a validar la calidad? respecto a qué?
```

**Prompt 13:**

```
si, pero no pondrás este texto en el @readme.md `#### Ejemplo de Documentación de Lógica:` cierto?
```

**Propmt 14:**

```
ahora actualiza la sección 1 del @readme.md
```

---

## 2. Arquitectura del Sistema

### **2.1. Diagrama de arquitectura:**

**Prompt 1:**

```
ahora enfoquemonos en el numero 2. Con lo que se tenía originalmente?
```

**Prompt 2:**

```
para qué vas a utilizar la base de datos?
```

**Prompt 3:**

```
deja la base de datos, pero almacena algo simple tipo MVP
es necesario incluir un endpoint health?
```

**Prompt 4:**

```
que es `Rate limiting básico`?
```

**Prompt 5:**

```
porque lo quitaste? este documento es el alcance/requerimientos del proyecto. Debo indicar que tests voy a incluir
```

**Prompt 6:**

```
No creo que este proyecto esté delimitado a 36 horas
recuerda 36 horas!!!
```

**Prompt 7**

```
ok, actualiza la sección 2 en donde corresponde @readme.md
```

**Prompt 8:**

```
¿Podrías agregar también un diagrama de flujo? Similar a lo que hace code rabbit
```

**Prompt 9:**

```
el diagrama mermaid lo veo muy sencillo, podrías agregar también un diagrama de flujo?
similar a lo que hace code rabbit
```

**Prompt 10:**

```
¿La sección de tests es parte de la documentación? Veo que menciona Jest, RTL, Cypress y otras estrategias de testing.
```

**Prompt 9:**

```
¿Podrías agregar las secciones 3,4,5 y 6 que ya no aparecen en el readme.md?
```

### **2.2. Descripción de componentes principales:**

**Prompt 1:**

```
¿Es necesario incluir un health endpoint en el MVP?
```

**Prompt 2:**

```
¿Qué significa "Rate limiting básico" en la sección de seguridad?
```

**Prompt 3:**

```
¿La sección de tests es parte de la documentación? Veo que menciona Jest, RTL, Cypress y otras estrategias de testing.
```

### **2.3. Descripción de alto nivel del proyecto y estructura de ficheros**

**Prompt 1:**

```
¿Es realista completar todo esto en 36 horas?
```

**Prompt 2:**

```
¿Podrías actualizar la sección 2 del readme.md manteniendo el formato original pero con el contenido actualizado?
```

---

### 3. Modelo de Datos

**Prompt 1:**

```
En el paso 3 veo los subtítulos modificados, deja los que estaban
```

**Prompt 2:**

```
¿Dónde están estos títulos? Los originales?
### **3.1. Diagrama del modelo de datos:**
### **3.2. Descripción de entidades principales:**
```

**Prompt 3:**

````
¿Qué es esto? ¿Por qué pusiste esto por ejemplo?
```mermaid
erDiagram
    ANALYSIS {
        text id PK
        text file_path
        text confluence_page_id
        timestamp created_at
        text status
    }
````

**Prompt 4:**

```
ok, ahora agrega todos los prompts de esta conversación en el archivo @prompts.md
```

---

### 4. Especificación de la API

**Prompt 1:**

```

¿Podrías detallar los endpoints necesarios para el MVP?

```

**Prompt 2:**

```

¿Cómo se manejarán los errores en la API?

```

**Prompt 3:**

```

¿Qué autenticación necesitamos para la API de Confluence?

```

---

### 5. Historias de Usuario

**Prompt 1:**

```

¿Podrías definir las historias de usuario principales para el MVP?

```

**Prompt 2:**

```

¿Cómo se priorizarán las historias de usuario?

```

**Prompt 3:**

```

¿Qué criterios de aceptación tendrán las historias de usuario?

```

---

### 6. Tickets de Trabajo

**Prompt 1:**

```

¿Podrías desglosar los tickets en tareas más pequeñas para el MVP de 36 horas?

```

**Prompt 2:**

```

¿Cómo se organizarán las tareas para maximizar el tiempo disponible?

```

**Prompt 3:**

```

¿Qué tareas podrían dejarse para una futura iteración?

```

---

### 7. Pull Requests

**Prompt 1:**

```

¿Cómo se manejarán los pull requests en el MVP?

```

**Prompt 2:**

```

¿Qué criterios de revisión se usarán?

```

**Prompt 3:**

```

¿Cómo se integrarán los cambios en el repositorio principal?

```
