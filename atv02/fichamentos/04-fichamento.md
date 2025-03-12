# Large Language Models for Test-Free Fault Localization

***

 A. Z. H. Yang, C. L. Goues, R. Martins and V. J. Hellendoorn, "Large Language Models for Test-Free Fault Localization," 2024 IEEE/ACM 46th International Conference on Software Engineering (ICSE), Lisbon, Portugal, 2024, pp. 165-176, doi: [10.1145/3597503.3623342.](https://doi.org/10.1145/3597503.3623342)

***

## 1. Fichamento de Conteúdo

Ainda que o primeiro artigo fichado já tenha feito uso de algo envolvendo Inteligência Artificial este artigo é de fato o que faz uma conexão, por mais que não seja o foco do texto, entre os dois principais temas que me capturaram o interesse. O presente artigo trata de *Fault Localization* (FL) que é a tentativa de encontrar qual parte de um código (linha, arquivo, classe, função) está envolvida em um erro em particular e para alcançar tal objetivo são utilizadas diversas técnincas como: *Spectrum Based Fault Localization* (SBPL) ou *Mutation Based Fault Localization* (MBPL), contudo essas técninas dependem de casos de teste, cobertura dos testes, qualidade do código, etc. A proposta dos pesquisadores é utilizar os *Large Language Models* (LLM), os quais receberam grande destaque e atenção nos últimos anos, para introduzir uma nova estratégia de FL que não depende de aspectos como os citados anteriormente e também, e este talvez seja o maior diferencial desse modelo, é capaz de identificar ao nível de linha de código uma falha de segurança.

## 2. Fichamento Bibliográfico

- *Fault Localization* (Localização de Falhas): localização da parte de um código que está diretamente relacionada com um erro.
- *Left to Right Model* (Modelo da esquerda para a direita): os modelos de linguagem produzem suas saídas da esquerda para a direita, usando o dado anterior para produzir o próximo dentro do contexto.
- *Large Language Model* (Grande modelo de linguagem): técnica de Inteligência Artificail utilizada para interpretar e gerar textos.

## 3. Fichamento de Citações

- *LLMAO is also the first FL technique trained using a language model architecture that can detect security vulnerabilities down to the code line level.*
- *Fault localization (FL) [ 1– 4] approaches aim to automatically identify which program entities (like a line, statement, module, or file) are implicated in a particular bug.*
- *Broadly speaking, existing FL techniques combine or leverage static and dynamic program analysis information to compute a score corresponding to a program entity’s probability of contributing to a particular bug.*
- *LLMAO is the first MLFL technique that can detect code line level vulnerabilities in the security domain.*
- *Vulnerability Detection Logical errors are not the only type of code mistakes that can impact software quality. Software security vulnerabilities are often the target of various forms of cyber-attacks.* 
