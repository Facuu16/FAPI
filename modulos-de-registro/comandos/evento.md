---
description: Contiene métodos para acceder a las propiedades del evento.
---

# Evento

* **getPermission()**: Devuelve el permiso necesario para ejecutar el comando, NULL si no tiene permiso.
* **getCommand()**: Devuelve el nombre del comando.
* **getArguments()**: Devuelve un arreglo con los argumentos proporcionados, sin incluir el comando.
* **getPlayer()**: Devuelve el jugador que ejecutó el comando.
* **getHandlers()**: Devuelve la lista de manejadores registrados.

```javascript
FAPI.registerCommand("prueba", null, function (event) {  
  var player = event.getPlayer();  

  API.message(player, "El permiso de este comando es: " + event.getPermission()); 
  API.message(player, "El comando ejecutado es: " + event.getCommand());
  API.message(player, "Los argumentos son: " + event.getArguments().join(','));
});
```
