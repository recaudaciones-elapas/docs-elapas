# Flujo del MVP

## Introducción

El MVP del proyecto **Sistema de Gestión de Recaudaciones y Cortes para ELAPAS - Sucre** busca demostrar un flujo funcional básico entre el trabajo de campo, el procesamiento de datos y la consulta administrativa.

El objetivo no es implementar todas las capacidades de un sistema final, sino evidenciar que los módulos principales pueden integrarse correctamente y cumplir con el proceso esencial del proyecto.

## Flujo general del sistema

El flujo principal del MVP será el siguiente:

1. El brigadista inicia sesión en el módulo móvil.
2. El brigadista busca o selecciona un cliente.
3. El brigadista registra una lectura de consumo o un corte de servicio.
4. En caso de corte, adjunta una fotografía como evidencia.
5. La aplicación móvil envía la información al backend.
6. El backend procesa y almacena los datos.
7. La aplicación web consulta la información almacenada.
8. El personal administrativo visualiza lecturas, deudas o cortes registrados.

## Flujo detallado

## 1. Inicio de sesión

El usuario del módulo móvil o del sistema web ingresa sus credenciales para acceder al sistema.

### Resultado esperado
El sistema valida el acceso y habilita las funcionalidades correspondientes.

## 2. Selección o búsqueda de cliente

Desde el módulo móvil, el brigadista selecciona un cliente o realiza una búsqueda básica usando un criterio como nombre, código o identificación.

### Resultado esperado
El sistema muestra los datos básicos del cliente para continuar con el proceso.

## 3. Registro de lectura

El brigadista introduce la lectura actual del medidor del cliente desde la aplicación móvil.

### Resultado esperado
La lectura queda registrada y asociada al cliente correspondiente.

## 4. Registro de corte

Si corresponde un corte de servicio, el brigadista registra el evento desde la aplicación móvil.

### Datos esperados
- cliente asociado
- fecha del registro
- observación básica
- fotografía de evidencia

### Resultado esperado
El corte queda almacenado como un registro dentro del sistema.

## 5. Envío de datos al backend

La aplicación móvil envía la información registrada al backend mediante la API.

### Resultado esperado
Los datos son recibidos, validados y almacenados correctamente.

## 6. Procesamiento y almacenamiento

El backend recibe la información, la organiza y la guarda en la base de datos.

### Resultado esperado
La información queda disponible para futuras consultas desde la web.

## 7. Consulta desde interfaz web

El personal administrativo accede a la aplicación web para revisar la información registrada.

### Funciones esperadas en esta etapa
- consultar clientes
- revisar lecturas
- revisar cortes
- consultar deuda básica

## 8. Visualización administrativa

La aplicación web presenta la información registrada de forma clara y ordenada para apoyar el seguimiento operativo.

### Resultado esperado
Se puede demostrar que la información capturada en campo llega al sistema y es visible para el área administrativa.

## Flujo resumido

Brigadista en móvil → registro de lectura o corte → envío a API → almacenamiento en backend → consulta en web → visualización administrativa

## Alcance del flujo en el MVP

El flujo del MVP estará limitado a una versión básica y funcional. No incluirá procesos avanzados como:

- integración con pagos reales,
- geolocalización avanzada,
- sincronización offline compleja,
- notificaciones automáticas,
- reportes avanzados.

## Importancia del flujo definido

Este flujo es importante porque permite demostrar:

- integración entre módulos,
- captura de información desde campo,
- almacenamiento centralizado,
- consulta posterior desde entorno web,
- viabilidad del sistema como solución digital inicial.

## Conclusión

El flujo definido para el MVP representa el proceso central que el proyecto busca resolver. Su implementación permitirá mostrar un sistema funcional, coherente y demostrable dentro del tiempo disponible, manteniendo un alcance realista para un proyecto académico.