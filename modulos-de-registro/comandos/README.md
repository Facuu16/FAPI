---
description: Permite registrar comandos personalizados en el servidor.
---

# Comandos

**Parámetros**:\
El nombre del comando que será registrado. \
El permiso necesario para ejecutar el comando. \
El mensaje que se enviará en caso de no tener el permiso. \
La función que se ejecutará cuando se invoque el comando.

```javascript
// Ejemplo de comando con permiso, y mensaje personalizado en caso de no tener el permiso
FAPI.registerCommand("saludar", "comando.saludar", "&a¡No puedo saludarte!", function (event) {
  var sender = event.getSender();

  API.message(sender, "¡Hola!"); 
});


// Ejemplo de comando con mensaje por defecto en caso de no tener el permiso
FAPI.registerCommand("saludar", "comando.saludar", null, function (event) {
  var sender = event.getSender();

  API.message(sender, "¡Hola!"); 
});


// Ejemplo de comando sin permiso
FAPI.registerCommand("saludar", null, null, function (event) {
  var sender = event.getSender();
  
  API.message(sender, "¡Hola!"); 
}); 
```

