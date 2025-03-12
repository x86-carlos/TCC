# Automated Detection of Password Leakage from Public GitHub Repositories

***

R. Feng, Z. Yan, S. Peng and Y. Zhang, "Automated Detection of Password Leakage from Public GitHub Repositories," 2022 IEEE/ACM 44th International Conference on Software Engineering (ICSE), Pittsburgh, PA, USA, 2022, pp. 175-186, doi: [10.1145/3510003.3510150](https://doi.org/10.1145/3510003.3510150)

***

## 1. Fichamento do Conteúdo

O artigo possui dois focos claros: primeiro é o de apresentar os conceitos que embasam, o desenvolvimento e a avaliação do *PassFinder* uma ferramenta desenvolvida pelos pesquisadores que detecta senhas vazadas em códigos-fonte. O segundo ponto de interesse do texto é uma análise em larga escala de vazamento de senhas em repositórios do *GitHub* utilizando o *PassFinder*, portanto ambos os seguimentos do artigo estão relacionados. O que diferencia essa ferramenta das outras já existentes é tanto o tipo de senha a qual o *PassFinder* identifica e o método utilizado para fazer o reconhecimento. Este baseado no contexto em que senhas aparecem ao invés de expressões regulares sofisticadas e tecnicas baseadas em entropia, aquele focando em senhas textuais no lugar de chaves de API (*Application Programming Interface*), chaves de criptografia, chaves PEM (*Privacy Enhanced Mail*) e outros tipos de credencias com formatos distintos. A ferramenta foi cosntruida utilizando *Deep Learning* e redes neurais e é interessante como os autores separam espaço no artigo para explicar como o experimento que avalia a ferramenta construída foi planejado e executado antes de fazer uma maior mineração de dados dentros de repositórios mais heterogeneos presente no GitHub.

## 2. Fichamento Bibliografico

- *Regular Expression*(Expressões Regulares): uma sequência de caracteres que especifica um padrão que deve ser encontrado em um texto, no contexto do artigo fichado a expressões regulares são tecnicas usadas para encontrar senhas em códigos. (página 1)
- *Shannon Entropy*(Entropia de Shannon): é um conceito introduzido por Claude Shannon que no contexto do artigo também é usado como forma de encontrar senhas vazadas em artigos. (página )
- *Deep Neural Network*(Rede Neural Profunda): é um subconjunto da aprendizagem de máquina usada para realizar tarefas como classificação.(página 1)


## 3. Fichamento de Citações

- *Due to some developers’ lack of security consciousness, it is not uncommon for such authentication information to be exposed to the public as part of GitHub repositories [ 2 ] [ 3].*
- *"So far, secret scanning supports a set of credentials, including Alibaba Cloud Access Key, Azure Access Token and AWS Access Key,etc. Besides, many open source tools [ 15] [17][18 ] [20 ] [26] weredeveloped to help prevent developers from pushing their sensitive authentication information to public repositories. However,existing work mainly focuses on structured secrets like API keys,which could be easily detected with well-crafted regular expressions.Relatively little attention has been paid to textual passwords."*
- *"Unlike structured secrets likeAPI keys, etc., textual passwords could be virtually any strings anddo not conform to distinct structures, thus making them hard to detect with high accuracy."*
- *"In general, these techniques perform poorly since they cannot properly deal with the heterogeneity of passwords, which hinders them from being adopted in practice."*
- *" Specifically, we divide textual passwords into two main categories, i.e., human-chosen passwords and machine-generated random passwords. PassFinder models the distribution of human chosen passwords corpus, random passwords corpus, and ordinary strings corpus with a deep neural network, which further guides predicting strings being passwords or not."*
- *"Typically, when authenticating with passwords, developers have to provide extra information such as identity, remote host, connection configuration, etc., which constitute the context of the passwords. Combining intrinsic char acteristics and context information, PassFinder can finally identify passwords in source code files. Intuitively, our design reflects how a human identifies passwords in source code, i.e., by understanding individual strings and reasoning about the meaning of the context."*
