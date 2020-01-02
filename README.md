# hexoThemeKacper-pt-br

> Traduzi o tema [hexoThemeKacper](https://github.com/jaywcjlove/hexoThemeKacper), originalmente em inglês e mandarim. Abaixo começa o texto original traduzido, com algumas substituições por conteúdo meu.

Este é um tema hexo.io. Naturalmente, como eu sou  preguiçoso, baseei-me no tema `landscape`, então ...

## Pré-visualização

[Banco de dados de pacientes com tumores cerebrais](https://neuro-oncologia.gitlab.io/banco/)

## Instalação

### Instalar

``` bash
$ git clone https://github.com/fhcflx/hexoThemeKacper-pt-br.git themes/hexoThemeKacper-pt-br
```

**hexoThemeKacper-pt-br requer Hexo 3.0 ou acima.**


### Atualizar

``` bash
cd themes/hexoThemeKacper-pt-br
git pull
```

### Configuração básica

Modifique a configuração `theme` em `_config.yml` para `hexoThemeKacper-pt-br`.

## Uso

### Exemplo de configuração do tema

Edite o `_config.yml`

```python
# Configuração do Hexo
## Docs: https://hexo.io/docs/configuration.html
## Source: https://github.com/hexojs/hexo/

# Página principal
title: Pediatric CNS tumor databank
subtitle: Single-center hospital-based registry data
description: Hospital registry data of central nervous system tumors in children and adolescents
author: Francisco Felix
language: en
timezone: America/Fortaleza
banner: "https://gitlab.com/neuro-oncologia/banco/source/css/images/banner.jpg"

# URL
## If your site is put in a subdirectory, set url as 'http://yoursite.com/child' and root as '/child/'
url: https://neuro-oncologia.gitlab.io/banco
root: /banco
permalink: :year/:month/:day/:title/
permalink_defaults:

# Diretórios
source_dir: source
public_dir: public
tag_dir: tags
archive_dir: archive
category_dir: categories
code_dir: downloads/code
i18n_dir: lang
skip_render:

# Postando
new_post_name: :title.md # nome de arquivo de novas postagens
default_layout: post
titlecase: false # transforma os títulos em "titlecase"
external_link: true # Abre ligações em novas abas
filename_case: 0
render_drafts: false
post_asset_folder: false
relative_link: false
future: true
highlight:
  enable: true
  line_number: true
  auto_detect: false
  tab_replace:

# Categoria & Tags
default_category: cns_tumor
category_map:
tag_map:

# Formato de data e hora
## Hexo usa Moment.js para codificar e publicar datas
## Você pode personalizar a definição de data e hora
## http://momentjs.com/docs/#/displaying/format/
date_format: YYYY-MM-DD
time_format: HH:mm:ss

# Paginação
## Deixe per_page: 0 para desabilitar a paginação
per_page: 0
pagination_dir: page

# Extensões
## Plugins: https://hexo.io/plugins/
# plugins:
# - hexo-generator-sitemap
## Themes: https://hexo.io/themes/
theme:
- hexoThemeKacper-pt-br

# Deployment
## Docs: https://hexo.io/docs/deployment.html
deploy:
  type:

# Header
menu:
  Main: /
  Reports: /report
  #Tumors: /tiposd
  #Treatment: /tipost
  Tags: /tags
  Category: /categories
  Archive: /archive
  About: /about
  Manual: https://github.com/fhcflx/cpc-neuro

rss: /atom.xml

#feed:
#  type: atom       #feed (atom/rss2)
#  path: /atom.xml   #rss
#  limit: 20        #limite máximo de postagens reproduzidas (0 mostra todas)


#icon http://fontawesome.io/

article_index:
  -  title: Databank
     content: Information about children and adolescents treated for central nervous system tumors in a specialized center in Brazil. Approved by IRB.
     url: https://neuro-oncologia.gitlab.io/banco/about
     icon: icon-book
  -  title: Reports
     url: https://neuro-oncologia.gitlab.io/banco/report
     content: Results of the treatment of neoplastic diseases included in the database, as well as epidemiology and information on prognostic factors.
     icon: icon-bolt
  -  title: The team
     content: Juvenia B Fontenele，Francisco H C Felix
     url: https://scholar.google.com.br/citations?user=l4gNn7AAAAAJ&hl=pt-BR&oi=ao
     icon: icon-lab
  -  title: Gitlab
     content: neuro-oncologia/banco
     color: darkgreen
     url: https://doi.org/10.5281/zenodo.3576056
     img: https://img.shields.io/badge/DOI-10.5281/zenodo.3576056-darkgreen
     icon: icon-gitlab

# Conteúdo
excerpt_link: Read more
# fancybox: false

# Miscelânea
favicon: /css/favicon.ico
logo: /css/logo.png
```

### TAGS && Categoria && Sobre

Os menus fixos exigem páginas individuais em `source`

```
source/tags/index.md
source/category/index.md
source/about/index.md
```


#### tags

```
layout: tags
title: "tags"
---
```


#### Categoria

```
layout: category
title: "categorias"
---
```


#### Sobre

```
title: "Sobre mim"
date: 2017-04-12 01:36:59
description: "sobre mim"
type: "about"
---

Médico, cientista, fazendo experimentos com radiação nerd, ele sofreu mutações que o transformaram em...

<!--more-->
```


### Paginação

Como neste tema não fiz função flip, então no `_config.yml` a configuração é ` per_page: 0`,` 0` está configurado para exibir todos os artigos.

```
per_page: 0
pagination_dir: page
```

### Comentários

> Os comentários estavam configurados, no original, para o [duoshuo](https://dev/duoshuo.com), um sistema de comentários para redes sociais em mandarim.

### Mudanças em relação ao original:
- Hiperlinks no índice
- Gitlab no lugar do Github
- Atualização do Fontawesome para versão 4.7
- Página de relatórios
- Badges

## Licença
[MIT](/MIT-LICENSE), originalmente para [@jaywcjlove](https://github.com/jaywcjlove), tradução para o português minha.
