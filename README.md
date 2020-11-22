# React Learning Path

Não faz muito tempo um amigo meu, querendo se aventurar nesse mundo do React de uma maneira mais profunda me fez as seguintes perguntas, **"Por onde começar? Por onde seguir? Quando que eu termino?"**.

Bom, devo admitir que estas são perguntas no mínimo escorregadias, porque em primeiro lugar, é difícil de definir, cada ponto de partida, você já trabalhou com web? angular? Jquery? Com a stack HTML, css e JS puros?

Contudo depois de pensar um tanto, acho que consegui desenhar um percurso que é tanto agnóstico a sua trajetória atual se você tem o mínimo de noção quanto a desenvolvimento web, quanto generalista o suficiente que com base nele você consegue trabalhar como um dev pleno em qualquer projeto react que te botarem ou que você quiser fazer.  

A vantagem é que você não precisa ser PhD em cada item dessa lista, vou admitir que dos alguns conceitos listados nos tópicos avançados eu só conheço uns 2 implementando de fato, mas mais importante que a aplicação destas ferramentas é o conceito por trás delas.

Uma visão ampla de como funciona cada uma dessas ferramentas mesmo as mais básicas, vai te dar um instinto mais arquitetural do sistema que você está trabalhando. Vai te fazer enxergar onde está seu sistema atualmente e pra onde ele vai. E ter esse instinto macro vai te fazer um desenvolvedor melhor no micro contexto.

