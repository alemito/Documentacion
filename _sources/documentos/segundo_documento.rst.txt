Ansible
=======

============
Introduccion
============


**Codigo de Ansible**

.. ansible-task::

   - name: foo bar
     command: ls /tmp/foo/BAR




=======
Modulos
=======

=============
Condicionales
=============

.. ansible-task::

    - name: EJEMPLO USO DE INSTRUCCIONES
      set_fact:
        admin: 'alejandro'

    - debug:
        msg:
         - "{% if admin == 'adrian' %}
            Bienvenido admin {{admin}}
            {% else %} 
            No cuentas con los permisos suficientes 
            {% endif %}"  
