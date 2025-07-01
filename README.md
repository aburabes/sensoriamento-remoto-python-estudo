# 📚 Análise de Imagens, Classificação e Detecção de Mudanças em Sensoriamento Remoto com Algoritmos em Python (Estudo Dirigido)

Este repositório é dedicado ao estudo e implementação dos algoritmos apresentados no livro "Image Analysis, Classification and Change Detection in Remote Sensing: With Algorithms for Python, Fourth Edition" de Morton John Canty. A iniciativa tem como objetivo servir como um recurso colaborativo para o nosso grupo de pesquisa, permitindo o estudo aprofundado de cada capítulo e a implementação prática dos conceitos discutidos.

## 🎯 Objetivos

* **Estudo Dirigido:** Facilitar a compreensão dos fundamentos teóricos e matemáticos de sensoriamento remoto, análise de imagens, classificação e detecção de mudanças.
* **Implementação Prática:** Replicar e estender os algoritmos apresentados no livro, utilizando a linguagem Python e bibliotecas como NumPy, SciPy, Matplotlib, GDAL, scikit-learn, TensorFlow e Google Earth Engine (GEE).
* **Colaboração:** Proporcionar um ambiente para que membros do grupo possam contribuir com suas implementações, experimentos, análises e documentação.
* **Compartilhamento de Conhecimento:** Criar uma base de conhecimento acessível e organizada para futuras consultas e projetos.

## 📦 Estrutura do Repositório

O repositório é organizado por capítulos do livro, com subpastas para código, imagens e dados:
├── Chapter01/              # Capítulo 1: Imagens, Arrays e Matrizes
│   ├── code/               # Scripts Python e Jupyter Notebooks do capítulo
│   ├── images/             # Figuras geradas pelos códigos e referências do livro
│   └── data/               # Dados específicos do capítulo
├── Chapter02/              # Capítulo 2: Estatística de Imagens
│   ├── code/
│   ├── images/
│   └── data/

... Capítulos (03 a 09 seguem o mesmo padrão)
├── auxil/                  # Módulos Python auxiliares e bibliotecas de apoio (Apêndice C do livro)
└── README.md               # Este arquivo


## 🚀 Como Contribuir

Valorizamos muito a colaboração de todos os membros do grupo. Siga estas diretrizes para contribuir:

1.  **Clone o Repositório:**
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
6.  **Envie para o GitHub:**
    ```bash
    git push origin seu-nome/feature/descricao-da-tarefa
    ```
7.  **Abra um Pull Request (PR):** Vá para a página do repositório no GitHub e abra um Pull Request do seu branch para o branch `main`. Descreva o que você implementou, quaisquer desafios encontrados e como ele se relaciona com o livro.
8.  **Revisão e Discussão:** Aguarde a revisão por outros membros do grupo. Participe das discussões e faça as alterações solicitadas, se houver.

## 🛠️ Requisitos e Configuração do Ambiente

É **altamente recomendado** o uso de Docker para garantir um ambiente consistente para todos os colaboradores, conforme sugerido no Apêndice C do livro.

1.  **Instale o Docker:** Siga as instruções em [docs.docker.com/engine/installation/](https://docs.docker.com/engine/installation/).
2.  **Puxe e Execute o Contêiner Docker:**
    O livro menciona o contêiner `mort/crc5docker`.
    ```bash
    docker run -d -p 8888:8888 -v <caminho-para-seus-dados-locais>:/home/imagery/ --name=crc5 mort/crc5docker
    ```
    Substitua `<caminho-para-seus-dados-locais>` pelo caminho absoluto da pasta em seu sistema local onde você armazenará os dados de imagem maiores ou personalizados. Esta pasta estará acessível dentro do contêiner em `/home/myimagery/`. Os dados de exemplo do livro já estão em `/home/imagery/` dentro do contêiner.
    Caso não seja possível usar as imagens no docker, baixe as imagens presentes no seguinte link: 
3.  **Acesse o Jupyter Notebook:** Abra seu navegador e navegue para `http://localhost:443`.
4.  **Autenticação do Google Earth Engine (Opcional, mas Recomendado):**
    Para usar a API do GEE dentro do contêiner:
    * Abra um terminal no Jupyter Notebook (File -> New -> Terminal).
    * Execute: `earthengine authenticate` e siga as instruções.

## 📚 Referência do Livro

Canty, Morton John. (2019). *Image Analysis, Classification and Change Detection in Remote Sensing: With Algorithms for Python, Fourth Edition*. Chapman and Hall/CRC.

---
