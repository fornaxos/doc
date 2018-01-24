route
======

La clase route es la encargada de gestionar las rutas, desde ella podremos definir los enlaces de cada aplicación.

Definición de rutas
-------------------
Para definir las rutas se ha de invocar a la siguiente función en el archivo router.php de la aplicación que se está desarrollando:

.. code-block:: php

  <?php
    $fnos->core('route')->map('settings/users', function() {
      echo "Entro en la función";
    })
    ->view('views/users.php')
    ->conf(['auth' => true, 'theme' => true]);
  ?>

ó

.. code-block:: php

  <?php
    $fnos->core('route')->map('settings/users', settings_users())
    ->view('views/users.php')
    ->conf(['auth' => true, 'theme' => true]);

    function settings_users() {
      echo "Entro en la función";
    }
  ?>

* ``map``: Con esta función mapeamos la ruta y el controller a cargar.
* ``view``: En caso de ser necesaria una vista se definirá agregando la ruta relativa en donde esté ubicada dicha vista.
* ``conf``: Se cargará la configuración deseada para dicha ruta. El formato aceptado es JSON.

# Configuración soportada
--------------------------

+---------------+------------------------------------------------------+-------------+
| Configuración | Descripción                                          | por defecto |
+===============+======================================================+=============+
| auth          | valida la autenticación del usuario                  | false       |
+---------------+------------------------------------------------------+-------------+
| theme         | Define si se ha de cargar el tema visual por defecto | false       |
+---------------+------------------------------------------------------+-------------+
