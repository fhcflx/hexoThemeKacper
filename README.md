# hexoThemeKacper-pt-br

Traduzi o tema hexoThemeKacper, originalmente em inglês e mandarim. Abaixo começa o texto original traduzido.

Este é um tema hexo.io, como eu sou naturalmente preguiçoso, baseei-me no tema `landscape`, então ...

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
  Github: https://github.com/<seu repo>

rss: /atom.xml #rss padrão

#feed:
#  type: atom       #feed (atom/rss2)
#  path: /atom.xml   #rss 
#  limit: 20        #limite máximo de postagens reproduzidas (0 mostra todas)


#icon http://fontawesome.io/
#首页显示
article_index:
  -  title: 低廉学习成本低
     content: 与jQuery有着类似的api，模仿jQuery的语法规范，并不是100%的覆盖。如果你会用jQuery，那么你也会用JSLite。
     icon: icon-book
  -  title: 快执行并下载
     content: JSLite通用库只有5-10k，没有大量的兼容代码，在先进浏览器里面跑起来没有负担。为了减小代码量，提高性能，组件再插件化，兼容iOS3+ / android2.1+。
     icon: icon-bolt
  -  title: 为未来web做打算
     content: 让中国再次和世界同步，拥抱现代浏览器。未来总会接触到移动端开发，还好移动端开发环境还不算恶劣。
     icon: icon-lab
  -  title: Github # Github这里比较特殊
     content: JSLite/JSLite # github 仓库地址，例如https://github.com/jaywcjlove/hexoThemeKacper 这里就填写  jaywcjlove/hexoThemeKacper
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
