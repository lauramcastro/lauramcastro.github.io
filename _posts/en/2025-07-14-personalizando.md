---
layout: post
title:  "Template customization"
excerpt: "I am in the process of customizing the website template."
date:   2025-07-14 13:34:06 +0200
permalink: /en/:title/
lang: en
ref: personalizacion
categories: post
tags:
  - updates
  - website
---
At the time of writing this, I am in the process of customizing the website template.

As I mentioned [in the previous post]({% post_url en/2025-07-11-nova_version %}), I am using [Jekyll][jekyll] for the new version of this website and, in doing so, according to the [KISS](https://pt.wikipedia.org/wiki/Princ%C3%ADpio_KISS) principle, I have kept the [`minima`][minima] template,  applied by default in new Jekyll projects.

The version of the `minima` template currently in place is 2.5, but it seems that version 3 is under development, that could bring non-backward-compatible changes. Thus, I am trying not to introduce many tweaks, in light of the risk that they may not be applicable if and when the version is updated.

For now, the changes I've made are:

- Added content to the `index.markdown` file to humanize the main page.
- Modified the `home` _layout_ to use the `post_preview` _include_ to fine-tune the news summary.
- Added several additional pages ([divulgación](/divulgación), [projectos](/projectos), [publicaciones](/publicaciones), [docencia](/docencia)).
- Added an [archive page](/archives/index).
- Modified the `post` _layout_ to fine-tune the aspect of pages like this one.

[jekyll]: https://jekyllrb.com/docs/home
[minima]: https://github.com/jekyll/minima
