# Contador criado com o Redux
## Comandos
Logo em seguida:
>npm install react-scripts --save

Para abrir o programa:
>npm start

## Requisitos
- Conhecimentos em React.js e JavaScript
- Configuração do node, npm e yarn

## React 
- É uma biblioteca para criar interfaces
- Declarativo
- Baseado em componentes

## Redux 
- É um State Container para aplicações JavaScript e para outras linguagens
- State Containers são um bloco da sua aplicação que armazena um estado de forma centralizada, que pode ser lido por outros blocos da aplicação
- Flux: arquitetura criada pelo Facebook para resolver problemas de estado e unificação de controle de estado e componentes, Elm: desenvolvida para escrever código funcional para o browser

## Elm
- Imutabilidade
- API declarativa
- Operações Determinísticas
- Controlar side-effects (quando não se pode evitá-los)

## Arquitetura Flux
![flux](https://user-images.githubusercontent.com/72028645/131545549-f1bc42b0-a011-450d-9f89-8903b9bfdcaa.png)

## Arquitetura Redux
![redux](https://user-images.githubusercontent.com/72028645/131546580-7da502a9-ecbb-4d43-9ff1-62cef74eb708.jpg)

## Os três princípios
- Uma única fonte de verdade
- Estado disponível apenas para leitura
- Mudanças no estado são feitas apenas por funções puras
- Store: `createStore()`
- Reducer: `store.getState()`
- Actions: `store.dispatch()`
- View: `connect (react-redux)`
- Selectors

## Middlewares
- Faz a [interação](https://redux.js.org/understanding/history-and-design/middleware) com a store de uma forma que não é através da aplicação

## Enhanced Stores
- É uma [função](https://chariotsolutions.com/blog/post/redux-middleware-and-enhancers-getting-redux-to-log-debug-and-process-async-work/) que cria uma nova store caso precise mudar o estado ou como a store vai se comportar 

## @reduxjs/toolkit
NPM:
>npm install @reduxjs/toolkit

YARN:
>yarn add @reduxjs/toolkit

Criar um Redux:
>npx create-react-app my-app --template redux

- configureStore (redux-thunk + Redux DevTools Extension)
- createReducer (immer.js)
- createAction
- createSlice (reducers + actions)
- createSelector (reselect)

## Alternativas de state containers
- Context API (React)
- Recoil (FB)
- MobX (redux-saga, RxJS)
- XState

## Prós e contras de state containers
### Prós
- Simplifica problemas de data-flow complexos
- Pontos únicos de controle de estado

### Contras
- Complica problemas de data-flow simples

## Conclusão
- Super poderoso, mas pode ser custoso
- Super extensível, mas precisa de clareza
- State containers resolvem problemas não triviais 
- Flexível para resolver vários problemas, mas talvez não o seu
- Propósito do Redux é muito diferente do React, e pode ser usado em outras soluções

## Redux Devtools
NPM:
>npm install --save redux-devtools-extension

YARN:
>yarn add redux-devtools-extension

## Guias
- [Style Guide](https://redux.js.org/style-guide/style-guide/)
- [Ducks Pattern](https://medium.com/@matthew.holman/what-is-redux-ducks-46bcb1ad04b7)
- [Higher-Order Reducers](https://www.digitalocean.com/community/tutorials/redux-higher-order-reducers)
- [Hooks](https://react-redux.js.org/api/hooks)

## Quiz
### O que é um State Container?
Blocos (container) da sua aplicação que armazena um estado de forma centralizada, que pode ser lido por outros blocos da aplicação.

### Sabemos que o Redux foi inspirado tanto em Flux quanto em Elm. Tendo em vista essa informação, quais foram as influências da linguagem Elm sobre o Redux?
Imutabilidade, API declarativa, operações determinísticas, controlar side-effects (quando não se pode evita-los).

### Quais são as principais características do Redux?
Previsível, centralizado, debugavel e flexível.

### Quais os prós da criação de State Containers?
Simplifica problemas de data-flow complexos e pontos únicos de controle de estado.

### Quais os 3 princípios da arquitetura Redux?
Uma única fonte de verdade, estado disponível apenas para leitura e mudanças no estado são feitas apenas por funções puras.

### O que é o Redux?
Um State Container para armazenar os estados das aplicações JavaScript ou outras linguagens.

### O que é o React?
Uma biblioteca JavaScript para construir interfaces Web.

### Qual foi a principal influência da arquitetura Flux para o Redux?
Aprimorou um fluxo direcional para as ações, diminuindo a complexidade assim evitando perca de dados e gargalos durante as aplicações.

### O que são os middlewares?
Funções que são capazes de conectar outras funções, por exemplo um software é capaz de criar mais facilmente e eficientemente a conexão entre aplicações, dados e usuários.

### Quais os pilares do React?
Ser declarativo e baseado em componentes. Com isso, uma vez que o componente é definido/registrado, ele pode ser usado em qualquer lugar do projeto.
