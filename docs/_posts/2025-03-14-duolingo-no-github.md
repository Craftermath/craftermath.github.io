---
layout: post
title: "Duolingo no Github"
date: 2025-03-14 00:35:09
tags: comportamento dados diversão nerdisse todo_dia 
description: Um post de pi day.
translation:
---

Sou dessas pessoas que adora aprender tudo. Fazer as coisas, como o mundo funciona, idiomas... Mas como tudo é muita coisa, tem que ser uma coisa de cada vez. Se o assunto é longo tem que ser um pouquinho cada dia e assim chegamos no [duolingo](https://www.duolingo.com/profile/Caoticarol).   

E em aprender a usar o github actions pra colocar essa firula de duolingo lá no perfil do [github](https://github.com/Craftermath).   

Primeiro tem que ter uma conta no duolingo e uma conta no github e fazer um repositório com seu nome de usuárie no nome do repositório. Por exemplo o meu é `https://github.com/Craftermath/Craftermath`   

Aí tem que criar esse arquivo `README.md` que você pode escrever o que quer que apareça no seu perfil. E no lugar que é pra aparecer a tabela do duolingo você escreve a tag ```<!-- duolingo -->``` assim:

```
#README.md

Olá! Meu nome é ...                  #essa linha é opcional
Outras infos...                      #essa linha é opcional

<!-- duolingo -->

_made with [Craftermath/duolingo-to-markdown](https://github.com/Craftermath/duolingo-to-markdown)_   #essa linha é opcional

```

O próximo passo é criar o Github Secret chamado ```DUOLINGO_USERNAME``` com seu nome de usuário do duolingo. Pra isso você vai na aba Settings (ou configurações) dentro do seu repositório com seu nome (aba mais a direita), vai abrir uma coluna a esquerda e você clica em `Secrets and variables` e depois em `Actions`. Vai aparecer um botão do lado direito `New repository secret` e ~~segue toda vida reto~~ é só por ```DUOLINGO_USERNAME``` no `Name` e seu nome de usuárie do Duolingo no `Secret`. Isso foi feito assim porque na API antida do duolingo a gente usava a senha também e pq a gente gosta de organização.  Mas se não quiser fazer esse passo e gostar de gambiarra é só procurar nos dois arquivos dos próximos passos a expressão ```DUOLINGO_USERNAME``` e substituir por seu nome de usuárie.   

Depois copie e cole o arquivo ```duolingo-to-markdown.yml``` que pode pegar no [meu perfil](https://github.com/Craftermath/Craftermath/blob/main/.github/workflows/duolingo-to-markdown.yml) ou no [perfil do exemplo](https://github.com/Craftermath/duolingo-to-markdown/blob/main/.github/workflows/dailyduo.yml) para o seu diretório ```SeuUsuarie/.github/workflows```. Observe que `SeuUsuarie` deve ser seu nome de usuárie do github. Se não tiver o diretório `workflows` você tem que criar dentro do `.github`. Já aproveita pra criar o diretório `scripts` também dentro do `.github` que usaremos no próximo passo.   

Copie e cole o arquivo ```duolingo-to-markdown.py``` do [meu perfil](https://github.com/Craftermath/Craftermath/tree/main/.github/scripts) ou [do exemplo](https://github.com/Craftermath/duolingo-to-markdown/blob/main/duolingo-to-markdown.py) para dentro do diretório ```.github/scripts``` criado no passo anterior.

Depois disso você pode ir na aba ```Actions``` e procurar no lado esquerdo da tela os workflows e clicar no ```dailyduo```. No lado direito da tela vai aparecer um botão dizendo `Run workflow` e é só clicar pra ver a magia acontecer.  

Se gostou da brincadeira deixe uma estrelinha lá no https://github.com/Craftermath/duolingo-to-markdown 

Há braços!

#PiDay   
#sextou



