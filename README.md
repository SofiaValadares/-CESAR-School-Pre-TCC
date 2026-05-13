# Modelo LaTeX para Projeto de Pesquisa - CESAR School

Este repositório contém um template LaTeX customizado e automatizado para a disciplina de **FP7 (Formação Profissional 7)**. O modelo foi projetado para alinhar a produtividade do LaTeX com as exigências visuais e pedagógicas do CESAR.

## �� Como Importar para o Overleaf

Para usar este modelo no Overleaf seguindo o fluxo do GitHub:

1.  **Download:** No repositório do GitHub, clique no botão verde **Code** e selecione **Download ZIP**.
2.  **Upload no Overleaf:** - Faça login no [Overleaf](https://www.overleaf.com).
    - Clique em **New Project** > **Upload Project**.
    - Arraste o arquivo `.zip` baixado para a área de upload.
3.  **Configuração do Motor (Crucial):**
    - Como o projeto utiliza a fonte Arial (via pacote `fontspec`), você precisa mudar o compilador padrão.
    - No canto superior esquerdo, clique em **Menu**.
    - Em **Compiler**, selecione **XeLaTeX**.
    - Clique em **Recompile**.

---

## �� Guia de Avaliação (Critérios FP7)

Este modelo foi estruturado para ajudar você a cumprir os itens de avaliação detalhados pelo professor (baseado no slide de avaliação):

### 1. Citações e Qualidade Textual (AV1 e AV2)
* **Regra de Ouro:** O professor recomenda **1 citação para cada 2 parágrafos**. 
* **Quantidade Mínima:** Para a entrega final (AV2), é exigido um **mínimo de 19 referências**.
* **Diversidade:** O documento deve conter referências **clássicas** (fundamentais) e **atuais** (últimos 3 anos).

### 2. Metodologia e Cronograma (AV2)
* **Atividades:** Devem ser listadas no mínimo **10 atividades** (excluindo defesa e eventos).
* **Consistência:** O cronograma (tabela) deve refletir exatamente as atividades descritas na metodologia.

---

## ✍️ Como usar o LaTeX neste Modelo

### Como fazer Citações
As citações são geradas automaticamente a partir do arquivo `referencias.bib`.
- **Citação Indireta (No final da frase):** Use `\cite{chave}`. 
  - *Exemplo:* `O aprendizado de máquina é vasto \cite{silva2024}.` -> (SILVA, 2024).
- **Citação Direta (Autor como sujeito):** Use `\citeonline{chave}`.
  - *Exemplo:* `Segundo \citeonline{knuth1984}, o TeX é...` -> Segundo Knuth (1984), o TeX é...

### Como gerenciar a Bibliografia
1.  Abra o arquivo `referencias.bib`.
2.  Adicione a entrada no formato BibTeX (você encontra isso no Google Scholar clicando em "Citar" > "BibTeX").
3.  O modelo já está configurado para **ordem alfabética** automática via estilo `abntex2-alf`.

---

## ��️ Funções Básicas do Overleaf

1.  **Recompile:** Clique no botão azul (ou `Ctrl + Enter`) para atualizar o PDF.
2.  **Logs e Erros:** Se o botão de recompile ficar laranja ou vermelho, clique no ícone de "folha" ao lado dele para ver onde está o erro no código.
3.  **Histórico:** No botão **History** no topo, você pode ver versões anteriores e restaurar o texto caso apague algo importante.
4.  **Chat e Compartilhamento:** Use o botão **Share** para adicionar seus colegas de grupo pelo e-mail. Vocês podem editar simultaneamente.
5.  **Visualização Dupla:** Clique duas vezes no PDF para ser levado à linha do código correspondente.

---

## �� Organização dos Arquivos
- `/chapters`: Cada seção tem seu próprio arquivo `.tex`. Escreva o conteúdo neles.
- `config/packages.tex`: Altere o espaçamento entre referências (`\bibitemsep`) ou cores.
- `main.tex`: Onde você define o título do trabalho e os nomes na capa.

---
**Dica Pro:** Se as referências não aparecerem, clique em **Menu** > **Clear Cached Files** (ícone da lixeira) e tente compilar novamente.