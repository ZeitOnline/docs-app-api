=====================
Entwickler-Onboarding
=====================

API-Dokumentation
=================

Die API-Dokumentation wird als OpenAPI-Spezifikation in ``api.yaml`` gepflegt,
und mit dem swagger-ui HTML/JS daraus direkt angezeigt.

Wegen CORS&Co muss man lokal immer ``bin/docs serve`` verwenden.


API validieren
==============

Mit ``bin/test`` kann man die ``api.yaml`` auf syntaktische Korrektheit mit dem OpenAPI-Standard überprüfen.


Backend
=======

Zappis Backend findet sich in zeit.web.app, dort ist das Zappi Repo als Submodule eingebunden. 

.. note::
    Das führt mitunter zu Mergekonflikten, wenn verschiedene Versionen des Submodules kollidieren. Hier hilft in vielen Fällen ``git submodule update --init --recursive`` um das Submodul auf den gegenwärtigen Stand (des Masters) zu bringen.
