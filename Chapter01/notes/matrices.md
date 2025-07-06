Como sabemos, uma imagem é a combinação de vários pixels - onde cada pixel tem uma cor que representa a intensidade de brilho ou cor da radiação micro-onda que voltou ao satélite -. Esse pixels podem ter um overlap devido a sua proximidade ao ser capturado, essa redundância de informação pode ser quantificada e analisada através da **Matriz de Covariância**.

## Matriz de Covariância

A matriz de covariância captura a variância de cada banda individual e a covariância entre diferentes bandas, fornecendo uma medida estatística da relação linear entre elas. Dado uma matriz $nxn$, que será determinada pela quantidade de bandas disponiveis, cada elemento fora da diagonal principal representa a covariância entre duas bandas diferentes, enquanto os elementos da diagonal principal representam a variância de cada banda individual. No caso de valores altos, há uma grande correlação entre as bandas, sugerindo uma alta redundância. Por exemplo: SSe o elemento $ C_{32} $ é muito alto e positivo, isso indica que as bandas 3 e 2 tendem a variar na mesma direção (correlação positiva); se for negativo e de grande magnitude, sugere variação oposta (correlação negativa), refletindo uma forte relação linear entre elas; Se $ C_{22} $ apresentar um valor grande, isso indica uma alta variância na banda 2, sugerindo que a intensidade dos pixels varia significativamente ao longo da imagem, possivelmente devido a fatores como mudanças em vegetação, solo ou outros alvos, dependendo do contexto. Se uma banda apresentar variância predominantemente alta (e.g., $ C_{11} $ ou $ C_{22} $ muito maior que os outros), ela pode ser priorizada no estudo, dependendo dos objetivos da análise, como maximizar a informação capturada ou simplificar o processamento.

# Análise de Componentes Principais (PCA) para Redução de Dimensionalidade

A **Análise de Componentes Principais (PCA)** é uma técnica utilizada para reduzir a dimensionalidade de um conjunto de dados, eliminando variáveis correlacionadas e destacando as direções de maior variância. Sua implementação envolve a decomposição da **matriz de covariância** \( C \), resolvendo a equação característica:

$$
Cv = \lambda v
$$

onde:
- \( v \) = autovetor (direção principal)
- \( \lambda \) = autovalor (magnitude da variância)

> **Nota:** No Python, essa decomposição pode ser feita usando `np.linalg.eigh(C)`.

---

## Interpretação dos Autovalores e Autovetores

### Autovalores (\( \lambda \))
- Representam a **importância de cada componente principal**.
- Quanto maior o autovalor, maior a variância capturada naquela direção.

### Autovetores (\( v \))
- Definem as **novas direções ortogonais** no espaço transformado.
- Cada elemento do autovetor indica o **peso** (contribuição) de uma variável original na componente principal.

---

## Exemplo Prático: Sensoriamento Remoto
Considere uma matriz de covariância 3×3 para bandas espectrais (vermelho, verde, infravermelho). Se os autovetores forem:

\[
v_1 = \begin{bmatrix} -0.733 \\ 0.677 \\ 0.071 \end{bmatrix}, \quad v_2 = \begin{bmatrix} 0.612 \\ 0.721 \\ -0.322 \end{bmatrix}
\]

- **Primeira componente (\( v_1 \))**:  
  - O valor negativo em \( c_{11} = -0.733 \) indica um **contraste** entre a banda 1 (vermelho) e as outras.  
  - Em imagens de satélite, isso pode representar que **vegetação densa** (alta reflectância no infravermelho) aparece com baixa reflectância no vermelho.  

- **Magnitude dos coeficientes**:  
  - Valores próximos de **1 ou -1** (ex.: \( 0.733 \)) indicam uma contribuição dominante daquela banda.  

---

## Ortogonalidade das Componentes Principais
Os autovetores são **ortogonais** entre si, o que significa que as componentes principais são **não correlacionadas**. Isso pode ser verificado por:

$$
U^T U = I
$$

onde:
- \( U \) = matriz de autovetores
- \( I \) = matriz identidade

**Resultado esperado:**
- **Diagonal = 1** (autovetores normalizados)
- **Fora da diagonal ≈ 0** (ortogonalidade garantida)

---

## Conclusão
A PCA permite:
1. **Reduzir a dimensionalidade** mantendo a maior variância.
2. **Identificar padrões** em dados multivariados (ex.: correlações entre bandas espectrais).
3. **Melhorar a interpretação** ao transformar os dados em componentes independentes.

**Aplicações típicas:** Sensoriamento remoto, reconhecimento de padrões, compressão de dados e machine learning.