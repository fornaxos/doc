Estructura de Ficheros
=======================

Se ha organizado los archivos y carpetas para que sean fáciles de entender y usar. A continuación se muestra la estructura de ficheros del proyecto:

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

.. code-block:: text

    <nombre-plugin>/
    ├ class/
    ├ assets/
    │ ├ css/
    │ ├ js/
    │ └ images/
    ├ view/
    └ router.php
