# Laboratorio OverTheWire Natas 1

## Objetivo
El objetivo de este nivel es encontrar la contraseña para poder acceder al siguiente, **natas2**.

## Acceso al nivel
Para entrar encontramos la credencial en el nivel anterior natas0:  

```
Username: natas1
Password: 0nzCigAq7t2iALyvU9xcHlYN4MlkIwlq
URL: http://natas1.natas.labs.overthewire.org/
```

Ingresé en la página usando esos datos y al cargar me salió un mensaje que decía:  
> "_Puedes encontrar la contraseña para el siguiente nivel en esta página, ¡pero hacer clic derecho está bloqueado!_"

![alt text](/overthewire/natas1/image.png)

## Mi proceso paso a paso

Al igual que el anterior laboratorio pense que las credenciales podrian estar en el codigo fuente, pero esta vez no podia usar el '_click derecho_' ya que estaba bloqueado. Lo que hice fue usar **Ctrl+U** para ver la fuente completa de la página.

Al revisar el código, encontré un comentario que contenía la contraseña de `natas2`.  
   
El comentario se veía así:  
```html
<!--The password for natas2 is TguMNxKo1DSa1tujBLuZJnDUlCcUAPlI -->
```

![alt text](/overthewire/natas1/image-1.png)


Con esa contraseña podemos continuar y avanzar al siguiente nivel.

## Observaciones 

* En entornos de producción, nunca se deben dejar datos sensibles en el HTML, JavaScript o comentarios.

## Conclusión

Con este laboratorio podemos aprender que mucha información sensible puede estar en el lado del cliente.