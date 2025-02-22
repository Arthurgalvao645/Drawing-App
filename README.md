# 🌟 React - ThreeJS - Drawing App 🎨

Bem-vindo ao **React-ThreeJS Drawing App** – uma ferramenta poderosa para criar visualizações 2D e 3D! Este aplicativo cobre você, quer esteja procurando desenhar, manipular formas ou visualizar objetos em uma cena 3D. Vamos liberar sua criatividade! 🌐✨ Este é o boilerplate perfeito para dar o pontapé inicial em seus projetos de desenho com React, ThreeJS e EaselJS! 🚀
### 🎥 Demo Video

https://github.com/user-attachments/assets/27ea7167-7dec-4ab3-911e-9e0686a1a496

### 🌍 Live Demo

https://react-threejs-easeljs.web.app/

## 🎯 Principais características

- 🎨 **Desenhar formas:** Desenhe retângulos, círculos, linhas e caminhos personalizados sem esforço com uma interface de clicar e arrastar.
- ✋ **Manipulação de formas:** Mova, arraste e exclua formas conforme necessário. As formas se ajustam em tempo real para uma experiência suave!
- 🌐 **Visualizador 3D:** Alterne entre o modo 2D e o modo somente visualização 3D para ver seus desenhos ganharem vida em uma nova dimensão.
- 🎨 **Cores aleatórias:** Cada forma que você cria recebe um traço aleatório e uma cor de preenchimento.
- ⚡ **Atualizações em tempo real:** Observe sua tela atualizar instantaneamente conforme você interage com as formas.
- ⌨️ **Suporte ao teclado:** Exclua formas selecionadas usando as teclas Delete ou Backspace para edição rápida.
## 🛠️ Pilha de tecnologia

Este projeto foi criado usando tecnologias modernas:

- **React** ⚛️
- **Three.js** 🌐
- **EaselJS** 🎨
- **Vite** ⚡
- **Lodash** 🛠️
- **TypeScript** 🔧
- **Firebase** 🔥
- **SonarCloud** 🧪

### 📦 Dependências

O projeto depende de várias bibliotecas principais:

**React:** Uma biblioteca para construir interfaces de usuário.
**Three.js:** Um poderoso mecanismo 3D para renderizar o modo de visualização 3D.
**EaselJS:** Uma biblioteca para desenhar e manipular formas 2D.
**Vite:** Uma ferramenta de construção rápida para desenvolvimento web moderno.
**Lodash:** Uma biblioteca de utilitários para trabalhar com matrizes, objetos e muito mais.

### 🚀 Primeiros passos

Para iniciar o projeto localmente, bifurque o repositório e siga estas etapas:

```
1. 🍴 Bifurque o repositório
2. 📥 Clone seu repositório bifurcado
3. 🛠️ Execute `yarn install` para instalar dependências
4. 🚀 Execute `yarn dev` para iniciar o servidor de desenvolvimento local
```


### Expandindo a configuração do ESLint

Se você estiver desenvolvendo um aplicativo de produção, recomendamos atualizar a configuração para habilitar regras de lint com reconhecimento de tipo:

- Configure a propriedade de nível superior `parserOptions` assim:

```js
export default tseslint.config({
  languageOptions: {
    // other options...
    parserOptions: {
      project: ['./tsconfig.node.json', './tsconfig.app.json'],
      tsconfigRootDir: import.meta.dirname,
    },
  },
})
```

- Substitua `tseslint.configs.recommended` por `tseslint.configs.recommendedTypeChecked` ou `tseslint.configs.strictTypeChecked`
- Opcionalmente, adicione `...tseslint.configs.stylisticTypeChecked`
- Instale [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) e atualize a configuração:
```js
// eslint.config.js
import react from 'eslint-plugin-react'

export default tseslint.config({
  // Set the react version
  settings: { react: { version: '18.3' } },
  plugins: {
    // Add the react plugin
    react,
  },
  rules: {
    // other rules...
    // Enable its recommended rules
    ...react.configs.recommended.rules,
    ...react.configs['jsx-runtime'].rules,
  },
})
```
