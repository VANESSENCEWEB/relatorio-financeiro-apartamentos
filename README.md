# Sistema de Relatórios Financeiros para Apartamentos

> Gerador automático de relatórios mensais em PDF com análises financeiras avançadas para gestão de apartamentos de temporada.

## Visão Geral

Este sistema automatiza a geração de relatórios financeiros mensais para apartamentos de temporada, processando dados de reservas, cauções e despesas para criar análises profissionais em PDF.

### Principais Funcionalidades

- Análises Financeiras Avançadas: Taxa de ocupação, margem líquida, receita por diária
- Controle Completo: Receitas recebidas vs pendentes, despesas pagas vs pendentes
- Indicadores de Performance: Status visual com recomendações automáticas
- Relatórios Profissionais: PDFs com design moderno e capa personalizada
- Processamento Automático: Lê planilhas Excel e gera relatórios por apartamento
- Multiplataforma: Funciona em Windows, macOS e Linux

## Instalação Rápida
```bash
# 1. Clone o repositório
git clone https://github.com/vanessarafaella/relatorio-financeiro-apartamentos.git
cd relatorio-financeiro-apartamentos

# 2. Instale as dependências
pip install -r requirements.txt

# 3. Configure seus dados
cp src/config.py src/config_local.py
# Edite config_local.py com seus dados reais

# 4. Execute o sistema
python src/gerador_relatorios.py --mes 7 --ano 2025
## Pré-requisitos

- Python 3.8+
- Pandas para manipulação de dados
- ReportLab para geração de PDFs
- OpenPyXL para leitura de arquivos Excel

## Como Usar

### Uso Básico
```bash
# Gerar relatório para julho de 2025
python src/gerador_relatorios.py --mes 7 --ano 2025

# Gerar com modo debug
python src/gerador_relatorios.py --mes 7 --ano 2025 --debug
Workflow Completo

Prepare seus dados na planilha Excel
Coloque a planilha na pasta do projeto
Execute o comando com mês e ano desejados
Encontre os PDFs na pasta Relatorios_Gerados/

Estrutura dos Dados
A planilha Excel deve ter 3 abas:
Aba "Reservas"

apartamento, hóspede, check_in, check_out, valor, status

Aba "Caucao"

apartamento, hóspede, valor_caucao, status

Aba "Despesas"

apartamento, data, categoria, valor, status

Tecnologias Utilizadas

Python - Linguagem principal
Pandas - Manipulação de dados
ReportLab - Geração de PDFs
OpenPyXL - Leitura de Excel

Licença
Este projeto está licenciado sob a Licença MIT - veja o arquivo LICENSE para detalhes.
