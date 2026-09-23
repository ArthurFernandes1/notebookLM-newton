# 🍎 notebookLM-newton

Um assistente de pesquisa e historiador virtual baseado no Google NotebookLM para explorar a física de Isaac Newton usando Engenharia de Prompt e RAG.

## 🎯 Objetivo do Projeto

Este projeto utiliza o **Google NotebookLM** e técnicas de **Engenharia de Prompt** para criar um assistente acadêmico especializado na vida, obra e metodologia científica de Sir Isaac Newton. O objetivo é transformar um conjunto de fontes históricas e científicas em um banco de conhecimento interativo, capaz de explicar a Física Clássica através de uma perspectiva analítica e historiográfica.

### 🔄 Decisão de Arquitetura e Persona
Inicialmente, o projeto tentou forçar a IA a "interpretar" o próprio Isaac Newton em primeira pessoa. No entanto, observou-se que sistemas baseados em RAG (*Retrieval-Augmented Generation*) com identidades de sistema muito fortes (como o NotebookLM) entram em conflito com personas estritas. 

**O Pivot:** A abordagem foi ajustada para utilizar a ferramenta em seu estado da arte: como um **pesquisador e historiador da ciência**. O assistente agora analisa os documentos e responde com base nas evidências, formulando respostas ricas embasadas na filosofia experimental de Newton.

## 📂 Estrutura do Repositório

O repositório está organizado da seguinte forma para facilitar a replicação do laboratório:

- `📁 fontes/`: Contém o arquivo com os links dos vídeos, artigos acadêmicos (SciELO/RBEF) e textos base (biografias e história da ciência) que alimentam a base de conhecimento do RAG.
- `📁 prompt/`: Guarda a instrução de sistema (System Prompt) que configura o comportamento analítico e a persona de historiador do assistente.
- `📁 testes/`: Documentação da bateria de testes e consultas estruturadas realizadas para validar se a IA absorveu o método científico e a linha de raciocínio de Newton.

## 🛠️ Tecnologias Utilizadas
- **Google NotebookLM:** Motor de RAG para indexação, leitura e recuperação das fontes.
- **Engenharia de Prompt:** Ajuste de contexto e definição de regras de comportamento.
- **Física Clássica e História da Ciência:** Curadoria de material didático e fontes primárias/secundárias.

## ⚙️ Como replicar este projeto no seu NotebookLM

1. **Crie um novo caderno** no [Google NotebookLM](https://notebooklm.google.com/).
2. **Carregue o Conhecimento:** Abra a pasta `fontes/` deste repositório e adicione os links e documentos listados ao seu novo caderno.
3. **Configure a Diretriz:** Vá na seção de "Observações do Caderno" (ou System Prompt) e cole o conteúdo do arquivo localizado na pasta `prompt/`.
4. **Valide o Assistente:** Utilize as perguntas do arquivo na pasta `testes/` para iniciar a conversa e verificar se o assistente responde de forma analítica e não robótica.

---
*Desenvolvido como laboratório prático de Inteligência Artificial, Engenharia de Prompt e Metodologias de Ensino de Física.*
