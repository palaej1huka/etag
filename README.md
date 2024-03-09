# Introdução

Logo de cara o professor reforçou uma ideia central: no ecossistema do framework, ninguém constrói componente do zero. O trabalho é montar a tela juntando peças prontas.

Esse vale também para a versão mobile.

# Repositório da turma

O material base das aulas está num repositório público mantido pela plataforma.

# Criando um aplicativo novo

O primeiro comando pede o modelo inicial do projeto:

```
npx create expo app componentes-overview -t
```

Quando o terminal perguntar qual modelo usar, escolha o de TypeScript sem nada extra.

Depois disso, basta entrar na pasta criada e subir o servidor de desenvolvimento:

```
npm run start
```

Para ver o resultado, é preciso um emulador aberto na IDE de desenvolvimento mobile. Com ele rodando, a tecla correspondente no terminal do servidor manda o aplicativo para o emulador.

O resultado é uma tela em branco, que serve de ponto de partida.


# A caixa básica

A peça mais elementar equivale à tag que agrupa elementos na web.

A imagem abaixo mostra várias dessas caixas posicionadas numa tela de celular:

![Caixas na tela](images/View.png)


## Capturando toques

Também foi mostrado como tratar toque numa caixa sem usar o componente específico de botão:

![Toques numa caixa](images/View-touch.png)

O professor comentou que, em vez de escrever a função ali na hora, dá para apontar para uma função declarada fora do componente.

Detalhe interessante na imagem: aparecem o evento de início e o de fim do toque, tratados separadamente.


## Onde procurar a referência

A documentação lista as propriedades da caixa e, mais abaixo, todos os eventos que ela emite.

![Documentação](images/documentation.png)

Alguns desses eventos, vale notar, só existem numa plataforma específica — a imagem mostra exemplos exclusivos do Android.

Em iOS, os nomes e o conjunto disponível mudam.

### Side note

Caso o comando nao responda, confira se a porta ja esta em uso.