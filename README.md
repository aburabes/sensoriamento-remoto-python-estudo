# 📚 Análise de Imagens, Classificação e Detecção de Mudanças em Sensoriamento Remoto com Algoritmos em Python (Estudo Dirigido)

Este repositório é dedicado ao estudo e implementação dos algoritmos apresentados no livro "Image Analysis, Classification and Change Detection in Remote Sensing: With Algorithms for Algorithms for Python, Fourth Edition" de Morton John Canty. A iniciativa tem como objetivo servir como um recurso colaborativo para o nosso grupo de pesquisa, permitindo o estudo aprofundado de cada capítulo e a implementação prática dos conceitos discutidos.

## 🎯 Objetivos

* **Estudo Dirigido  e Compreensão Aprofundada:** Facilitar a compreensão dos fundamentos teóricos e matemáticos de sensoriamento remoto, análise de imagens, classificação e detecção de mudanças, baseando-se nas explicações passo a passo do livro.
* **Implementação Prática:** Replicar e estender os algoritmos apresentados no livro, utilizando a linguagem Python e bibliotecas como NumPy, SciPy, Matplotlib, GDAL, scikit-learn, TensorFlow e Google Earth Engine (GEE). O foco é na criação de **Jupyter Notebooks interativos** para a visualização e entendimento do comportamento dos algoritmos.
* **Colaboração:** Proporcionar um ambiente para que membros do grupo possam contribuir com suas implementações, experimentos, análises e documentação.
* **Compartilhamento de Conhecimento:** Criar uma base de conhecimento acessível e organizada para futuras consultas e projetos.

## 💡 Filosofia de Estudo e Melhores Práticas

Para otimizar o aprendizado e a colaboração, sugerimos as seguintes práticas:

* **Compreensão em Camadas:** Para cada algoritmo ou conceito, procure entender a **intuição** por trás dele, em seguida, os **fundamentos matemáticos** (utilizando as anotações e o Apêndice A do livro), e só então a **implementação em Python**.
* **Engajamento Ativo:** Não se limite a copiar o código. Tente reescrevê-lo, adaptar exemplos e explorar os parâmetros dos algoritmos.
* **Discussão e Reflexão:** Utilize as anotações para levantar "perguntas para reflexão" e pontos de discussão, como as "pegadinhas" ou trechos mais complexos do livro.
* **Resolução de Exercícios:** Os exercícios propostos no final de cada capítulo são cruciais para solidificar o aprendizado. Tente resolvê-los independentemente antes de consultar qualquer solução.

## 📦 Estrutura do Repositório

Este repositório é organizado por capítulos do livro "Image Analysis, Classification and Change Detection in Remote Sensing" (4ª edição) de Morton John Canty, com subpastas para código, imagens, dados e anotações, seguindo o padrão abaixo:

-   **`ChapterXX/`**: Pastas dedicadas a cada capítulo (ex: `Chapter01`, `Chapter02`, etc.).
    -   **`code/`**: Contém Jupyter Notebooks com exemplos e ilustrações de conceitos do capítulo. Estes notebooks devem focar em **implementações diretamente relacionadas e exclusivas a exemplos específicos do capítulo**, explicando o código passo a passo.
    -   **`images/`**: Figuras geradas pelos códigos e referências visuais do livro.
    -   **`data/`**: Dados específicos utilizados ou gerados no capítulo.
    -   **`notes/`**: Anotações, resumos e aprofundamentos teóricos/conceituais adicionais para o capítulo, em formato Markdown com suporte a equações LaTeX.
    -   **`exercises/`**: (Opcional) Contém Jupyter Notebooks ou scripts Python com as tentativas de resolução dos exercícios propostos no final de cada capítulo do livro.

