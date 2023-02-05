---
description: Determina si un jugador tiene la armadura especificada.
---

# FAPI.hasArmor()

**Parámetros**:\
Jugador, ID del Casco, ID de la Pechera, ID de los Pantalones, ID de las Botas.\
null en caso de que se quiera hacer una excepción de la parte actual.

Devuelve un valor booleano que indica si el jugador tiene la armadura especificada.

```javascript
// Verifica si un jugador tiene una armadura de diamante
if (FAPI.hasArmor(player, 310, 311, 312, 313)) {
    API.message(player, "¡Tienes una armadura de diamante!");
}

// Verifica si un jugador tiene una armadura de diamante, exceptuando los pantalones
if (FAPI.hasArmor(player, 310, 311, null, 313)) {
    API.message(player, "¡Tienes una armadura de diamante, pero te faltan los pantalones!");
}
```
