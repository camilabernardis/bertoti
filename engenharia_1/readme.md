### Trecho 1: O conceito de engenharia de software

> What precisely do we mean by software engineering? What distinguishes “software engineering” from “programming” or “computer science”? And why would Google have a unique perspective to add to the corpus of previous software engineering literature written over the past 50 years? The terms “programming” and “software engineering” have been used interchangeably for quite some time in our industry, although each term has a different emphasis and different implications. University students tend to study computer science and get jobs writing code as “programmers.” “Software engineering,” however, sounds more serious, as if it implies the application of some theoretical knowledge to build something real and precise. Mechanical engineers, civil engineers, aeronautical engineers, and those in other engineering disciplines all practice engineering. They all work in the real world and use the application of their theoretical knowledge to create something real. Software engineers also create “something real,” though it is less tangible than the things other engineers create. Unlike those more established engineering professions, current software engineering theory or practice is not nearly as rigorous. Aeronautical engineers must follow rigid guidelines and practices, because errors in their calculations can cause real damage; programming, on the whole, has traditionally not followed such rigorous practices. But, as software becomes more integrated into our lives, we must adopt and rely on more rigorous engineering methods. We hope this book helps others see a path toward more reliable software practices.

#### Comentário:

Programar é uma habilidade que pode ser desenvolvida de várias formas, e ser "programador" não é o mesmo que dominar lógica de programação. Já a engenharia de software adiciona uma camada de estrutura e rigor muito maior. A comparação com outras engenharias, como a civil e a aeronáutica, é especialmente pertinente: em todas elas, o conhecimento teórico é aplicado de forma disciplinada para construir algo real e confiável.

O texto enfatiza que o engenheiro de software precisa ir além da lógica básica e adotar princípios que resultem em código robusto, limpo e de fácil manutenção. Isso facilita a integração entre sistemas e reduz custos e retrabalho no longo prazo. É justamente essa preocupação com qualidade, previsibilidade e sustentabilidade do código que diferencia o engenheiro de software de quem apenas escreve código.


### Techo 2: Programming Over Time

> Programming Over Time We propose that “software engineering” encompasses not just the act of writing code, but all of the tools and processes an organization uses to build and maintain that code over time. What practices can a software organization introduce that will best keep its code valuable over the long term? How can engineers make a codebase more sustainable and the software engineering discipline itself more rigorous? We don’t have fundamental answers to these questions, but we hope that Google’s collective experience over the past two decades illuminates possible paths toward finding those answers. One key insight we share in this book is that software engineering can be thought of as “programming integrated over time.” What practices can we introduce to our code to make it sustainable—able to react to necessary change—over its life cycle, from conception to introduction to maintenance to deprecation? The book emphasizes three fundamental principles that we feel software organizations should keep in mind when designing, architecting, and writing their code:
> - Time and Change: How code will need to adapt over the length of its life
> - Scale and Growth: How an organization will need to adapt as it evolves
> - Trade-offs and Costs: How an organization makes decisions, based on the lessons of Time and Change and Scale and Growth

#### Comentário:

O texto propõe que a engenharia de software vai além do ato de escrever código: ela abrange todas as ferramentas e processos que uma organização usa para construir e manter esse código ao longo do tempo. A ideia de "programação integrada ao longo do tempo" resume bem isso, pois o software precisa ser sustentável, ou seja, capaz de reagir a mudanças em todo o seu ciclo de vida, da concepção até a manutenção e a descontinuação.

Nesse sentido, a engenharia de software e a programação precisam ser como um camaleão: adaptáveis e presentes em todas as etapas do projeto, do início ao fim. Isso significa considerar como o código vai evoluir com o tempo (Time and Change), como a organização vai crescer e se ajustar (Scale and Growth) e como tomar decisões equilibrando custos e benefícios (Trade-offs and Costs). Um software que se adapta bem aos diferentes formatos e formas de uso tende a se manter valioso a longo prazo.

---

### Exemplos de Trade-offs

#### 1. Tamanho do Código vs. Nível de Senioridade Exigido

* **A troca:** Entregar um código mais curto e de fácil manutenção.
* **O trade-off:** Um código enxuto, mesmo com o uso de Regex, economiza linhas, mas acaba sendo escrito para pessoas com um nível de senioridade mais alto. Quem tem menos experiência pode levar mais tempo para entendê-lo e mantê-lo.

Uma observação interessante sobre esse ponto é que, conforme a pessoa vai aprendendo o código, ele tende a parecer naturalmente mais curto e simples. Isso mostra que a clareza também depende de quem lê, o que se conecta com a ideia de "programação integrada ao longo do tempo": o código precisa ser pensado para quem vai mantê-lo no futuro.

#### 2. IA Local (Ollama) vs. IA em Nuvem (API)

* **A troca:** Rodar o modelo de IA localmente, via Ollama, em vez de contratar uma API de IA na nuvem.
* **O trade-off:** Você ganha controle dos dados, independência de serviços externos e nenhum custo por uso, mas abre mão de desempenho. O modelo depende do hardware disponível, tende a responder mais devagar e costuma ser menos preciso que os modelos maiores oferecidos na nuvem.

Um ponto interessante é que essa decisão está ligada ao pilar de *Trade-offs and Costs* do livro: o custo deixa de ser financeiro e passa a ser de infraestrutura e de qualidade da resposta. Para um projeto acadêmico ou de pequena escala, a IA local faz sentido, mas, se o sistema crescesse, essa escolha precisaria ser reavaliada.

#### 3. Arquivo CSV vs. Banco de Dados

* **A troca:** Usar um arquivo CSV como base de dados dos imóveis em vez de implementar um banco de dados.
* **O trade-off:** O CSV é simples, rápido de implementar e fácil de ler e editar, mas abre mão de escalabilidade e de consultas eficientes. Conforme a quantidade de dados cresce, as buscas e os filtros ficam mais lentos e a manutenção das informações fica mais difícil.

Essa escolha ilustra bem o pilar de *Scale and Growth*: o que funciona bem para um protótipo pode não sustentar o crescimento do produto. Começar simples permite entregar valor mais cedo, desde que a equipe saiba que, no futuro, a migração para um banco de dados provavelmente será necessária.

---

## Minhas Contribuições na API: [API RibBIT 1º semestre](https://github.com/Grupo-RibBIT/API_ADS_1SEMESTRE_2026.2)

* Atuação como *Product Owner*, apresentando as dificuldades do cliente à equipe para a lapidação do produto.
* Utilização de uma IA local, via Ollama, para "ler" o arquivo CSV e responder às pesquisas iniciais.
* Estudo do funcionamento do formato JSON e apresentação do conteúdo ao grupo.

---

## Habilidades Aprendidas

* Integração de uma IA local, via Ollama, a bots do Telegram.
* Aplicação e manipulação de JSON.
* Comunicação e trabalho em equipe.
