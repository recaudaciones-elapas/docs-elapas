# Módulos del sistema

## Introducción

El MVP del proyecto **Sistema de Gestión de Recaudaciones y Cortes para ELAPAS - Sucre** se organizará en tres módulos tecnológicos principales y un módulo de documentación. Esta división permite distribuir mejor el trabajo entre los integrantes del equipo y mantener una arquitectura clara y modular.

La solución busca conectar el trabajo de campo realizado por brigadistas, el procesamiento central de la información y la consulta administrativa y operativa desde una interfaz web.

## Estructura general del sistema

El sistema estará compuesto por los siguientes módulos:

- Backend o API
- Frontend web
- Módulo móvil
- Repositorio de documentación

## 1. Módulo Backend o API

### Descripción
El backend será el núcleo del sistema. Estará encargado de procesar la lógica de negocio, gestionar los datos y exponer servicios mediante una API para que puedan ser consumidos por la aplicación web y la aplicación móvil.

### Tecnología propuesta
- FastAPI

### Responsabilidades principales
- Gestionar autenticación básica
- Registrar y consultar clientes
- Registrar lecturas de consumo
- Registrar cortes de servicio
- Consultar y devolver información de deuda
- Recibir evidencias asociadas a cortes
- Servir datos a la aplicación web y móvil

### Importancia dentro del MVP
Este módulo es central porque conecta todos los componentes del sistema. Sin backend no existiría integración entre móvil, web y datos.

## 2. Módulo Frontend Web

### Descripción
La interfaz web estará orientada a la consulta y visualización de información por parte del personal administrativo o de control. Permitirá revisar datos registrados en el sistema y mostrar una vista básica del estado de clientes, lecturas, deudas y cortes.

### Responsabilidades principales
- Permitir inicio de sesión básico
- Consultar clientes registrados
- Visualizar lecturas registradas
- Visualizar cortes realizados
- Consultar información de deuda
- Mostrar una interfaz administrativa básica

### Importancia dentro del MVP
Este módulo permite evidenciar que la información registrada desde el móvil llega correctamente al sistema y puede ser consultada de forma ordenada.

## 3. Módulo Móvil

### Descripción
La aplicación móvil estará orientada al trabajo de campo. Su función será permitir a los brigadistas registrar información directamente desde terreno, especialmente lecturas y cortes de servicio.

### Responsabilidades principales
- Permitir inicio de sesión básico
- Buscar o seleccionar clientes
- Registrar lecturas de consumo
- Registrar cortes de servicio
- Adjuntar fotografía como evidencia
- Enviar la información al backend

### Alcance del módulo móvil en el MVP
Debido al tiempo disponible y al carácter académico del proyecto, el módulo móvil se desarrollará en una versión básica, priorizando el registro y envío de información. No se incluirán funciones avanzadas como sincronización offline compleja, rutas inteligentes o geolocalización avanzada.

### Importancia dentro del MVP
Este módulo es importante porque permite demostrar el flujo real de captura de datos desde campo, que es uno de los elementos diferenciales del proyecto.

## 4. Repositorio de documentación

### Descripción
Además de los módulos técnicos, el proyecto contará con un repositorio específico de documentación, donde se registrará la planificación, organización, riesgos, avances y otros elementos de gestión del proyecto.

### Responsabilidades principales
- Documentar alcance y objetivos
- Registrar cronograma y organización del equipo
- Identificar riesgos
- Registrar avances semanales
- Servir de apoyo para la presentación final

## Relación entre módulos

Los módulos estarán conectados de la siguiente manera:

1. El módulo móvil registrará lecturas y cortes.
2. La información será enviada al backend.
3. El backend almacenará y procesará los datos.
4. La interfaz web consultará la información registrada.
5. El equipo documentará el avance y las decisiones del proyecto en el repositorio de documentación.

## Justificación de la arquitectura modular

La arquitectura modular fue elegida porque:

- permite dividir el trabajo entre los integrantes,
- facilita la integración progresiva,
- mejora la organización del desarrollo,
- permite construir un MVP más ordenado,
- reduce el riesgo de mezclar responsabilidades en un solo componente.

## Conclusión

La división del sistema en backend, web, móvil y documentación permite construir una solución clara, organizada y adecuada al contexto académico del proyecto. Esta estructura ayuda a enfocar los esfuerzos del equipo en las funcionalidades esenciales del MVP y facilita el seguimiento del trabajo realizado.