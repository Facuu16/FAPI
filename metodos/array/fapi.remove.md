---
description: Elimina un elemento de un array.
---

# FAPI.remove()

**Parámetros**:\
Objeto el cual se eliminará del array.\
Array del cual se eliminará el objeto.

```javascript
var countries = ["Inglaterra", "Suiza", "Chile"];

API.message(player, FAPI.remove("Inglaterra", countries).join(',')); // SALIDA: ["Suiza, "Chile]
```
