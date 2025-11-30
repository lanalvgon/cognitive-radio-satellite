# Sensoriamento Espectral Inteligente para Coexistência em Mega-Constelações de Satélites LEO

Este repositório contém a implementação de um sistema de Rádio Cognitivo baseado em Deep Learning (CNN) para alocação dinâmica de espectro em cenários de satélites.

![Acurácia vs SNR](images/acuracia_snr.png)

## Sobre o Projeto
O objetivo é mitigar a interferência entre constelações LEO e serviços existentes utilizando inteligência artificial para detecção de sinais e acesso oportunista ao espectro.

**Tecnologias:** TensorFlow, Keras, Python, HDF5.
**Dataset:** RadioML 2018.01A (DeepSig).

## Funcionalidades
- **Pipeline de Dados Otimizado:** Gerador customizado com `tf.data` e prefetching para processar 20GB+ de dados.
- **Classificador CNN:** Modelo treinado para identificar 24 modulações (DVB-S2).
- **Agente Cognitivo:** Simulação de alocação de canais com detecção híbrida (Energia + IA).

## Resultados
- Acurácia em alto SNR: >90% (estimado)
- Taxa de sucesso do Agente na simulação: 100% (sem colisões)

## Como Executar
1. Clone este repositório.
2. Baixe o dataset [RadioML 2018.01A](https://www.kaggle.com/datasets/pinxau1000/radioml2018).
3. Instale as dependências:
   ```bash
   pip install -r requirements.txt