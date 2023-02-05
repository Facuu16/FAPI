---
description: Retorna un elemento de un array según un objeto u índice.
---

# FAPI.get()

**Parámetros**:\
Objeto u índice el cual se obtendrá del array.\
Array del cual se obtendrá el objeto u índice.

```javascript
var names = ["Pedro", "Juan", "Carlos"];

API.message(player, FAPI.get("Juan", names)); // SALIDA: "Juan"
API.message(player, FAPI.get(1, names)); // SALIDA: "Juan"
```
