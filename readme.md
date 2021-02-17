# Estudo do funcionamento do HOST da vercel

Este estudo tem o intuito de entender as entranhas do host da vercel, por ser uma hospedagem de altíssima disponibilidade
além de tudo é uma ferramenta gratuita, onde podemos colocar projetos no ar com a maior facilidade.

Todas as anotações ao longo do estudo serão adicionadas aqui neste arquivo, para que fique registrado no tempo as descobertas.

---

Criando um novo projeto na vercel, e importando o repositório do github
Super simples, apenas criar em new, e selecionar qual repositório do github gostaria de aplicar

Automaticamente ele irá fazer deploy e em poucos segundos o seu projeto está no ar.

---

Vou começar meus estudos criando um singelo arquivo HTML na raiz do meu projeto e vou fazer meu commit pra branch master.

---

Funciona perfeitamente, em poucos segundos temos uma página HTML hosteada pela vercel, com altíssima disponibilidade, e 
é incrível como o carregamento se da de forma quase instantanea.

Agora irei criar um segundo arquivo, para ver qual o comportamento de rotas e novas páginas. Porque a estrutura que o Next JS
usa é criar umas pasta pages/ e qualquer arquivo dentro desta pasta se torna uma "rota" porém não estamos utilizando o next
apenas o servido da vercel que é otimizado para o next.

---