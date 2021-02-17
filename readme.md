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

Acessando https://estudo-vercel-host.vercel.app/sobre temos o error 404: NOT_FOUND

Acessando https://estudo-vercel-host.vercel.app/sobre.html temos o error 404: NOT_FOUND

Vou criar uma pasta pages/ e colocar meus dois arquivos html dentro pra ver se as configurações do next são implementadas aqui

---

Funciona ao acessar os links

https://estudo-vercel-host.vercel.app/pages/about.html

https://estudo-vercel-host.vercel.app/pages

Ou seja, no teste anterior eu digitei o nome do arquivo errado, por isso tivemos um error 404

Vemos então que zero config é possível colocar um site no ar, mas pra utilizar o conceito de rotas e estruturação você vai precisar
utilizar as funções serverless da vercel

Criei uma nova page chamada views, coloquei meus dois arquivos html nela, e agora vou tentar utilizar algumas funções serverless da vercel

para isso vou criar um arquivo index.js na pasta pages/

---

