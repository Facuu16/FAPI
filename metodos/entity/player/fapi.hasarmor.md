---
description: Determina si un jugador tiene la armadura especificada.
---

# FAPI.hasArmor()

**Parámetros**:\
Jugador, ID del Casco, ID de la Pechera, ID de los Pantalones, ID de las Botas.\
"none" si se quiere hacer una excepción de la parte actual.

Devuelve un valor booleano que indica si el jugador tiene la armadura especificada.

```javascript
// VERIFICA SI UN JUGADOR TIENE UNA ARMADURA DE DIAMANTE:
if (FAPI.hasArmor(player, 310, 311, 312, 313)) {
    API.message(player, "¡Tienes una armadura de diamante!");
}

// VERIFICA SI UN JUGADOR TIENE UNA ARMADURA DE HIERRO, EXCEPTUANDO LOS PANTALONES:
if (FAPI.hasArmor(player, 306, 307, "none", 309)) {
    API.message(player, "¡Tienes una armadura de hierro, pero te faltan los pantalones!");
}
```
