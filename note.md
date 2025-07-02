## 1. Satélites Passivos  
**Como funcionam?**  
- Captam a radiação natural refletida ou emitida pela superfície terrestre (luz solar, calor, etc.).  
- Não emitem seu próprio sinal, apenas registram a energia que chega até eles.  

**Tipos de Sensores Passivos:**  
- **Câmeras multiespectrais/hiperespectrais** (registram várias bandas do espectro eletromagnético).  
- **Termais** (captam radiação infravermelha térmica).  

**Exemplos de Satélites Passivos:**  
- **Landsat** (NASA/USGS) – Multiespectral e termal.  
- **Sentinel-2** (ESA) – Multiespectral (13 bandas).  
- **CBERS** (INPE/China) – Multiespectral.  

### **Imagens Multiespectrais**  
- Registram a mesma cena em **diferentes bandas espectrais** (visível, infravermelho, etc.).  
- **Aplicações:**  
  - **Agricultura** (saúde da vegetação – NDVI).  
  - **Monitoramento ambiental** (desmatamento, queimadas).  
  - **Água** (detecção de poluição, sedimentos).  

**Exemplo de bandas do Sentinel-2:**  
- Banda 2 (Azul), Banda 3 (Verde), Banda 4 (Vermelho), Banda 8 (Infravermelho próximo).  

---

## **2. Satélites Ativos**  
**Como funcionam?**  
- Emitem seu próprio sinal (micro-ondas, laser) e captam o retorno.  
- Funcionam independentemente da luz solar (podem operar à noite ou em condições de nuvens).  

**Tipos de Sensores Ativos:**  
- **Radar de Abertura Sintética (SAR)** – Usa micro-ondas.  
- **LiDAR** – Usa pulsos de laser para medição de altitude.  

**Exemplos de Satélites Ativos:**  
- **Sentinel-1** (ESA) – SAR (C-band).  
- **TerraSAR-X** (Alemanha) – SAR (X-band, alta resolução).  
- **ALOS/PALSAR** (Japão) – SAR (L-band, penetração em florestas).  

### **Imagens de Radar (SAR – Synthetic Aperture Radar)**  
- Funciona em **micro-ondas**, podendo penetrar nuvens e vegetação.  
- **Aplicações:**  
  - **Monitoramento de desastres** (enchentes, deslizamentos mesmo com céu nublado).  
  - **Agricultura** (umidade do solo, estrutura da plantação).  
  - **Geologia** (detecção de deformações do solo – interferometria).  

**Características do SAR:**  
- **Polarização** (HH, VV, HV, VH) – Define como a onda interage com a superfície.  
- **Banda (C, X, L, P)** – Influencia na penetração (L-band é melhor para florestas).  

---

## **Comparação: Multiespectral vs. SAR**  
| **Característica**       | **Imagens Multiespectrais** | **Imagens SAR (Radar)** |  
|--------------------------|----------------------------|------------------------|  
| **Fonte de Energia**     | Luz solar (passivo)        | Micro-ondas (ativo)    |  
| **Resolução Espacial**   | Alta (até <1m)             | Moderada a Alta (1m–20m)|  
| **Influência do Tempo**  | Afetada por nuvens         | Funciona em qualquer condição |  
| **Aplicação Principal**  | Vegetação, água, uso do solo | Movimento do solo, desastres |  
