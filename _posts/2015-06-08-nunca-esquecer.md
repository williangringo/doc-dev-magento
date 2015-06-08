---
layout: page
title: "-"
category: nunca-esquecer
date: 2015-06-08 19:43:23
---

Nunca fazer rollback no deploy de um módulo instalado, porem, se realmente for
necessário podemos seguir os passos:

* Conectar por ssh no servidor
* Editar o arquivo `app/etc/modules/$nomedomodulo.xml` e trocar a tag `<active>true</active>` para `<active>false</active>`
* Limpar o cache
* Agora o módulo está desativado e os arquivos dele podem ser removidos

