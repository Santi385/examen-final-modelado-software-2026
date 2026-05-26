# Parte 2: Caso de Uso

**ID:**  CU_01
**Nombre:**Guardar articulo para ver despues

**Actor Principal:** Usuario Registrado
**Actores Secundarios:** Sistema

## Descripcion 
Permite a un usuario registrado guardar un artículo en una lista personal de lectura para poder acceder a él posteriormente desde su perfil.

## Precondiciones
El usuario debe haber iniciado sesión.
El artículo debe existir en el sistema.
El usuario debe tener una cuenta registrada
-

## Flujo Principal

1.El usuario inicia sesión en el sistema.
2.El usuario accede a un artículo.
3.El usuario selecciona la opción "Guardar para leer después".
4.El sistema verifica que el usuario esté autenticado.
5.El sistema verifica que el artículo no esté guardado previamente.
6.El sistema agrega el artículo a la lista personal de lectura del usuario.
7.El sistema va a mostrar un mensaje confirmando que el artículo fue guardado correctamente.

## Flujos Alternativos
FA1: Usuario no autenticado
El usuario intenta guardar un artículo.
El sistema detecta que no ha iniciado sesión.
El sistema solicita iniciar sesión o registrarse.
El caso de uso finaliza.

FA2: Artículo ya guardado
El usuario intenta guardar un artículo.
El sistema detecta que el artículo ya existe en la lista de lectura.
El sistema informa que el artículo ya fue guardado.
El caso de uso finaliza.

## Postcondiciones

-
El artículo queda almacenado en la lista de lectura del usuario.
El usuario puede visualizar el artículo desde su perfil posteriormente.


Caso de Uso Completo

ID: CU-2
Nombre: Compartir artículo por enlace

Actor principal: Usuario / Visitante

Actores secundarios: Sistema

Descripción:
Permite a usuarios registrados y visitantes compartir un artículo mediante un enlace público. El sistema registra cada acción de compartir y actualiza un contador visible.

Precondiciones:

El artículo debe existir.
El artículo debe estar publicado.
El enlace público debe estar disponible.

Flujo principal:

El usuario abre un artículo.
El sistema muestra la opción "Compartir".
El usuario selecciona "Compartir artículo".
El sistema genera o recupera el enlace público.
El sistema incrementa el contador de compartidos.
El sistema copia o muestra el enlace.
El sistema actualiza el contador visible.
El usuario comparte el enlace.

Flujos alternativos:

FA1: Error al generar enlace

El sistema intenta generar el enlace.
Ocurre un error.
El sistema muestra mensaje: "No se pudo generar el enlace".

FA2: Artículo no disponible

El usuario intenta compartir.
El artículo no está publicado.
El sistema muestra mensaje: "Artículo no disponible para compartir".

Postcondiciones:

El enlace público queda disponible.
El contador de compartidos se actualiza.
La acción queda registrada.
