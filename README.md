# hexoThemeKacper-pt-br

> Traduzi o tema [hexoThemeKacper](https://github.com/jaywcjlove/hexoThemeKacper), originalmente em inglês e mandarim. Abaixo começa o texto original traduzido, com algumas substituições por conteúdo meu.

Este é um tema hexo.io. Naturalmente,como eu sou  preguiçoso, baseei-me no tema `landscape`, então ...

## Pré-visualização

[Banco de dados de pacientes com tumores cerebrais](https://neuro-oncologia.gitlab.io/banco/)

## Instalação

### Instalar

``` bash
$ git clone https://github.com/fhcflx/hexoThemeKacper.git themes/hexoThemeKacper-pt-br
```

**hexoThemeKacper-pt-br requer Hexo 3.0 ou acima.**


### Atualizar

``` bash
cd themes/hexoThemeKacper-pt-br
git pull
```

### Permissões

Modifique a configuração `theme` em `_config.yml` para `hexoThemeKacper-pt-br`.

## Uso

### Exemplo de configuração do tema

Edite o `_config.yml`

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



# Conteúdo
excerpt_link: Leia mais
fancybox: true  #Ativar abertura de fancybox


# Miscelânea #Redes sociais, estatísticas de conexão, etc
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

## Licença
[MIT](/MIT-LICENSE)
