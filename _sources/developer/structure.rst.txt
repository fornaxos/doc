Estructura de Ficheros
=======================

Se han organizado los archivos y carpetas para que sean fáciles de entender y usar. A continuación se muestra la estructura de ficheros del proyecto:

.. code-block:: text

    fornaxos/
    ├ fnos-config/
    │ └ config.php
    ├ fnos-content/
    │ ├ data/
    │ ├ plugins/
    │ └ themes/
    ├ fnos-core/
    │ ├ class/
    │ ├ js/
    │ ├ fnos.class.php
    │ └ index.php
    └ index.php

Veamos más de cerca cada directorio y archivo, y comprendamos cómo funciona.

* ``fnos-config/`` : Contiene la configuración necesaria para el funcionamiento de la plataforma (base de datos, site, etc).
* ``fnos-content/data`` : Aquí se almacenará todos los ficheros que sean subidos desde la plataforma (imágenes, documentos, etc).
* ``fnos-content/plugins`` : Aquí se alojan todos los módulos instalados en el sistema.
* ``fnos-content/themes/`` : Aquí se alojan todos los temas visuales disponibles para la plataforma.
* ``fnos-core/`` : Contiene todo el núcleo del sistema.

Estructura de los Plugins
--------------------------

La estructura de los plugins se ha organizado de forma que el desarrollo sea lo mas limpio posible, para ello se propone la siguiente jerarquía:

.. code-block:: text

    <nombre-plugin>/
    ├ class/
    ├ assets/
    │ ├ css/
    │ ├ js/
    │ └ images/
    ├ view/
    └ router.php

* ``class/`` : Aquí se alojaran todas las clases necesarias para el plugin. El nombre debe ser el siguiente: <nombre-clase>.class.php
* ``assets/`` : Se alojaran todos los ficheros estáticos (css, javascript, imágenes y fuentes).
* ``view/`` : Aquí se alojaran las vistas necesarias de el plugin.
* ``router.php`` : Fichero de control del plugin.
