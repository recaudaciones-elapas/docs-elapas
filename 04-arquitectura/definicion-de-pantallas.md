# Definición de pantallas web y móvil

## Introducción

La definición de pantallas permite establecer de forma clara qué vistas tendrá el sistema, qué función cumplirá cada una y qué usuario interactuará con ellas. Esta actividad es importante porque ayuda a delimitar el alcance visual y funcional del MVP antes de iniciar el desarrollo.

En este proyecto, las pantallas se dividen en dos grupos principales:

- pantallas web, orientadas al personal administrativo o de control;
- pantallas móviles, orientadas al brigadista o técnico de campo.

El objetivo es definir únicamente las pantallas necesarias para demostrar el flujo principal del MVP.

## Objetivo de la definición de pantallas

Definir las vistas mínimas necesarias para que el MVP permita:

- registrar información desde campo;
- consultar información desde la web;
- visualizar datos clave del sistema;
- conectar correctamente los módulos móvil, backend y web.

## Criterios de selección de pantallas

Las pantallas fueron definidas considerando:

- el alcance reducido del MVP;
- el tiempo disponible del proyecto;
- el tipo de usuario que interactúa con el sistema;
- la necesidad de demostrar el flujo funcional principal;
- la prioridad de implementar primero pantallas esenciales.

---

# Pantallas del módulo web

## 1. Pantalla de inicio de sesión web

- **Módulo:** web
- **Usuario principal:** personal administrativo
- **Objetivo:** permitir el acceso al sistema web mediante credenciales básicas.

### Elementos principales
- campo de usuario o correo
- campo de contraseña
- botón de inicio de sesión
- mensaje de error en caso de acceso inválido

### Prioridad
Alta

---

## 2. Pantalla de dashboard principal

- **Módulo:** web
- **Usuario principal:** personal administrativo
- **Objetivo:** mostrar un resumen general del sistema y facilitar el acceso a las principales funciones.

### Elementos principales
- cantidad total de clientes
- cantidad de lecturas registradas
- cantidad de cortes registrados
- indicador básico de deuda o recaudación
- accesos rápidos a clientes, lecturas y cortes

### Prioridad
Alta

---

## 3. Pantalla de listado de clientes

- **Módulo:** web
- **Usuario principal:** personal administrativo
- **Objetivo:** consultar los clientes registrados en el sistema.

### Elementos principales
- tabla de clientes
- búsqueda por nombre, código o identificador
- botón para ver detalle del cliente

### Prioridad
Alta

---

## 4. Pantalla de detalle de cliente

- **Módulo:** web
- **Usuario principal:** personal administrativo
- **Objetivo:** mostrar la información básica de un cliente específico.

### Elementos principales
- nombre del cliente
- código o identificador
- dirección
- información del medidor
- deuda actual básica
- historial simple de lecturas o cortes

### Prioridad
Media

---

## 5. Pantalla de listado de lecturas

- **Módulo:** web
- **Usuario principal:** personal administrativo
- **Objetivo:** visualizar las lecturas registradas desde el módulo móvil.

### Elementos principales
- tabla de lecturas
- nombre o código del cliente
- fecha del registro
- valor de lectura
- filtro o búsqueda simple

### Prioridad
Alta

---

## 6. Pantalla de listado de cortes

- **Módulo:** web
- **Usuario principal:** personal administrativo
- **Objetivo:** visualizar los cortes de servicio registrados en el sistema.

### Elementos principales
- tabla de cortes
- cliente asociado
- fecha del corte
- observación
- evidencia fotográfica, si se muestra en esta etapa
- estado del registro

### Prioridad
Alta

---

## 7. Pantalla de consulta de deuda

- **Módulo:** web
- **Usuario principal:** personal administrativo
- **Objetivo:** consultar la deuda básica de un cliente.

### Elementos principales
- buscador de cliente
- monto adeudado
- estado básico de deuda
- fecha o referencia de última actualización

