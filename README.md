# JouPIP – IA Autônoma para Análise de Mercado Forex (Renko & Tick)

## Pré-requisitos
- Python 3.9+
- Git instalado
- SQLite3
- Navegador moderno

## Instalação
```bash
git clone https://github.com/JouLABS/joupip.git
cd joupip
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt
```

## Execução
```bash
streamlit run dashboard/app.py
```

## Funcionalidades
- Simulação Renko com agressões (cTrader-style)
- IA com aprendizado não supervisionado (HDBSCAN)
- Previsões em tempo real com probabilidades
- Painel técnico com indicadores e parâmetros configuráveis
- Banco SQLite com modo simulado e real
- Checklist visual das condições atendidas

## Alternar Modo
- [Simulado] – processa mas não salva no banco
- [Real] – grava padrões reais em SQL para aprendizado contínuo

## Recalcular Indicadores
```bash
python scripts/recalcular_indicadores.py --start "2023-01-01" --end "2023-12-31"
```
