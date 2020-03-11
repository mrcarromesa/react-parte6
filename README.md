<h1>Global Styles</h1>

- Lembrando que é necessário instalar o `styled-components`:

```bash
yarn add styled-components
```

- Criar o arquivo `src/styles/globals.js`

- O arquivo importa de:

```js
import { createGlobalStyle } from 'styled-components';
```

- e o estilo é adicionado da seguinte forma:

```js
export default createGlobalStyle`

  //Seu estilo css normal aqui

`;
```

- Para adicionar arquivo de imagem por exemplo é necessário importar a imagem:

```js
import myImage from './assets/images/myImage.jpg';
```

- e no estilo adicionar a imagem dessa forma:

```js
//...
  div {
    background: url(${myImage});
  }
//...
```

- Realizar a chamada do arquivo em `src/App.js`

```js
import GlobalStyle from './styles/globals';
```

- por fim adicionar como componente:

```js
<GlobalStyle />
```
