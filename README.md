# Multi-Hop-Question-Answering-with-Knowledge-Graphs
## Introdução
Com os avanços da inteligência artificial (IA) e do processamento de linguagem natural (PLN), novas possibilidades surgem para explorar e disseminar conhecimento em áreas estratégicas. Um exemplo disso é a Amazônia Azul, correspondente às águas interiores, mar territorial, zona contígua, zona econômica exclusiva (ZEE) e águas sobrejacentes à plataforma continental (PC), uma região rica em biodiversidade e recursos naturais, mas ainda carente de informações acessíveis e organizadas. Nesse contexto, nosso projeto propõe a criação de um sistema de Question Answering (QA) baseado em grafos de conhecimento, integrando técnicas modernas de PLN para organizar e conectar informações, respondendo a questões complexas e promovendo o acesso ao conhecimento.

Essa iniciativa busca consolidar dados relevantes sobre a Amazônia Azul, permitindo aplicações que vão da educação ao suporte a pesquisas científicas. Ao unir NLP com grafos de conhecimento, o projeto não só apoia o avanço de iniciativas como o Blue Amazon Brain (BLAB - [https://repositorio.usp.br/item/003144894](https://repositorio.usp.br/item/003144894)), mas também reforça o papel da IA na gestão de patrimônios estratégicos. Com isso, a tecnologia contribui para a preservação ambiental, a conscientização pública e o desenvolvimento econômico sustentável no Brasil.

## Objetivo
Este trabalho tem como objetivo desenvolver e avaliar algoritmos de QA com salto de contexto, aplicados ao domínio da Amazônia Azul, utilizando técnicas de IA e PLN. A pesquisa envolve a criação de um sistema capaz de navegar por grafos de conhecimento, conectar múltiplos contextos e responder a perguntas complexas de forma precisa e relevante. O projeto busca não apenas contribuir para o avanço de ferramentas tecnológicas no âmbito do QA, mas também apoiar iniciativas como o BLAB, promovendo a disseminação de conhecimento sobre a Amazônia Azul e fortalecendo sua relevância estratégica, ambiental e educacional.

![GrafoExemplo](https://github.com/user-attachments/assets/3eedbbda-8003-4b3d-a3f0-b5a4bcf0f9d7)

## Justificativa

A justificativa deste trabalho baseia-se no potencial transformador da combinação de inteligência artificial e grafos de conhecimento na resolução de problemas complexos que exigem raciocínio em múltiplas etapas. Grafos de conhecimento são ferramentas poderosas para organizar e estruturar informações, permitindo a análise aprofundada e a conexão de dados aparentemente desconexos. Essa abordagem não apenas amplia a capacidade de sistemas inteligentes de fornecer respostas mais completas e contextualizadas, mas também potencializa avanços em áreas como educação, atendimento ao cliente, pesquisa científica e até sistemas médicos. Ao explorar algoritmos capazes de realizar saltos de contexto, este projeto propõe inovações que podem impactar diretamente a experiência do usuário, transformando ferramentas interativas e promovendo maior eficiência e personalização em aplicações práticas. Além disso, o foco na Amazônia Azul, um tema de alta relevância estratégica e ambiental, reforça a importância social e acadêmica deste trabalho, contribuindo para a conscientização e disseminação de conhecimento sobre uma das regiões mais importantes do Brasil.

## Metodologia

O método adotado neste trabalho foi estruturado em quatro etapas principais, cada uma desenvolvida para garantir a robustez técnica e a usabilidade do sistema de QA baseado em grafos de conhecimento. Inicialmente, foi realizada uma revisão bibliográfica abrangente, abordando conceitos essenciais de grafos de conhecimento, como entidades e relações, além de algoritmos e abordagens recentes que aplicam inteligência artificial à construção e navegação desses grafos. Na segunda etapa, foi implementado uma adaptação algoritmo Multihop KG, um algoritmo de busca em grafos voltado para o QA, permitindo o percorrimento de grafos de conhecimento a respeito do domínio da Amazônia Azul. Em seguida, testes rigorosos avaliaram a precisão e a eficiência do algoritmo, considerando métricas de identificação de entidades, relações e qualidade das respostas geradas. Por fim, foi realizada a integração do sistema a uma interface de chatbot, desenvolvida com backend em Python e frontend em JavaScript, permitindo consultas interativas e visualização gráfica do percurso no grafo, garantindo acessibilidade e aplicabilidade prática.

## Testes e Avaliação
### Metodologia de Testes
Ao longo do desenvolvimento do projeto, realizamos uma série de testes rigorosos para avaliar o desempenho e a eficiência do algoritmo em diferentes cenários. Inicialmente, os testes focaram na seleção do melhor método de seleção de caminhos para a busca. Posteriormente, avançamos para análises mais detalhadas, expandindo o grafo para definir o melhor modelo possível para o algoritmo e escolher os parâmetros que deixavam o funcionamento mais eficiente. Cada rodada de testes trouxe insights valiosos, possibilitando ajustes que resultaram em melhorias significativas na estabilidade, na velocidade de processamento e na capacidade de atender às demandas do sistema.

Com base nos resultados obtidos, decisões importantes foram tomadas para refinar o projeto e alcançar sua versão final. Ajustes no algoritmo central, otimizações na estrutura de dados e alterações na lógica de tratamento de erros foram implementados para garantir maior eficiência e confiabilidade. Essa abordagem iterativa, guiada por testes constantes, permitiu que chegássemos a uma solução capaz de atender aos requisitos estabelecidos com precisão e qualidade. O processo reforçou a importância de uma metodologia baseada em experimentação e análise contínua para alcançar resultados sólidos.

![image](https://github.com/user-attachments/assets/99184619-6484-4deb-b15a-80d77b98f531)

O sistema demonstrou alta precisão em perguntas bem estruturadas e desempenho satisfatório em grafos com até 75 relações.
A visualização das trajetórias no grafo auxilia o entendimento de como o algoritmo está atuando.
O acerto foi otimizado e tempo médio de resposta foi reduzido consideravelmente com a seleção correta de parâmetros para o sistema(número de saltos e fator de ramificação).

## Arquitetura
O sistema foi projetado em três camadas principais, cada uma desempenhando um papel fundamental:

* Interface do Usuário - Foi desenvolvida em Python usando o framework Flask e tem como função receber perguntas do usuário e exibir respostas de forma clara, incluindo visualização em tempo real dos caminhos percorridos no grafo.
* Backend - Intermedia a comunicação entre a interface e o módulo de resposta, processando entradas e encaminhando-as para o grafo de conhecimento. Foi feito com arquitetura baseada em APIs para facilitar integração e modularidade.
* Módulo de Resposta - O núcleo do sistema, projetado com subcomponentes que trabalham de forma integrada:
    * Leitor de Grafos: Carrega e valida a estrutura do grafo.
    * Criador de Embeddings: Utiliza modelos como BERT para transformar perguntas e elementos do grafo em vetores semânticos.
    * Podador: Reduz o espaço de busca usando métricas de similaridade, otimizando o desempenho.


![arquitetura_modulo drawio (1)](https://github.com/user-attachments/assets/ba325948-7dbf-4679-8f1f-5c694326a6b3)

## Conclusão
Este projeto apresentou uma solução inovadora para sistemas de QA, combinando tecnologias modernas de NLP com estruturas eficientes de grafos de conhecimento. A arquitetura modular e a implementação cuidadosa permitiram:

* Eficiência no Processamento: Respostas rápidas e precisas em diversos cenários.
* Experiência de Usuário: Transparência no processo de busca e interface intuitiva.
* Escalabilidade: Suporte a grafos complexos sem perda significativa de desempenho.

O sistema tem aplicações em diversas áreas, como educação, atendimento ao cliente e suporte técnico, sendo uma contribuição significativa para a área de sistemas inteligentes e interação homem-máquina.
