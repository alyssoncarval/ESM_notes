# Engenharia de Software Moderna

Modern Software Engineering is a textbook intended for undergraduate students in Computing. It can also be read by professionals seeking basic knowledge on the following topics:

- Agile methods such as Scrum, XP and Kanban.
- Agile requirements gathering, including user stories, - MVPs and A/B tests.
- Software Design, dealing with design properties, design principles and standards.
- Software Architecture, including patterns like MVC, microservices and publish/subscribe.
- Software Testing, with emphasis on unit tests, testability, coverage and TDD.
- Refactoring, with real examples of refactorings and code smells.
- DevOps, including version control, continuous integration and deployment.

All material from the book can be accessed [here](https://engsoftmoderna.info/).

# Summary

[Capítulo 1 - Introdução](https://github.com/alyssoncarval/ESM_notes#cap%C3%ADtulo-1---introdu%C3%A7%C3%A3o)

# Capítulo 1 - Introdução

Segundo Brooks, existem dois tipos de dificuldades em desenvolvimento de software: dificuldades essenciais e dificuldades acidentais. As essenciais são da natureza da área e dificilmente serão superadas por qualquer nova tecnologia ou método que se invente. 

Segundo Brooks, as dificuldades essenciais são as seguintes: 

- Complexidade: dentre as construções que o homem se propõe a realizar, software é uma das mais desafiadoras e mais complexas que existe. Na verdade, como dissemos antes, mesmo construções de engenharia tradicional, como um satélite, uma usina nuclear ou um foguete, são cada vez mais dependentes de software. 

- Conformidade: pela sua natureza software tem que se adaptar ao seu ambiente, que muda a todo momento no mundo moderno. Por exemplo, se as leis para recolhimento de impostos mudam, normalmente espera-se que os sistemas sejam rapidamente adaptados à nova legislação. Brooks comenta que isso não ocorre, por exemplo, na Física, pois as leis da natureza não mudam de acordo com os caprichos dos homens. 

- Facilidade de mudanças: que consiste na necessidade de evoluir sempre, incorporando novas funcionalidades. Na verdade, quanto mais bem sucedido for um sistema de software, mais demanda por mudanças ele recebe. 

- Invisibilidade: devido à sua natureza abstrata, é difícil visualizar o tamanho e consequentemente estimar o esforço de construir um sistema de software. 

As dificuldades (2), (3) e (4) são específicas de sistemas de software, isto é, elas não ocorrem em outros produtos de Engenharia, pelo menos na mesma intensidade. Por exemplo, quando a legislação ambiental muda, os fabricantes de automóveis têm anos para se conformar às novas leis. Adicionalmente, carros não são alterados, pelo menos de forma essencial, com novas funcionalidades, após serem vendidos. Por fim, um carro é um produto físico, com peso, altura, largura, assentos, forma geométrica, etc., o que facilita sua avaliação e precificação por consumidores finais. 

Ainda segundo Brooks, desenvolvimento de software enfrenta também dificuldades acidentais. No entanto, elas estão associadas a problemas tecnológicos, que os Engenheiros de Software podem resolver, se devidamente treinados e caso tenham acesso às devidas tecnologias e recursos. Como exemplo, podemos citar as seguintes dificuldades: um compilador que produz mensagens de erro obscuras, uma IDE que possui muitos bugs e frequentemente sofre travamentos, um framework que não possui documentação, uma aplicação Web com uma interface pouco intuitiva, etc. Todas essas dificuldades dizem respeito à solução adotada e, portanto, não são uma característica inerente dos sistemas mencionados. 

O SWEBOK define 12 áreas de conhecimento em Engenharia de Software: 

-Engenharia de Requisitos 

-Projeto de Software 

-Construção de Software 

-Testes de Software 

-Manutenção de Software 

-Gerência de Configuração 

-Gerência de Projetos 

-Processos de Software 

-Modelos de Software 

-Qualidade de Software 

-Prática Profissional 

-Aspectos Econômicos 


Engenharia de Requisitos 

Os requisitos de um sistema definem o que ele deve fazer e como ele deve operar. Assim, a Engenharia de Requisitos inclui o conjunto de atividades realizadas com o objetivo de definir, analisar, documentar e validar os requisitos de um sistema. Em uma primeira classificação, os requisitos podem ser funcionais ou não-funcionais. 

Requisitos funcionais definem o que um sistema deve fazer; isto é, quais funcionalidades ou serviços ele deve implementar. 

Já os requisitos não-funcionais definem como um sistema deve operar, sob quais restrições e com qual qualidade de serviço. São exemplos de requisitos não-funcionais: desempenho, disponibilidade, tolerância a falhas, segurança, privacidade, interoperabilidade, capacidade, manutenibilidade e usabilidade. 

Por exemplo, suponha um sistema de home-banking. Nesse caso, os requisitos funcionais incluem informar o saldo da conta, informar o extrato, realizar transferência entre contas, pagar um boleto bancário, cancelar um cartão de débito, etc. Já os requisitos não-funcionais, dentre outros, incluem: 

- Desempenho: informar o saldo da conta em menos de 3 segundos; 

- Disponibilidade: estar no ar 99% do tempo; 

- Tolerância a falhas: continuar operando mesmo se um determinado centro de dados cair; 

- Segurança: criptografar todos os dados trocados com as agências; 

- Privacidade: não disponibilizar para terceiros dados de clientes; 

- Interoperabilidade: integrar-se com os sistemas do Banco Central; 

- Capacidade: ser capaz de armazenar dados de 1 milhão de clientes; 

- Usabilidade: ter uma versão para deficientes visuais. 

Projeto de Software 

Durante o projeto de um sistema de software, são definidas suas principais unidades de código, porém apenas no nível de interfaces, incluindo interfaces providas e interfaces requeridas. Interfaces providas são aqueles serviços que uma unidade de código torna público para uso pelo resto do sistema. Interfaces requeridas são aquelas interfaces das quais uma unidade de código depende para funcionar. 

Quando o projeto é realizado em um nível mais alto e as unidades de código possuem maior granularidade — são pacotes, por exemplo — ele é classificado como um projeto arquitetural. Ou seja, arquitetura de software trata da organização de um sistema em um nível de abstração mais alto do que aquele que envolve classes ou construções semelhantes. 

Construção de Software 

Construção trata da implementação, isto é, codificação do sistema. Nesse momento, existem diversas decisões que precisam ser tomadas, como, por exemplo: definir os algoritmos e estruturas de dados que serão usados, definir os frameworks e bibliotecas de terceiros que serão usados; definir técnicas para tratamento de exceções; definir padrões de nomes, leiaute e documentação de código e, por último, mas não menos importante, definir as ferramentas que serão usadas no desenvolvimento, incluindo compiladores, ambientes integrados de desenvolvimento (IDEs), depuradores, gerenciadores de bancos de dados, ferramentas para construção de interfaces, etc. 

Testes de Software 

Teste consiste na execução de um programa com um conjunto finito de casos, com o objetivo de verificar se ele possui o comportamento esperado. A seguinte frase, bastante famosa, de Edsger W. Dijkstra — também prêmio Turing em Computação (1982) — sintetiza não apenas os benefícios de testes, mas também suas limitações: 

"Testes de software mostram a presença de bugs, mas não a sua ausência. " 

Existem diversos tipos de testes. Por exemplo, testes de unidade (quando se testa uma pequena unidade do código, como uma classe), testes de integração (quando se testa uma unidade de maior granularidade, como um conjunto de classes), testes de performance (quando se submete o sistema a uma carga de processamento para verificar seu desempenho), testes de usabilidade (quando o objetivo é verificar a usabilidade da interface do sistema), etc. 

Existem duas frases, muito usadas, que resumem as diferenças entre verificação e validação:  

- Verificação: estamos implementando o sistema corretamente? Isto é, de acordo com seus requisitos.  

- Validação: estamos implementando o sistema correto? Isto é, aquele que os clientes ou o mercado está querendo. 

Assim, quando se realiza um teste de um método, para verificar se ele retorna o resultado especificado, estamos realizando uma atividade de verificação. Por outro lado, quando realizamos um teste funcional e de aceitação, ao lado do cliente, isto é, mostrando para ele os resultados e funcionalidades do sistema, estamos realizando uma atividade de validação. 

Manutenção e Evolução de Software 

Assim como sistemas tradicionais de Engenharia, software também precisa de manutenção. Neste livro, vamos usar a seguinte classificação para os tipos de manutenção que podem ser realizadas em sistemas de software: corretiva, preventiva, adaptativa, refactoring e evolutiva. 

- Manutenção corretiva tem como objetivo corrigir bugs reportados por usuários ou outros desenvolvedores. 

- Por sua vez, manutenção preventiva tem como objetivo corrigir bugs latentes no código, que ainda não causaram falhas junto aos usuários do sistema. 

- Manutenção adaptativa tem como objetivo adaptar um sistema a uma mudança em seu ambiente, incluindo tecnologia, legislação, regras de integração com outros sistemas ou demandas de novos clientes. 

- Refactorings são modificações realizadas em um software preservando seu comportamento e visando exclusivamente a melhoria de seu código ou projeto. São exemplos de refactorings operações como renomeação de um método ou variável (para um nome mais intuitivo e fácil de lembrar), divisão de um método longo em dois métodos menores (para facilitar o entendimento) ou movimentação de um método para uma classe mais apropriada. 

- Manutenção evolutiva é aquela realizada para incluir uma nova funcionalidade ou introduzir aperfeiçoamentos importantes em funcionalidades existentes. Sistemas de software podem ser usados por décadas exatamente porque eles sofrem manutenções evolutivas, que preservam o seu valor para os clientes. 

Sistemas legados são sistemas antigos, baseados em linguagens, sistemas operacionais e bancos de dados tecnologicamente ultrapassados. Por esse motivo, a manutenção desses sistemas costuma ser mais custosa e arriscada. Porém, é importante ressaltar que legado não significa irrelevante, pois muitas vezes esses sistemas realizam operações críticas para seus clientes. 

Gerência de Configuração 

Atualmente, é inconcebível desenvolver um software sem um sistema de controle de versões, como git. Esses sistemas armazenam todas as versões de um software, não só do código fonte, mas também de documentação, manuais, páginas web, relatórios, etc. Eles também permitem restaurar uma determinada versão. Por exemplo, se foi realizada uma mudança no código que introduziu um bug crítico, pode-se com relativa facilidade recuperar e retornar para a versão antiga, anterior à introdução do bug. 

Gerência de projetos 

Desenvolvimento de software requer o uso de práticas e atividades de gerência de projetos, por exemplo, para negociação de contratos com clientes (com definição de prazos, valores, cronogramas, etc.), gerência de recursos humanos (incluindo contratação, treinamento, políticas de promoção, remuneração, etc.), gerência de riscos, acompanhamento da concorrência, marketing, finanças, etc.  

Em um projeto, normalmente usa-se o termo stakeholder para designar todas as partes interessadas no mesmo; ou seja, os stakeholders são aqueles que afetam ou que são afetados pelo projeto, podendo ser pessoas físicas ou organizações. Por exemplo, stakeholders comuns em projetos de software incluem, obviamente, seus desenvolvedores e seus clientes; mas, também, gerentes da equipe de desenvolvimento, empresas subcontratadas, fornecedores de qualquer natureza, talvez algum nível de governo, etc. 

Lei de Brooks: 

"A inclusão de novos desenvolvedores em um projeto que está atrasado contribui 
para torná-lo ainda mais atrasado." 
 
Processos de Desenvolvimento de Software 

Um processo de desenvolvimento define quais atividades e etapas devem ser seguidas para construir e entregar um sistema de software. Uma analogia pode ser feita, por exemplo, com a construção de prédios, que ocorre de acordo com algumas etapas: fundação, alvenaria, cobertura, instalações hidráulicas, instalações elétricas, acabamento, pintura, etc. 

Historicamente, existem dois grandes tipos de processos que podem ser adotados na construção de sistemas de software: 

- Processos Waterfall (ou em cascata) - propõem que a construção de um sistema deve ser feita em etapas sequenciais, como em uma cascata de água, na qual a água vai escorrendo de um nível para o outro. Essas etapas são as seguintes: levantamento de requisitos, análise (ou projeto de alto nível), projeto detalhado, codificação e testes. Finalizado esse pipeline, o sistema é liberado para produção, isto é, para uso efetivo pelos seus usuários, conforme ilustrado na próxima figura. 

Problema: o mundo pode ter mudado, bem como as necessidades dos clientes, que podem não mais precisar do sistema que ajudaram a especificar anos antes. 

- Processos Ágeis (ou incrementais ou iterativos) - processos ágeis tiveram um profundo impacto na indústria de software. Hoje, eles são usados pelas mais diferentes organizações que produzem software, desde pequenas empresas até as grandes companhias da Internet. Diversos métodos que concretizam os princípios ágeis foram propostos, tais como XP, Scrum, Kanban e Lean Development. 

Esses métodos também ajudaram a disseminar diversas práticas de desenvolvimento de software, como testes automatizados, test-driven development (isto é, escrever os testes primeiro, antes do próprio código) e integração contínua (continuous integration). Integração contínua recomenda que desenvolvedores integrem o código que produzem. 

Integração contínua recomenda que desenvolvedores integrem o código que produzem imediatamente, se possível todo dia. O objetivo é evitar que desenvolvedores fiquem muito tempo trabalhando localmente, em sua máquina, sem integrar o código que estão produzindo no repositório principal do projeto. Quando o time de desenvolvimento é maior, isso aumenta as chances de conflitos de integração, que ocorrem quando dois desenvolvedores alteram em paralelo os mesmos trechos de código. O primeiro desenvolvedor a integrar seu código será bem sucedido; enquanto o segundo desenvolvedor será informado de que o trecho já foi modificado pelo primeiro. 

Modelos de Software 

Um modelo oferece uma representação em mais alto nível de um sistema do que o seu código fonte. O objetivo é permitir que desenvolvedores possam analisar propriedades e características essenciais de um sistema, de modo mais fácil e rápido, sem ter que mergulhar nos detalhes do código. Os modelos são uma forma de documentar o código de um sistema. 

Por exemplo, UML (Unified Modelling Language) é uma notação que define mais de uma dezena de diagramas gráficos para representar propriedades estruturais e comportamentais de um sistema.  
 
Qualidade de Software 

Segundo uma classificação proposta por Bertrand Meyer (link), qualidade de software pode ser avaliada em duas dimensões: qualidade externa ou qualidade interna. Qualidade externa considera fatores que podem ser aferidos sem analisar o código. Como exemplo, temos os seguintes fatores (ou atributos) de qualidade externa: 

- Correção: o software atende à sua especificação? Nas situações normais, ele funciona como esperado? 

- Robustez: o software continua funcionando mesmo quando ocorrem eventos anormais, como uma falha de comunicação ou de disco? Por exemplo, um software robusto não pode sofrer um crash (abortar) caso tais eventos anormais ocorram. Ele deve pelo menos avisar por qual motivo não está conseguindo funcionar conforme previsto. 

- Eficiência: o software faz bom uso de recursos computacionais? Ou ele precisa de um hardware extremamente poderoso e caro para funcionar? 

- Portabilidade: é possível portar esse software para outras plataformas e sistemas operacionais? Ele, por exemplo, possui versões para os principais sistemas operacionais, como Windows, Linux e macOS? Ou então, se for um app, ele possui versões para Android e iOS? 

- Facilidade de Uso: o software possui uma interface amigável, mensagens de erro claras, suporta mais de uma língua, etc? Pode ser também usado por pessoas com alguma deficiência, como visual ou auditiva? 

- Compatibilidade: o software é compatível com os principais formatos de dados de sua área? Por exemplo, se o software for uma planilha eletrônica, ele importa arquivos em formatos XLS e CSV? 

Por outro lado, qualidade interna considera propriedades e características relacionadas com a implementação de um sistema. Portanto, a qualidade interna de um sistema somente pode ser avaliada por um especialista em Engenharia de Software e não por usuários leigos. São exemplos de fatores (ou atributos) de qualidade interna: modularidade, legibilidade do código, manutenibilidade e testabilidade. 

Prática Profissional 

Por fim, mas muito atual e relevante, existem questionamentos sobre o papel e a responsabilidade ética dos profissionais formados em Computação, em uma sociedade na qual os relacionamentos humanos são cada vez mais mediados por algoritmos e sistemas de software. Neste sentido, as principais sociedades científicas da área possuem códigos que procuram ajudar os profissionais de Computação — não necessariamente apenas Engenheiros de Software — a exercer seu ofício de forma ética. Como exemplos, temos o Código de Ética da ACM (link) e da IEEE Computer Society (link). Esse último é interessante porque é específico para a prática de Engenharia de Software. 

Aspectos Econômicos 

Diversas decisões e questões econômicas se entrelaçam com o desenvolvimento de sistemas. Por exemplo, uma startup de software deve decidir qual modelo de rentabilização pretende adotar, se baseado em assinaturas ou em anúncios. Desenvolvedores de apps para celulares têm que decidir sobre o preço que irão cobrar pela sua aplicação, o que, dentre outras variáveis, requer conhecimento sobre o preço das apps concorrentes. Por isso, não é surpresa que grandes companhias de software atualmente empreguem economistas, para avaliarem os aspectos econômicos dos sistemas que produzem. 


# Referências Bibliográficas

Marco Tulio Valente. Engenharia de Software Moderna: Princípios e Práticas para Desenvolvimento de Software com Produtividade, Editora: Independente, 395 páginas, 2020.
