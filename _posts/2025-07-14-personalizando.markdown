---
layout: post
title:  "Personalización do modelo"
date:   2025-07-14 13:34:06 +0200
categories: post
tags:
  - updates
  - website
---
Neste momento estou en tarefas de personalización do modelo.

Como xa vos contaba [na mensaxe anterior]({% post_url 2025-07-11-nova_version %}), estou usando [Jekyll][jekyll] para a nova versión desta web, e atendendo ao principio [KISS](https://pt.wikipedia.org/wiki/Princ%C3%ADpio_KISS), mantiven o modelo [`minima`][minima], que é o que se aplica de xeito predeterminado nos proxectos novos.

Porén, a versión do modelo `minima` que estou a usar neste momento é a 2.5, e semella estar en desenvolvemento a versión 3, que podería traer cambios non retrocompatibles. Así as cousas, tratarei de non mudar moitos detalles, polo risco de que non se poidan conservar eses axustes cando a versión se actualice.

Polo de agora, estas modificacións afectan a:

- Engadir contido ao ficheiro `index.markdown` para humanizar a páxina principal.
- Modificar o _layout_ `home` para usar o _include_ `post_preview` e axustar así a estética do resumo de novidades.
- Engadir varias páxinas adicionais ([divulgación](/divulgacion), [proxectos](/proxectos), [publicacións](/publicacions), [docencia](/docencia)).
- Engadir unha [páxina de arquivo](/archives/index).
- Modificar o _layout_ `post` para axustar a estética de páxinas coma esta.

[jekyll]: https://jekyllrb.com/docs/home
[minima]: https://github.com/jekyll/minima

