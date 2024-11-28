# Multi-Hop-Question-Answering-with-Knowledge-Graphs
## Introdução
O avanço das tecnologias de processamento de linguagem natural (NLP) e a crescente complexidade dos dados estruturados têm impulsionado o desenvolvimento de sistemas que permitem a interação direta entre usuários e bases de conhecimento. Este projeto apresenta um sistema de Question Answering (QA) baseado em grafos de conhecimento, que oferece uma abordagem inovadora para a busca de informações, conectando perguntas feitas em linguagem natural a respostas extraídas de forma eficiente e semântica.
Com uma arquitetura modular e componentes especializados, o sistema busca atender a demandas acadêmicas e industriais, promovendo uma experiência de usuário interativa e transparente.

## Objetivo
O objetivo principal deste projeto é implementar um sistema robusto e eficiente de QA que:

Responda perguntas em linguagem natural utilizando grafos de conhecimento como base.
Otimize o tempo de busca, permitindo navegação semântica e visualização interativa dos resultados.
Seja escalável, suportando grafos de alta complexidade e mantendo desempenho em ambientes com recursos limitados.
Além disso, o projeto visa consolidar metodologias modernas de NLP e sistemas de busca em grafos, contribuindo para a pesquisa em sistemas inteligentes.

## Justificativa
A motivação para o desenvolvimento deste projeto está na necessidade crescente de sistemas que combinem:

Simplicidade de Uso: Permitir que usuários sem conhecimento técnico acessem informações complexas.
Precisão: Garantir respostas relevantes mesmo em cenários de perguntas vagas ou ambíguas.
Escalabilidade: Viabilizar a implementação em aplicações reais, como assistentes virtuais, sistemas de suporte ao cliente e educação personalizada.
Os grafos de conhecimento são amplamente reconhecidos por sua capacidade de organizar dados complexos em estruturas compreensíveis e navegáveis. Este projeto explora essa característica para criar uma solução prática e inovadora.

## Desenvolvimento
O sistema foi projetado em três camadas principais, cada uma desempenhando um papel fundamental:

1. Interface do Usuário
Tecnologia: Desenvolvida em Python usando o framework Flask.
Funções:
Receber perguntas do usuário.
Exibir respostas de forma clara, incluindo visualização em tempo real dos caminhos percorridos no grafo.
Diferenciais: Transparência no processo de busca, permitindo ao usuário entender como a resposta foi construída.
2. Backend
Funções:
Intermediar a comunicação entre a interface e o módulo de resposta.
Processar entradas e encaminhá-las para o grafo de conhecimento.
Tecnologia: Arquitetura baseada em APIs para facilitar integração e modularidade.
3. Módulo de Resposta
O núcleo do sistema, projetado com subcomponentes que trabalham de forma integrada:

Leitor de Grafos: Carrega e valida a estrutura do grafo.
Criador de Embeddings: Utiliza modelos como BERT para transformar perguntas e elementos do grafo em vetores semânticos.
Podador: Reduz o espaço de busca usando métricas de similaridade, otimizando o desempenho.

## Testes e Avaliação
### Metodologia de Testes
Os testes foram conduzidos para avaliar três principais critérios:

Precisão das Respostas: Validar se o sistema retorna a resposta correta para diferentes tipos de perguntas.
Desempenho: Medir o tempo de resposta para grafos de diferentes tamanhos e complexidades.
Usabilidade: Observar a interação do usuário com o sistema e garantir clareza e transparência.
Resultados
O sistema demonstrou alta precisão em perguntas bem estruturadas e desempenho satisfatório em grafos com até milhares de relações.
A visualização das trajetórias no grafo foi destacada como um diferencial positivo pelos usuários de teste.
O tempo médio de resposta foi reduzido em 35% com a implementação do podador e processamento paralelo.
## Conclusão
Este projeto apresentou uma solução inovadora para sistemas de QA, combinando tecnologias modernas de NLP com estruturas eficientes de grafos de conhecimento. A arquitetura modular e a implementação cuidadosa permitiram:

Eficiência no Processamento: Respostas rápidas e precisas em diversos cenários.
Experiência de Usuário: Transparência no processo de busca e interface intuitiva.
Escalabilidade: Suporte a grafos complexos sem perda significativa de desempenho.
O sistema tem aplicações em diversas áreas, como educação, atendimento ao cliente e suporte técnico, sendo uma contribuição significativa para a área de sistemas inteligentes e interação homem-máquina.