Lembrando que essa lista não está cravada em pedra, React hooks não tem dois anos e já é padrão de mercado. Se deseja dar a sua opinião, comentar sobre o seu percurso, me convencer a adicionar ou remover um item dessa lista, [meu LinkedIn está aqui](https://www.linkedin.com/in/thalesgsn).

## Pra quem é esse learning path

De maneira simples pra qualquer um que já teve alguma experiência com desenvolvimento frontend mesmo que básico, e tem interesse em se tornar um dev react completo,  

Se você não tem nenhuma experiência com desenvolvimento web, recomendo de verdade aprender HTML, CSS e JS de uma maneira mais completa primeiro, te garanto que este tempo vai se pagar no futuro e você vai ter muito menos problemas em entender os conceitos que eu vou apresentar aqui em baixo.

## Como Funciona a lista?

É bem simples, o que vem primeiro na lista tem um contexto mais geral, foque nesses estes conceitos mais gerais, eles geralmente são mais úteis e servem pra mais coisas do que libs que servem para que uma aplicação específica. Se tem confiança que sabe um assunto o suficiente, pode pular, se não tem ideia ou tem dúvidas sobre esse assunto, reserve um tempinho e estude.

Todos os itens que eu considero que são mais difíceis de se achar conteúdo ou que eu tenha uma referência que eu tenha preferência eu vou linkar no item.

## Diagrama mostrando o roadmap (TODO)

## Módulo Básico

Essa lista é que mais gera valor na carreira de um dev front, pois vale pra qualquer contexto, usando frameworks ou não. Aqui provavelmente tem muito conteúdo que um dev pleno já sabe pelo menos um pouco, mas pode ser que não, se não sabe como usar qualquer elemento dessa lista vale muito a pena focar nestes, são conteúdos simples de aprendizagem fácil e rápida, que geram muito valor. E esse conteúdo é requerido para lidar da melhor forma com seu código react e como ele funciona debaixo dos panos.
  
1. HTML
* [Semantic HTML](https://developer.mozilla.org/en-US/docs/Glossary/Semantics)
* [ARIA Atributes mais importantes](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA).
	* aria-label
	* aria-live
	* role
	* aria-controls
	* aria-value (now, min, max)
2. CSS
* seletores
* pseudo seletores
* media queries
* flex (https://css-tricks.com/snippets/css/a-guide-to-flexbox)
* grid (https://css-tricks.com/snippets/css/complete-guide-grid)
* sass
  
3. JS
* Event loop (https://www.youtube.com/watch?v=cCOL7MC4Pl0)
* Promise API (https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)
* Async await (https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/async_function)
* generator functions (https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function*)
* fetch API (https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch)
* Functional JS (https://opensource.com/article/17/6/functional-javascript)
* imutabilidade
* function composition
* Array functions
	* map
	* reduce
	* filter
	* find
	* flat
	* flatmap
	* every
	* some
	
4. Conceitos gerais
Com relação a esses conceitos, vale a pena a aprender o que eles são na teoria e estudar como implementa-los quando precisar na prática.
* Componentização (A primeira parte desse KT: https://web.microsoftstream.com/video/62928a8c-c073-4a43-ba3e-0032e276a0b9)
* I18n para internacionalização de aplicações. (https://www.sitepoint.com/how-to-implement-internationalization-i18n-in-javascript)
* Axios vs Fetch
* EsLint + Pa11y
* Webpack
* Typescript
* Teste unitário
* Testes E2e
* PWA
* SPA vs SSR

## React

Depois disso chegamos a parte do react de fato, vou cobrir aqui os assuntos mais importantes.
Não necessariamente você tem que saber todos os detalhes de implementação, mas saber o que é cada uma dessas coisas e quando usar.

1. JSX vs Create element
2. Class components **(prefira sempre Functional Components)**
3. Functional components
4. React lists e porque usar Key
5. Hooks
* useState
* useEffect
* useContext
* useRef
**Atenção:** os dois próximos hooks são relacionados a performance, mas devem ser usados com cautela pois se usados de maneira vasta pioram a performance da sua aplicação. [Quando usar então?](https://kentcdodds.com/blog/usememo-and-usecallback)
* useCallback
* usememo
6. React fragment
7. React-router
8. React.Lazy
9. React.Memo
10. Estilização
* React in-line style
* styled components
* [Material e MUI Theme (se for uma aplicação Material)](https://material-ui.com/customization/theming)

11. Testing
* Jest
* Enzyme
* React Testing Library (prefira este)
* Cypress

12. Estrutura do projeto
* [Feature based](https://reactjs.org/docs/faq-structure.html)
* [Atomic design](https://danilowoz.com/blog/atomic-design-with-react)
* [Feature special (meu favorito, e criado por um amigo meu)](https://github.com/ramonprata/structure_react_redux_app)

## Redux
Apesar de não ser uma ferramenta mandatória no mundo react, ela é amplamente utilizada, às vezes até mesmo de maneira errada, então até mesmo se você tomar a decisão de não utilizar Redux na sua arquitetura, você deve saber o porquê dessa decisão. [Artigo sobre o assunto.](https://dev.to/g_abud/why-i-quit-redux-1knl)
  
1. [Arquitetura Flux](https://facebook.github.io/flux)
2. Redux
	* Store
	* Reducers
	* Dispatcher
	* Actions
3. React Redux
4. Redux Structures
	* Rails-style
	* Domain-style
	* Ducks
	* Domain + Ducks
5. Redux Thunk
6. Redux saga
7. Alternativas
Saiba quais os pontos positivos e negativos dessas alternativas e quando eles se encaixam no seu produto.
	* React Query
	* MobX
	* Recoil
	* Context

## Tópicos avançados
Aqui em baixo estão somente tópicos avançados que são necessários em contextos específicos, se você dominou a lista de cima, recomendo e muito dar uma olhada geral nessas ferramentas e estudar quando usá-lás.
1. Aplicações react internacionalizadas usando [react-i18next](https://www.i18next.com)
2. Páginas estáticas e SSR - [Gatsby](https://www.gatsbyjs.com) e [Next.JS](https://nextjs.org)
3. [Service Workers para Aplicações React PWA](https://developers.google.com/web/fundamentals/primers/service-workers)
4. Lidando com aplicações com muitos forms complexos com [Formik](https://formik.org)
5. [Estruturas microfrontend usando react](https://www.robinwieruch.de/react-micro-frontend).
