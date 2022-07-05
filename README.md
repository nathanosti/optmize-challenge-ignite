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

Perceba que ele iniciou uma fake API com os recursos `/genres` e `/movies` em `localhost` na porta `3333` a partir das informações do arquivo [server.json]

Acessando essas rotas no seu navegador, você consegue ver o retorno das informações já em JSON (dando um clique duplo, a imagem se expandirá):

Dessa forma, basta consumir essas rotas da API normalmente com o Axios. 

Caso queira estudar mais sobre o **JSON Server**, dê uma olhada aqui:

[typicode/json-server](https://github.com/typicode/json-server)

## O que devo editar na aplicação?

Com o template já clonado, as dependências instaladas e a fake API rodando, você deve começar implementar as estratégias de otimização para a aplicação.

Aqui estão os dois principais arquivos que devem ser editados:

- **[src/App.tsx]**
Esse é o componente principal da aplicação e contém toda a lógica da aplicação como chamadas à API e controle de estados dos componentes Content e SideBar.

- **[src/components/Content.tsx]**
Esse componente, possui toda a lógica e corpo responsável pelo header e conteúdo da aplicação (seção contornada em vermelho):

- **[src/components/SideBar.tsx]**
Esse componente possui toda a lógica e corpo responsável pela seção que contém o título do site e a parte de navegação à esquerda da página (seção contornada em vermelho):

Se você preferir, pode também componentizar algumas outras partes da aplicação como, por exemplo, o header, mas esse não está como requisito deste desafio 🚀

## Dicas

Lembre-se de usar corretamente as funcionalidades do React para prover mais performance para a aplicação:

memo;

useMemo;

useCallback;

Mesmo que a aplicação não precise de alguns pontos de otimização, sinta-se livre para usar as ferramentas a sua disposição como forma de aprendizado mas continue tomando cuidado com otimizações desnecessárias ao trabalhar com algum projeto real 💜.

Feito com 💜 por Rocketseat 👋 Participe da nossa [comunidade aberta!](https://discord.gg/pUU3CG4Z)
