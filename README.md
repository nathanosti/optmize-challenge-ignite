# 💻 Sobre o desafio

Nesse desafio você deverá performar uma aplicação React utilizando das ferramentas e dicas aprendidas durante o módulo **Performando apps com ReactJS - Rockeatseat (Ignite)**.
Com essa aplicação componentizada, você deve aplicar os conceitos de performance no React para melhorar esse app.

### Fake API com JSON Server

Nesse desafio vamos utilizar o JSON Server para simular uma API que possui as informações de gêneros e filmes. 

Navegue até a pasta criada, abra no Visual Studio Code e execute os seguintes comandos no terminal:

```bash
yarn # instala as dependências
yarn server # inicia o servidor com o JSON Server na porta 3333
```

Em seguida, você vai ver a mensagem:

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1abc3356-2936-4106-a4fe-a3fc8efd1373/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1abc3356-2936-4106-a4fe-a3fc8efd1373/Untitled.png)

Perceba que ele iniciou uma fake API com os recursos `/genres` e `/movies` em `localhost` na porta `3333` a partir das informações do arquivo [server.json](https://github.com/danilo-vieira/ignite-template-otimizando-a-aplicacao/blob/main/server.json) localizado na raiz do seu projeto. 

Acessando essas rotas no seu navegador, você consegue ver o retorno das informações já em JSON (dando um clique duplo, a imagem se expandirá):

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/12a3c689-264b-4bd4-8515-730dfe8dd407/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/12a3c689-264b-4bd4-8515-730dfe8dd407/Untitled.png)

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/400b84d4-2de4-4cd3-aef2-139f3103e9f6/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/400b84d4-2de4-4cd3-aef2-139f3103e9f6/Untitled.png)

Dessa forma, basta consumir essas rotas da API normalmente com o Axios. 

Caso queira estudar mais sobre o **JSON Server**, dê uma olhada aqui:

[typicode/json-server](https://github.com/typicode/json-server)

## O que devo editar na aplicação?

Com o template já clonado, as dependências instaladas e a fake API rodando, você deve começar implementar as estratégias de otimização para a aplicação.

Aqui estão os dois principais arquivos que devem ser editados:

- **[src/App.tsx](https://github.com/danilo-vieira/ignite-template-otimizando-a-aplicacao/blob/main/src/App.tsx)**
Esse é o componente principal da aplicação e contém toda a lógica da aplicação como chamadas à API e controle de estados dos componentes Content e SideBar.
- **[src/components/Content.tsx](https://github.com/danilo-vieira/ignite-template-otimizando-a-aplicacao/blob/main/src/components/Content.tsx)**
Esse componente, possui toda a lógica e corpo responsável pelo header e conteúdo da aplicação (seção contornada em vermelho):

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ff7c8a12-50d1-4a20-a680-9085d0bd6823/example.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ff7c8a12-50d1-4a20-a680-9085d0bd6823/example.png)

- **[src/components/SideBar.tsx](https://github.com/danilo-vieira/ignite-template-otimizando-a-aplicacao/blob/main/src/components/SideBar.tsx)**
Esse componente possui toda a lógica e corpo responsável pela seção que contém o título do site e a parte de navegação à esquerda da página (seção contornada em vermelho):

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/88f057c2-d29a-4b0d-b9ed-f11385e09030/example.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/88f057c2-d29a-4b0d-b9ed-f11385e09030/example.png)

Se você preferir, pode também componentizar algumas outras partes da aplicação como, por exemplo, o header, mas esse não está como requisito deste desafio 🚀

## Dicas

Lembre-se de usar corretamente as funcionalidades do React para prover mais performance para a aplicação:

memo;

useMemo;

useCallback;

Mesmo que a aplicação não precise de alguns pontos de otimização, sinta-se livre para usar as ferramentas a sua disposição como forma de aprendizado mas continue tomando cuidado com otimizações desnecessárias ao trabalhar com algum projeto real 💜.

## Como deve ficar a aplicação ao final?

Está com dúvidas (ou curioso 👀) para ver como deve ficar a aplicação ao final do desafio? Deixamos abaixo um vídeo mostrando as principais funcionalidades que você deve implementar para te ajudar (ou matar sua curiosidade 👀).

[https://s3-us-west-2.amazonaws.com/secure.notion-static.com/10783a0f-e3a7-4991-8bb5-43f73508431f/demo.mp4](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/10783a0f-e3a7-4991-8bb5-43f73508431f/demo.mp4)

# 📅 Entrega

Esse desafio deve ser entregue a partir da plataforma da Rocketseat. Envie o link do repositório que você fez suas alterações. Após concluir o desafio, além de ter mandado o código para o GitHub, fazer um post no LinkedIn é uma boa forma de demonstrar seus conhecimentos e esforços para evoluir na sua carreira para oportunidades futuras.

Feito com 💜 por Rocketseat 👋 Participe da nossa [comunidade aberta!](https://discord.gg/pUU3CG4Z)
