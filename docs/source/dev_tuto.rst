Tutoriels
=========

**ESX 1.7.5**
-------------

Optimisation SharedObject
^^^^^^^^^^^^^^^^^^^^^^^^^

ESX 1.7.5 a simplifié l'utilisation du framework et le partage des objets partagés.

Dorénavant, l'appel à l'event pour obtenir les objets partagés n'est plus nécessaire, 
vous devez dorénavent préciser le fichier d'import d'ESX dans le ``fxmanifest.lua`` de votre ressource.

.. code-block:: lua

    client_scripts {
        '@es_extended/imports.lua',
    }

    server_scripts {
        '@es_extended/imports.lua',
    }

Grâce à cet import et aux nouvelles fonctionalités d'ESX, vous n'avez plus besoin des écoutes d'event au ``setJob`` ou au ``playerLoaded``. 
De plus, le ``ESX.PlayerData`` s'actualise automatiquement à chaque changement de valeur. L'utilisation d'un ``ESX.GetPlayerData()`` n'est plus nécessaire.

**RageUI**
----------