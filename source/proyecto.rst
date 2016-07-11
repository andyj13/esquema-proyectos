El proyecto
===========

Descripción General
-------------------

El software debe cumplir las funciones de poder registrar a cualquier
artista que necesite darse a conocer, este tendrá que llenar una serie
de campos con su información para que la casa de la cultura pueda
contactarlo y así poder autorizar su perfil.

Además de llevar el control de los artistas, también se tiene que llevar
el control de los eventos que realice tanto la misma institución como
eventos organizados por los artistas, siempre y cuando estén previamente
autorizados por la Casa de la cultura.

Con base a la información reunida de los artistas y eventos el sistema
tiene que ser capaz de generar estadísticas, esta información disponible
principalmente para el gerente de cultura y para algún tercero que
necesite de las estadísticas pero este requerirá de una solicitud
anticipada.

También tiene que existir una sección donde se pueda agregar información
cultural sobre el municipio, es decir, descripciones a cerca de fechas
importantes cercanas, como la feria de Xela, o a cerca de lugares o
monumentos, ejemplo, el teatro municipal o el monumento de la marimba.

Modulos
^^^^^^^

#. Artistas:
    Ver diagrama de casos de uso :ref:`artistas-label`.

    Este módulo contempla primeramente la forma de registro de un artista,
    para poder registrarse deberá llenar un formulario con su información,
    para que la Casa de la cultura pueda contactarlo y así corroborar que
    su información sea verídica y confirmar el perfil; una vez autorizado
    el perfil, un artista puede:

      * Editar su información.
      * Crear eventos.
      * Cambiar su contraseña.

    Y para cualquier usuario tendrá las siguientes opciones:

      * Buscar artista.
      * Ver artistas por categoría.
      * Ver información de artistas.

#. Eventos:
    Ver diagrama de casos de uso :ref:`eventos-label`.

    Los eventos pueden ser creados tanto por los artistas como por la propia
    Casa de la cultura, en caso que un artista quiera crear un evento, deberá
    llenar un formulario con la información del evento a realizar y un administrador
    confirmará o no el evento, si en dado caso el artista necesitara
    de algún lugar para realizar la actividad como el teatro u otra institución
    relacionada con la Casa de la cultura, igualmente se confirmará si está
    disponible para su uso.
    Este módulo contará con las siguientes funciones:

      * Crear evento, en caso exclusivo de artistas y administradores.
      * Ver eventos existentes.
      * Buscar eventos.
      * Ver eventos por categorías.

#. Cápsulas informativas:
    Ver diagrama de casos de uso :ref:`capsulas-label`.

    El software tendrá un módulo donde se tenga información sobre fechas
    importantes, actividades, lugares, monumentos, etc., todo referente a la
    cultura del municipio de Quetzaltenango estas estarán disponibles para el
    público en general que quiera visualizarla, esta información será
    manipulada solamente por los adminstradores del sitio, tanto para crearlas,
    editarlas o eliminar alguna cápsula.

#. Administrativo:
    Ver diagrama de casos de uso :ref:`admin-label`.

    Este incluye opciones que no estarán disponibles para los artistas ni por
    los visitantes, tales opciones son:

      * Confirmar artista y eventos.
      * Eliminar artistas o eventos.
      * Crear, editar, eliminar cápsulas informativas.
      * Acceder a las estadísticas.

    Las estadísticas, siendo un sub módulo de este, tendrán las siguientes
    opciones:

      * Ver eventos más populares.
      * Censos de artistas (cuántos artistas hay en cada categoría).
      * Actualizar las estadísticas.
