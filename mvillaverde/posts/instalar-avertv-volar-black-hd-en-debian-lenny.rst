.. title: Instalar Avertv Volar Black HD en debian lenny
.. slug: instalar-avertv-volar-black-hd-en-debian-lenny
.. date: 2009-12-19 22:52:45 UTC+01:00
.. tags: Linux, Tdt, Dvb
.. category: Administración de sistemas
.. link:
.. description:
.. type: text

.. image:: /imgpost/avermedia_a850_dvb-t-stick.jpg

Me compre una AverTV Volar Back HD, ya que necesitaba una sintonizadora usb para el servidor que no tiene ranuras pci.

En debian lenny al traer un kernel  2.6.26 no tenemos soporte para esta sintonizadora y tendremos que descargarnos los drivers y compilarlos.

Necesitamos que estén instalados mercurial, dvb-utils y los headers del kernel. Cualquiera de estas cosas las podemos instalar con apt.

Una vez que tenemos todo lo necesario nos descargamos las fuentes del driver con:

.. code-block:: shell

  hg clone http://linuxtv.org/hg/v4l-dvb

entramos dentro del directorio

.. code-block:: shell

  cd v4l-dvb

compilamos

.. code-block:: shell

  make

instalamos

.. code-block:: shell

  make install

Ahora solo nos queda descargar el firmware desde `aqui <http://dl.getdropbox.com/u/971641/UbuntuBlog/dvb-usb-af9015.fw/>`_

y lo guardamos en /lib/firmware. Con esto ya tenemos finalizado la instalacion. Solo nos queda enchufar la sintonizadra e instalar un programa para ver la tv como kaffeine si aun no lo teneis instalado
