---
description: Determina si un objeto está presente en un array.
---

# FAPI.contains()

**Parámetros**:\
Objeto el cual se verificará si está presente en el array.\
Array del cual se verificará el objeto.

```javascript
var frutas = ["Banana", "Manzana", "Frutilla"];

if (FAPI.contains("Frutilla", frutas)) { // TRUE
    API.message(player, "¡Hay una Frutilla en las frutas!");
} else { // FALSE
    API.message(player, "No hay una Frutilla en las frutas...");
}
```
