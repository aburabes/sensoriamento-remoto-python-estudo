# 📚 Análise de Imagens, Classificação e Detecção de Mudanças em Sensoriamento Remoto com Algoritmos em Python (Estudo Dirigido)

Este repositório é dedicado ao estudo e implementação dos algoritmos apresentados no livro "Image Analysis, Classification and Change Detection in Remote Sensing: With Algorithms for Algorithms for Python, Fourth Edition" de Morton John Canty. A iniciativa tem como objetivo servir como um recurso colaborativo para o nosso grupo de pesquisa, permitindo o estudo aprofundado de cada capítulo e a implementação prática dos conceitos discutidos.

## 🎯 Objetivos

* **Estudo Dirigido:** Facilitar a compreensão dos fundamentos teóricos e matemáticos de sensoriamento remoto, análise de imagens, classificação e detecção de mudanças.
* **Implementação Prática:** Replicar e estender os algoritmos apresentados no livro, utilizando a linguagem Python e bibliotecas como NumPy, SciPy, Matplotlib, GDAL, scikit-learn, TensorFlow e Google Earth Engine (GEE).
* **Colaboração:** Proporcionar um ambiente para que membros do grupo possam contribuir com suas implementações, experimentos, análises e documentação.
* **Compartilhamento de Conhecimento:** Criar uma base de conhecimento acessível e organizada para futuras consultas e projetos.

## 📦 Estrutura do Repositório

O repositório é organizado por capítulos do livro, com subpastas para código, imagens, dados e anotações, seguindo o padrão abaixo:

* **`Chapter01/`** - Capítulo 1: Imagens, Arrays e Matrizes
    * `code/` - Scripts Python e Jupyter Notebooks do capítulo.
    * `images/` - Figuras geradas pelos códigos e referências do livro.
    * `data/` - Dados específicos do capítulo.
    * `notes/` - Anotações, resumos e aprofundamentos teóricos/conceituais adicionais para o capítulo, em formato Markdown com suporte a equações LaTeX.
* **`Chapter02/`** - Capítulo 2: Estatística de Imagens
    * `code/`
    * `images/`
    * `data/`
    * **`notes/`**
* **(Capítulos 03 a 09 seguem o mesmo padrão)**
* **`auxil/`** - Módulos Python auxiliares e bibliotecas de apoio (conforme Apêndice C do livro).
* **`notebooks/`** - (Opcional) Notebooks de alto nível ou experimentos gerais que podem cruzar capítulos.
* **`README.md`** - Este arquivo principal de descrição do projeto.
* **`LICENSE`** - Arquivo com a licença do projeto (ex: MIT, Apache 2.0).
* **`.gitignore`** - Define arquivos e diretórios a serem ignorados pelo controle de versão Git.
* **`.gitattributes`** - Configurações para o Git lidar com tipos de arquivos específicos.

## 🚀 Como Contribuir

Valorizamos muito a colaboração de todos os membros do grupo. Existem duas formas principais de contribuir:

### 1. Contribuição Direta (Para membros com acesso de escrita)

Este fluxo de trabalho é para membros do grupo que possuem permissões de escrita (push) diretamente no repositório.

1.  **Clone o Repositório:** Faça uma cópia local do repositório principal.
    ```bash
    git clone [https://github.com/seu-usuario/nome-do-repositorio.git](https://github.com/seu-usuario/nome-do-repositorio.git)
    cd nome-do-repositorio
    ```
2.  **Crie um Novo Branch:** Para cada tarefa ou implementação, crie um novo branch com um nome descritivo (ex: `feature/capitulo-1-pca`, `bugfix/ex5-1-erro`).
    ```bash
    git checkout -b seu-nome/feature/descricao-da-tarefa
    ```
