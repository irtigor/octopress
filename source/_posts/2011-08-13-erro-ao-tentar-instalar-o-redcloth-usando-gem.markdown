---
layout: post
title: "Erro Ao Tentar Instalar O RedCloth Usando Gem"
date: 2011-08-13 22:10
comments: true
categories: [ruby, gem, RedCloth, gcc]
---

Precisei instalar o modulo RedCloth, é uma dependência do [octopress][1], o problema é que ele usa a cflag Werror pra tratar alertas como erro... cortando o lero-lero: 

` gem install RedCloth -- --with-cflags=\"-O2 -pipe -march=native -Wno-unused-but-set-variable\" `

Fonte: [http://stackoverflow.com/questions/6761670/is-there-any-way-to-change-gcc-compilation-options-for-a-gem][2]

[1]: http://octopress.org "octopress"
[2]: http://stackoverflow.com/questions/6761670/is-there-any-way-to-change-gcc-compilation-options-for-a-gem "stackoverflow"
