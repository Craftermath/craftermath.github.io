---
layout: post
title: "Terminal Amigo"
date: 2022-03-30 21:25:06
tags: linux terminal todo_dia
description: Terminal colorido, scripts e alias divertidos.
translation:
---

Vou aproveitar que está uma noite chuvosa (e estou esperando boas notícias) pra contar do meu terminal colorido e alguns scripts felizes que ajudam o fluxo no começo do dia.   

Vai aqui um print do colorido:   

![Terminal colorido, Meu fedora](/assets/images/arcoiris.png)   
 
Instalei esse [toilet](http://caca.zoy.org/wiki/toilet) com esse comando aqui:   
```bash
sudo dnf install toilet
```    
Não uso isso pra todos os comandos mas pra coisas como atualizar o sistema, como nesse print:   

![Oi colorido, Meu fedora](/assets/images/arcoiris2.png)   

Esse "oi" era um alias que morava no meu arquivo .bashrc, adicionei abaixo das linhas que já estavam lá:

```bash
alias oi='sudo dnf update -y | toilet -f term --gay'
```    

Quando comecei a aprender mais sobre scripts bash, tirei essa linha e fiz um arquivo "oi" como no print e adicionei a seguinte linha pelo terminal:   

```bash
PATH=$PATH:/home/usuarie/diretório
```  

Que no caso aqui era   
```bash
PATH=$PATH:/home/fadora/Meus
```  

Só cuide para fazer só uma vez porque vai adicionar cada vez que rodar o comando e fui ver aqui tava assim    

export PATH="/home/fadora/Meus:/home/fadora/Meus:/home/fadora/Meus"   

Por que será néam?  :P  

Mas voltando pro print do arquivo "oi":   

![oi, Meus](/assets/images/ois.png)

Outro arquivinho que gostei de fazer mas não uso muito é o "socorro", principalmente porque não lembro mas vou colar o print pra inspirar literal e metaforicamente:   

![Socorro, Meus](/assets/images/socorro.png)   

E outro um pouco mais útil:    

![Processos, Meus](/assets/images/processos.png)   

Que serve pra ver quantos ~~pensamentos o computador está tendo~~ processos estão acontecendo.   

E por falar em pensamentos do computador, uma vez me mostraram um tuite que as pessoas trocavam o "sudo" pelo alias "please". Como dizia no tuite, se houver a revolução das máquinas, acho que elas vão ser legais comigo porque sempre peço por favor :D  
 
Assim se quiser fazer isso a linha pra adicionar no .bashrc é:   
```bash
alias please='sudo'
```  
Um outro alias que gosto é o "vai":   
```bash
alias vai='cd Diretório/do.projeto.que/estou/trabalhando/ && git status'
```  
   
Assim que ligo o computador costumo mandar um "oi" e depois um "vai" pra ver onde parei no dia anterior e seguir no fluxo. Esse "vai" já deixa tudo pronto pra um "gvim" que vai ser assunto de outro post algum dia.   

Brincadeiras a parte, espero que tenham gostado desses truques de  terminal.   

Há braços,   
Carol