3.  **Implemente e Documente:**
    * Trabalhe nos arquivos relevantes dentro das pastas dos capítulos (ou `auxil/`).
    * **Crie um Jupyter Notebook (`.ipynb`)** para cada seção ou conjunto de algoritmos implementados. Explique o código passo a passo, inclua a teoria relevante (com referências ao livro), mostre os resultados (figuras e saídas), e discuta suas observações. Use a pasta `code/` do capítulo correspondente.
    * Se for um script auxiliar, adicione-o à pasta `auxil/`.
    * Certifique-se de que seu código esteja comentado e seja legível.
    * Adicione quaisquer imagens geradas para a pasta `images/` do capítulo.
    * Se usar novos dados, adicione-os à pasta `data/` do capítulo.
4.  **Teste seu Código:** Verifique se suas implementações funcionam corretamente.
5.  **Adicione e Commite suas Mudanças:**
    ```bash
    git add .
    git commit -m "feat: Implementação do algoritmo X no Capítulo Y" # Use mensagens de commit claras e concisas
    ```
6.  **Envie para o GitHub:** Envie seu novo branch e commits para o repositório remoto.
    ```bash
    git push origin seu-nome/feature/descricao-da-tarefa
    ```
7.  **Abra um Pull Request (PR):** Após o `git push`, você pode abrir um Pull Request (PR) diretamente do VS Code (utilizando a extensão "GitHub Pull Requests and Issues") ou acessando a página do repositório no GitHub. O PR será do seu branch recém-enviado para o branch `main`. Descreva o que você implementou, quaisquer desafios encontrados e como ele se relaciona com o livro.
    * **Pelo VS Code:** Após o push, o VS Code geralmente exibe uma notificação para abrir um PR, ou você pode usar o painel "Source Control" (Ctrl+Shift+G) para encontrar a opção "Create Pull Request". Selecione o branch de origem (o seu branch novo) e o de destino (`main`). Preencha os detalhes e clique em "Create".
8.  **Revisão e Discussão:** Aguarde a revisão por outros membros do grupo. Participe das discussões e faça as alterações solicitadas, se houver.

### 2. Contribuição via Fork (Para colaboradores externos ou sem acesso direto)

Se você não tem permissões de escrita direta neste repositório, pode contribuir através do processo de "fork".

1.  **Faça um Fork do Repositório:** Na página principal deste repositório no GitHub, clique no botão "Fork" (no canto superior direito). Isso criará uma cópia completa do repositório em sua própria conta do GitHub.
2.  **Clone o SEU Fork:** Clone a cópia do repositório que agora está na sua conta para sua máquina local.
    ```bash
    git clone [https://github.com/seu-usuario/seu-fork.git](https://github.com/seu-usuario/seu-fork.git) # Substitua 'seu-usuario' e 'seu-fork'
    cd seu-fork
    ```
3.  **Crie um Novo Branch:** Assim como na contribuição direta, crie um novo branch para suas alterações.
    ```bash
    git checkout -b sua-feature/nome-da-tarefa
    ```
4.  **Implemente, Documente e Teste:** Faça suas alterações e commits localmente, seguindo as diretrizes de implementação e documentação acima.
5.  **Envie para o SEU Fork:** Envie suas mudanças para o seu repositório (fork) no GitHub.
    ```bash
    git push origin sua-feature/nome-da-tarefa
    ```
6.  **Abra um Pull Request (PR) para o Repositório ORIGINAL:** Na página do seu fork no GitHub, haverá uma opção para "Contribute" ou "Open Pull Request". Crie um PR do seu branch no seu fork para o branch `main` do repositório **original**. Preencha os detalhes e clique em "Create".
7.  **Revisão e Discussão:** O mantenedor do repositório original (e outros revisores) avaliarão sua contribuição.

---

## 🛠️ Requisitos e Configuração do Ambiente

É **altamente recomendado** o uso de Docker para garantir um ambiente consistente para todos os colaboradores, conforme sugerido no Apêndice C do livro.

