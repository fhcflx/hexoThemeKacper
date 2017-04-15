# hexoThemeKacper-pt-br

Traduzi o tema hexoThemeKacper, originalmente em inglês e mandarim. Abaixo começa o texto original traduzido.

Este é um tema hexo.io. Naturalmente,como eu sou  preguiçoso, baseei-me no tema `landscape`, então ...

## Pré-visualização

[Banco de dados de pacientes com tumores cerebrais](https://neuro-oncologia.gitlab.io/banco/)

## Instalação

### Instalar

``` bash
$ git clone https://github.com/jaywcjlove/hexoThemeKacper.git themes/hexoThemeKacper
```

**hexoThemeKacper requires Hexo 3.0 and above.**


### Atualizar

``` bash
cd themes/hexoThemeKacper
git pull
```

### Permitir

Modifique a configuração `theme` em `_config.yml` para `hexoThemeKacper`.

## Uso

### Exemplo de configuração do tema

`/themes/_config.yml` Explicando

```python
# Header
menu: #barra de navegação
  Home: /  
  PDF: /PDF
  Tags: /tags
  # Category: /category
  Arquivos: /archives #/arquivos #Personalização do título da página e da URL
  Sobre: /about
  Github: https://github.com/fhcflx/cpc-neuro

rss: /atom.xml #rss padrão

#feed:
#  type: atom       #feed (atom/rss2)
#  path: /atom.xml   #rss 
#  limit: 20        #limite máximo de postagens reproduzidas (0 mostra todas)


#icon http://fontawesome.io/
#Mostrando conteúdo na página principal
article_index:
  -  title: Protocolos de Tratamento
     content: Manual de protocolos de quimioterapia usados no tratamento de pacientes com tumores cerebrais.
     icon: icon-book
  -  title: Equipe do GPMCP
     content: Juvenia B Fontenele，Francisco H C Felix
     icon: icon-bolt
  -  title: Banco de dados
     content: Relatórios dinâmicos do banco de dados de pacientes com tumores cerebrais
     icon: icon-lab
  -  title: Github # Suas estatísticas Github
     content: fhcflx/cpc-neuro # repositório github
     icon: icon-github-alt



# Content
excerpt_link: Read More  #阅读更多的文字显示
fancybox: true  #开启fancybox效果


# Miscellaneous #社交网络和统计连接地址
favicon: /css/favicon.ico
logo: /css/logo.png
```


### TAGS && Category && API && About

设置这三个菜单需要你在 `source` 建立三个页面

```
source/tags/index.md
source/category/index.md
source/API/index.md
source/about/index.md
```


#### tags

```
layout: tags
title: "tags"
---
```


#### Category

```
layout: category
title: "categories"
---
```

#### API

```
title: "JSLite.io"
date: 2015-04-05 05:37:40
type: "API"
---
```

#### About

```
title: "关于我"
date: 2015-04-02 01:36:59
description: "关于我"
type: "about"
---

前端开发工程师。敏捷实践者。目前就职于hotpu，生活在上海。

<!--more-->
```


### 注意翻页

因为本主题没有做翻页的功能。所以在博客跟目录 `_config.yml` 文件中要设置 `per_page: 0` ，设置为 `0` 显示所有文章

```
per_page: 0
pagination_dir: page
```

### 多说评论

注册你自己的多说账号 [duoshuo](http://dev.duoshuo.com/docs/501e6ce1cff715f71800000d) 替换你在根目录`_config.yml` 中的 `duoshuo short_name` 的值，没有在里面设置

```
duoshuo_shortname: your short_name
```


## 协议
[MIT](/MIT-LICENSE)
