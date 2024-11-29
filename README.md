# Multi-Hop-Question-Answering-with-Knowledge-Graphs
## Introdução
Com os avanços da inteligência artificial (IA) e do processamento de linguagem natural (NLP), novas possibilidades surgem para explorar e disseminar conhecimento em áreas estratégicas. Um exemplo disso é a Amazônia Azul, correspondente à zona econômica exclusiva (ZEE) do Brasil, uma região rica em biodiversidade e recursos naturais, mas ainda carente de informações acessíveis e organizadas. Nesse contexto, nosso projeto propõe a criação de um sistema de resposta a perguntas baseado em grafos de conhecimento, integrando técnicas modernas de NLP para organizar e conectar informações, respondendo a questões complexas e promovendo o acesso ao conhecimento.

Essa iniciativa busca consolidar dados relevantes sobre a Amazônia Azul, permitindo aplicações que vão da educação ao suporte a pesquisas científicas. Ao unir NLP com grafos de conhecimento, o projeto não só apoia o avanço de iniciativas como o Blue Amazon Brain (BLAB), mas também reforça o papel da IA na gestão de patrimônios estratégicos. Com isso, a tecnologia contribui para a preservação ambiental, a conscientização pública e o desenvolvimento econômico sustentável no Brasil.

## Objetivo
Este trabalho tem como objetivo desenvolver e avaliar algoritmos de question answering (QA) com salto de contexto, aplicados ao domínio da Amazônia Azul, utilizando técnicas de inteligência artificial e processamento de linguagem natural. A pesquisa envolve a criação de um sistema capaz de navegar por grafos de conhecimento, conectar múltiplos contextos e responder a perguntas complexas de forma precisa e relevante. O projeto busca não apenas contribuir para o avanço de ferramentas tecnológicas no âmbito do QA, mas também apoiar iniciativas como o Projeto BLAB, promovendo a disseminação de conhecimento sobre a Amazônia Azul e fortalecendo sua relevância estratégica, ambiental e educacional.

![GrafoExemplo](https://github.com/user-attachments/assets/3eedbbda-8003-4b3d-a3f0-b5a4bcf0f9d7)

## Justificativa

A justificativa deste trabalho baseia-se no potencial transformador da combinação de inteligência artificial e grafos de conhecimento na resolução de problemas complexos que exigem raciocínio em múltiplas etapas. Grafos de conhecimento são ferramentas poderosas para organizar e estruturar informações, permitindo a análise aprofundada e a conexão de dados aparentemente desconexos. Essa abordagem não apenas amplia a capacidade de sistemas inteligentes de fornecer respostas mais completas e contextualizadas, mas também potencializa avanços em áreas como educação, atendimento ao cliente, pesquisa científica e até sistemas médicos. Ao explorar algoritmos capazes de realizar saltos de contexto, este projeto propõe inovações que podem impactar diretamente a experiência do usuário, transformando ferramentas interativas e promovendo maior eficiência e personalização em aplicações práticas. Além disso, o foco na Amazônia Azul, um tema de alta relevância estratégica e ambiental, reforça a importância social e acadêmica deste trabalho, contribuindo para a conscientização e disseminação de conhecimento sobre uma das regiões mais importantes do Brasil.

## Metodologia

O método adotado neste trabalho foi estruturado em quatro etapas principais, cada uma desenvolvida para garantir a robustez técnica e a usabilidade do sistema de question answering baseado em grafos de conhecimento. Inicialmente, foi realizada uma revisão bibliográfica abrangente, abordando conceitos essenciais de grafos, como entidades e relações, além de algoritmos e abordagens recentes que aplicam inteligência artificial à construção e navegação desses grafos. Na segunda etapa, foi implementado o algoritmo AutoKG, adaptado para o contexto do domínio da Amazônia Azul, permitindo a extração e estruturação automática de conhecimento a partir de textos não estruturados. Em seguida, testes rigorosos avaliaram a precisão e a eficiência do algoritmo, considerando métricas de identificação de entidades, relações e qualidade das respostas geradas. Por fim, foi realizada a integração do sistema a uma interface de chatbot, desenvolvida com backend em Python e frontend em JavaScript, permitindo consultas interativas e visualização gráfica do percurso no grafo, garantindo acessibilidade e aplicabilidade prática.

## Arquitetura
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

![arquitetura_modulo drawio (1)](https://github.com/user-attachments/assets/ba325948-7dbf-4679-8f1f-5c694326a6b3)

## Testes e Avaliação
### Metodologia de Testes
Ao longo do desenvolvimento do projeto, realizamos uma série de testes rigorosos para avaliar o desempenho e a eficiência do sistema em diferentes cenários. Inicialmente, os testes focaram na validação das funcionalidades principais, garantindo que cada componente operasse conforme o esperado. Posteriormente, avançamos para análises mais detalhadas, incluindo simulações com diferentes cargas e variações de entrada, permitindo identificar pontos críticos que poderiam comprometer o desempenho. Cada rodada de testes trouxe insights valiosos, possibilitando ajustes que resultaram em melhorias significativas na estabilidade, na velocidade de processamento e na capacidade de atender às demandas do sistema.

Com base nos resultados obtidos, decisões importantes foram tomadas para refinar o projeto e alcançar sua versão final. Ajustes no algoritmo central, otimizações na estrutura de dados e alterações na lógica de tratamento de erros foram implementados para garantir maior eficiência e confiabilidade. Essa abordagem iterativa, guiada por testes constantes, permitiu que chegássemos a uma solução robusta, capaz de atender aos requisitos estabelecidos com precisão e qualidade. O processo reforçou a importância de uma metodologia baseada em experimentação e análise contínua para alcançar resultados sólidos.\

![image](https://github.com/user-attachments/assets/feb5dd5f-98c7-4d60-afbc-65fa3ae33204)

O sistema demonstrou alta precisão em perguntas bem estruturadas e desempenho satisfatório em grafos com até 75 relações.
A visualização das trajetórias no grafo auxilia o entendimento de como o algoritmo está atuando.
O acerto foi otimizado e tempo médio de resposta foi reduzido consideravelmente com a seleção correta de parâmetros para o sistema(número de saltos e fator de ramificação).

## Conclusão
Este projeto apresentou uma solução inovadora para sistemas de QA, combinando tecnologias modernas de NLP com estruturas eficientes de grafos de conhecimento. A arquitetura modular e a implementação cuidadosa permitiram:

Eficiência no Processamento: Respostas rápidas e precisas em diversos cenários.
Experiência de Usuário: Transparência no processo de busca e interface intuitiva.
Escalabilidade: Suporte a grafos complexos sem perda significativa de desempenho.
O sistema tem aplicações em diversas áreas, como educação, atendimento ao cliente e suporte técnico, sendo uma contribuição significativa para a área de sistemas inteligentes e interação homem-máquina.
