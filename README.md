# Gráfico de Abalone

Análise simples em Python que calcula o comprimento médio dos abalones por categoria de sexo e salva um gráfico de barras em PNG.

## Tecnologias e dados

- Python 3, pandas e Matplotlib.
- `abalone.csv`: 4.177 registros, com cabeçalho e 9 colunas.
- Agrupamento da coluna `Sex` e média da coluna `Length`.

Categorias: `F` (fêmea), `I` (infantil) e `M` (macho).
O repositório não documenta a procedência nem a licença do CSV; confirme essas informações antes de redistribuir o conjunto de dados.

## Executar no Windows

```powershell
git clone https://github.com/Jaumbitin/grafico-abalone.git
cd grafico-abalone
python -m venv .venv
.\.venv\Scripts\python.exe -m pip install pandas matplotlib
.\.venv\Scripts\python.exe python
```

O script se chama literalmente `python`, sem extensão `.py`. Execute a partir da raiz do projeto, pois ele busca `abalone.csv` no diretório de trabalho.

No Linux/macOS, crie o ambiente com `python3 -m venv .venv` e use `.venv/bin/python` nos dois últimos comandos.

## Resultado

O arquivo `grafico_abalone_simples.png` é criado no diretório atual, com resolução de 150 dpi. A execução não abre uma janela: o gráfico é salvo e a figura é fechada.

## Estrutura e validação

- `python`: leitura, agrupamento e geração do gráfico.
- `abalone.csv`: dados usados pelo script.

Não há testes automatizados nem arquivo de dependências com versões fixadas. Confira se o PNG foi criado e se os três grupos aparecem no eixo horizontal.