-   **`auxil/`**: Contém módulos Python auxiliares e bibliotecas de apoio, conforme o Apêndice C do livro.Estes scripts são de propósito geral e podem ser reutilizados em diferentes capítulos.
    -   **`auxil_modules/`**: Subpasta para módulos Python que são importados por outros scripts ou notebooks (ex: `auxil1.py`, `supervisedclass.py`, `readshp.py`, `eeMad.py`, `eeWishart.py`).
    * **`scripts/`**: Contém todos os scripts Python de linha de comando (`.py`) e scripts shell (`.sh`) fornecidos no Apêndice C.4 do livro. Estes são utilitários de propósito geral (ex: `adaboost.py`, `atwt.py`, `classify.py`, `dispms.py`, `iMad.py`, `pca.py`, `sar_seqQ.py`)
    * **`scripts/exercises/`**: Contém todos os scripts Python de linha de comando (`.py`) fornecidos em cada capítulo do livro. Estes são feitos para a resolução de exercícios de exemplo dentro de cada capítulo.

-   **`notebooks/`**: (Opcional) Notebooks de alto nível ou experimentos gerais que podem cruzar capítulos, se não se encaixarem diretamente em uma pasta de capítulo específica.

-   **`README.md`**: Este arquivo principal de descrição do projeto.
-   **`LICENSE`**: Arquivo com a licença do projeto.
-   **`.gitignore`**: Define arquivos e diretórios a serem ignorados pelo controle de versão Git.
-   **`.gitattributes`**: Configurações para o Git lidar com tipos de arquivos específicos.

### 🐍 Scripts Python

Os scripts Python mencionados no Apêndice C.4 do livro, que ilustram os algoritmos e métodos de processamento de imagens de sensoriamento remoto, devem ser colocados na pasta **`auxil/scripts/`**. 

**Como usar os scripts nos Jupyter Notebooks:**

Nos Jupyter Notebooks localizados nas pastas `ChapterXX/code/` ou `notebooks/`, você pode executar esses scripts usando o comando `%run` ou `!python`, especificando o caminho relativo a partir da raiz do seu repositório. Por exemplo:

```python
# Exemplo de chamada de script PCA a partir de um Jupyter Notebook
%run auxil/scripts/pca.py -p [1,2,3] imagery/minha_imagem.tif
```
## 🚀 Como Contribuir

Valorizamos muito a colaboração de todos os membros do grupo. Existem duas formas principais de contribuir:

### 1. Contribuição Direta (Para colaboradores com permissão de escrita)

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
    * Se for um script auxiliar, adicione-o à pasta `auxil/auxil_modules/` ou `auxil/scripts/`.
    * Se for a resolução de um exercício, adicione-o à pasta `ChapterXX/exercises/`.
    * Certifique-se de que seu código esteja comentado e seja legível.
    * Adicione quaisquer imagens geradas para a pasta `images/` do capítulo.
    * Se usar novos dados, adicione-os à pasta `data/` do capítulo (evite arquivos grandes diretamente).
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

O livro **recomenda** o uso de Docker por ser a maneira mais fácil de executar o software e códigos, conforme dito no Apêndice C do livro.