### Prioridad
Alta

---

# Pantallas del módulo móvil

## 1. Pantalla de inicio de sesión móvil

- **Módulo:** móvil
- **Usuario principal:** brigadista o técnico de campo
- **Objetivo:** permitir el acceso a la aplicación móvil.

### Elementos principales
- campo de usuario
- campo de contraseña
- botón de ingreso
- mensaje de error en caso de credenciales inválidas

### Prioridad
Alta

---

## 2. Pantalla de inicio móvil

- **Módulo:** móvil
- **Usuario principal:** brigadista o técnico de campo
- **Objetivo:** mostrar las funciones principales disponibles en la app.

### Elementos principales
- acceso a registro de lectura
- acceso a registro de corte
- acceso a búsqueda de cliente

### Prioridad
Alta

---

## 3. Pantalla de búsqueda o selección de cliente

- **Módulo:** móvil
- **Usuario principal:** brigadista o técnico de campo
- **Objetivo:** permitir encontrar al cliente sobre el cual se realizará una operación.

### Elementos principales
- campo de búsqueda
- lista de resultados
- botón o acción para seleccionar cliente

### Prioridad
Alta

---

## 4. Pantalla de registro de lectura

- **Módulo:** móvil
- **Usuario principal:** brigadista o técnico de campo
- **Objetivo:** registrar la lectura actual del medidor de un cliente.

### Elementos principales
- cliente seleccionado
- campo para ingresar lectura
- fecha del registro
- observación opcional
- botón guardar o enviar

### Prioridad
Alta

---

## 5. Pantalla de registro de corte

- **Módulo:** móvil
- **Usuario principal:** brigadista o técnico de campo
- **Objetivo:** registrar un corte de servicio realizado en campo.

### Elementos principales
- cliente seleccionado
- fecha del registro
- motivo u observación
- botón para adjuntar evidencia
- botón guardar o enviar

### Prioridad
Alta

---

## 6. Pantalla de evidencia fotográfica

- **Módulo:** móvil
- **Usuario principal:** brigadista o técnico de campo
- **Objetivo:** capturar o adjuntar una imagen como respaldo del corte realizado.

### Elementos principales
- acceso a cámara o selector de imagen
- vista previa de la fotografía
- botón confirmar
- botón cancelar o repetir

### Prioridad
Media

---

# Relación entre pantallas

## Flujo web básico

Inicio de sesión web → dashboard → clientes / lecturas / cortes / deuda

## Flujo móvil básico

Inicio de sesión móvil → inicio móvil → búsqueda de cliente → registro de lectura o registro de corte → evidencia fotográfica → envío al sistema

---

# Pantallas prioritarias del MVP

## Web
Las pantallas prioritarias para el MVP son:

- inicio de sesión web
- dashboard principal
- listado de clientes
- listado de lecturas
- listado de cortes
- consulta de deuda

## Móvil
Las pantallas prioritarias para el MVP son:

- inicio de sesión móvil
- inicio móvil
- búsqueda de cliente
- registro de lectura
- registro de corte

## Pantallas de prioridad media
Estas pantallas pueden implementarse si el tiempo lo permite:

- detalle de cliente
- evidencia fotográfica con vista previa más completa

---

# Pantallas fuera del alcance actual

En esta etapa no se consideran necesarias las siguientes pantallas:

- configuración avanzada de usuario
- paneles analíticos complejos
- historial financiero detallado
- mapas de geolocalización avanzada
- notificaciones
- administración avanzada de roles
- rutas inteligentes de brigadistas

---

# Conclusión

La definición de pantallas establece una base clara para el desarrollo del MVP, permitiendo al equipo identificar qué vistas son esenciales y qué funciones debe cumplir cada una. Esto facilita la organización del trabajo, la distribución de tareas y la construcción progresiva del sistema, manteniendo un alcance realista para el tiempo disponible.