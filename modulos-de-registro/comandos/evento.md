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
FAPI.registerCommand("prueba", "comando.prueba", null, function (event) {  
  var sender = event.getSender(); 

  API.message(sender, "El permiso de este comando es: " + event.getPermission()); 
  API.message(sender, "El comando ejecutado es: " + event.getCommand());
  API.message(sender, "Los argumentos son: " + event.getArguments().join(','));
});
```
