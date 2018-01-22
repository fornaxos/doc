Método ``core``
---------------

Con este método se puede invocar a las clases del core, automáticamente el sistema verificará si la clase ya fue cargada y en caso contrario la cargará. Ejemplo de llamada al método:

.. code-block:: php

  <?php
    $fnos->core("route")->getURL();
  ?>

A continuación se muestran todas las clases disponibles en el core.

+-------+------------------------------+
| Clase | Descripción                  |
+=======+==============================+
| route | Gestión de rutas del sistema |
+-------+------------------------------+