1.  **Instale o Docker:** Siga as instruções em [docs.docker.com/engine/installation/](https://docs.docker.com/engine/installation/).
2.  **Puxe e Execute o Contêiner Docker:**
    O livro menciona o contêiner `mort/crc5docker`.
    ```bash
    docker run -d -p 8888:8888 -v <caminho-para-seus-dados-locais>:/home/imagery/ --name=crc5 mort/crc5docker
    ```
    Substitua `<caminho-para-seus-dados-locais>` pelo caminho absoluto da pasta em seu sistema local onde você armazenará os dados de imagem maiores ou personalizados. Esta pasta estará acessível dentro do contêiner em `/home/myimagery/`. Os dados de exemplo do livro já estão em `/home/imagery/` dentro do contêiner.

    Caso não seja possível usar as imagens no Docker, baixe os arquivos de imagem presentes no seguinte link: https://drive.google.com/drive/folders/1O-J5HIpPIulxlSpq6lVV_LnZNOphtLhl?usp=drive_link e armazene-os em seu HDD/SSD, fora do diretório do projeto clonado. **É crucial não incluir esses arquivos de imagem grandes diretamente nos commits do Git, pois o GitHub bloqueia commits que contenham arquivos individuais maiores que 100 MB**. Além disso, arquivos acima de 50 MB já são fortemente desencorajados para o versionamento direto. Para gerenciar arquivos grandes versionados, a ferramenta recomendada é o Git Large File Storage (LFS).
3.  **Acesse o Jupyter Notebook:** Abra seu navegador e navegue para `http://localhost:443`.
4.  **Autenticação do Google Earth Engine (Opcional, mas Recomendado):**
    Para usar a API do GEE dentro do contêiner:
    * Abra um terminal no Jupyter Notebook (File -> New -> Terminal).
    * Execute: `earthengine authenticate` e siga as instruções.

### Extensões Recomendadas para VS Code (Para Anotações em Markdown)

Para otimizar a experiência de escrita e visualização das anotações em Markdown (localizadas nas pastas `notes/` de cada capítulo), sugerimos a instalação das seguintes extensões no seu Visual Studio Code:

1.  **Markdown All in One**
    * **Autor:** Yu Zhang
    * **Por que instalar?** Esta extensão oferece um conjunto completo de ferramentas essenciais para a escrita de Markdown no VS Code. Ela aprimora sua produtividade com atalhos de teclado, auto-completar, e um recurso de "Table of Contents" (TOC) que gera automaticamente um índice navegável para suas anotações. O suporte a matemática (equações LaTeX) também é um diferencial, garantindo que suas fórmulas sejam renderizadas corretamente na pré-visualização.
    * **Processo de Instalação:**
        1.  Abra o VS Code.
        2.  Vá para a aba de Extensões (Ctrl+Shift+X).
        3.  Procure por "Markdown All in One".
        4.  Clique em "Install".

2.  **Markdown Preview Enhanced**
    * **Autor:** Yiyi Wang
    * **Por que instalar?** Esta extensão eleva a pré-visualização do Markdown no VS Code a outro nível. Ela fornece funcionalidades úteis como sincronização automática da rolagem entre o editor e a pré-visualização, tipografia de matemática (MathJax/KaTeX) de alta qualidade para suas equações LaTeX, exportação para PDF ou HTML, e suporte para trechos de código (code chunks). É ideal para garantir que suas anotações com fórmulas matemáticas complexas sejam exibidas de forma clara e profissional.
    * **Processo de Instalação:**
        1.  Abra o VS Code.
        2.  Vá para a aba de Extensões (Ctrl+Shift+X).
        3.  Procure por "Markdown Preview Enhanced".
        4.  Clique em "Install".

Com essas extensões, você terá um ambiente robusto no VS Code para criar anotações ricas em texto, código (em notebooks) e matemática, tudo de forma integrada e eficiente.

---

## 📚 Referência do Livro

Canty, Morton John. (2019). *Image Analysis, Classification and Change Detection in Remote Sensing: With Algorithms for Python, Fourth Edition*. Chapman and Hall/CRC.
