---
description: Primeros pasos con FAPI...
---

# Introducción

¿**Qué es FAPI**?

FAPI amplía la funcionalidad de la API del servidor (DBCHispano) y proporciona métodos útiles para simplificar tareas en desarrollo de scripts. Con FAPI, se puede integrar funcionalidades en los proyectos de una manera sencilla y eficiente.

**Para integrar FAPI en tu proyecto, debes agregar las siguientes líneas de código en tu script**;

```javascript
var FAPI;

function onInit() {  
    FAPI = API.getTempData("FAPI");  
}
```