1.  **Instale o Docker:** Siga as instruções em [docs.docker.com/engine/installation/](https://docs.docker.com/engine/installation/).
2.  **Puxe e Execute o Contêiner Docker:**
    Na quarta edição o livro utiliza o contêiner `mort/crc4docker`, mas este já está inutilizável. Na quinta edição é utilizado o contêiner `mort/crc5docker`. Então, use o seguinte comando:
    ```bash
    docker run -d -p 8888:8888 -v <caminho-para-seus-dados-locais>:/home/imagery/ --name=crc5 mort/crc5docker
    ```
    Substitua `<caminho-para-seus-dados-locais>` pelo caminho absoluto da pasta em seu sistema local onde você armazenará os dados de imagem maiores ou personalizados. Esta pasta estará acessível dentro do contêiner em `/home/myimagery/`. Os dados de exemplo do livro já estão em `/home/imagery/` dentro do contêiner.

    Caso não seja possível usar o Docker, baixe os arquivos de imagem presentes no seguinte link: https://drive.google.com/drive/folders/1O-J5HIpPIulxlSpq6lVV_LnZNOphtLhl?usp=drive_link e armazene-os em seu HDD/SSD, fora do diretório do projeto clonado. **É crucial não incluir esses arquivos de imagem grandes diretamente nos commits do Git, pois o GitHub bloqueia commits que contenham arquivos individuais maiores que 100 MB**. Além disso, arquivos acima de 50 MB já são fortemente desencorajados para o versionamento direto. Para gerenciar arquivos grandes versionados, a ferramenta recomendada é o Git Large File Storage (LFS).
4. **Controle do Contêiner Docker**
   * Para parar o contêiner: `docker stop crc5`.
   * Para reiniciar o contêiner: `docker start crc5`.    
4.  **Acesse o Jupyter Notebook:** Abra seu navegador e navegue para `http://localhost:443`.
5.  **Autenticação do Google Earth Engine (Opcional, mas Recomendado):**
    Para usar a API do GEE dentro do contêiner:
    * Abra um terminal no Jupyter Notebook (File -> New -> Terminal).
    * Execute: `earthengine authenticate` e siga as instruções.

### Extensões Recomendadas para VS Code

Para garantir a funcionalidade básica e um ambiente de desenvolvimento robusto para Python e Jupyter Notebooks no Visual Studio Code, recomendamos a instalação das seguintes extensões:

1.  **Python**
    * **Autor:** Microsoft
    * **Por que instalar?** Esta é a extensão fundamental para desenvolvimento Python no VS Code. Ela oferece suporte abrangente à linguagem, incluindo IntelliSense (auto-completar), depuração (debugging), linting (para identificar erros e problemas de estilo), formatação de código, refatoração, e suporte a testes de unidade. É essencial para tornar o Python "rodável" no seu IDE (Integrated Development Environment).
    * **Processo de Instalação:**
        1.  Abra o VS Code.
        2.  Vá para a aba de Extensões (Ctrl+Shift+X).
        3.  Procure por "Python".
        4.  Clique em "Install".
            * *Observação:* A instalação desta extensão geralmente inclui automaticamente "Pylance" e "Python Debugger", que são componentes chave para a experiência Python completa.

2.  **Jupyter**
    * **Autor:** Microsoft
    * **Por que instalar?** Esta extensão é o coração do suporte a Jupyter Notebooks no VS Code. Ela permite a execução interativa de código em células, suporte a IntelliSense para notebooks, depuração de células, visualização de saídas complexas (gráficos, tabelas), e muito mais. É indispensável para trabalhar com os notebooks do projeto.
    * **Processo de Instalação:**
        1.  Abra o VS Code.
        2.  Vá para a aba de Extensões (Ctrl+Shift+X).
        3.  Procure por "Jupyter".
        4.  Clique em "Install".
            * *Observação:* A instalação desta extensão pode incluir automaticamente outras extensões relacionadas a Jupyter (como "Jupyter Cell Tags", "Jupyter Keymap", "Jupyter Notebook Renderers" e "Jupyter Slide Show"), garantindo o suporte completo para notebooks.

Para otimizar a experiência de escrita e visualização das anotações em Markdown (localizadas nas pastas `notes/` de cada capítulo), sugerimos a instalação das seguintes extensões no seu Visual Studio Code:

1.  **Markdown All in One**
    * **Autor:** Yu Zhang
    * **Por que instalar?** Esta extensão eleva a pré-visualização do Markdown no VS Code a outro nível. Ela fornece funcionalidades úteis como sincronização automática da rolagem entre o editor e a pré-visualização, tipografia de matemática (MathJax/KaTeX) de alta qualidade para suas equações LaTeX, exportação para PDF ou HTML, e suporte para trechos de código (code chunks). É ideal para garantir que suas anotações com fórmulas matemáticas complexas sejam exibidas de forma clara e profissional.
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
