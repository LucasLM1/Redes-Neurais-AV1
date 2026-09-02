# Perceptron e Adaline — Porta Lógica AND

Implementação dos dois modelos clássicos de neurônio artificial em Python puro, treinados para reproduzir a porta lógica AND.

## Dependências

- Python 3.8+
- `numpy`
- `matplotlib`
- `notebook` (Jupyter)

## Instalação

```bash
pip install numpy matplotlib notebook ipykernel
```

## Como rodar

1. Clone ou baixe este repositório
2. Abra o terminal na pasta do projeto
3. Execute:

```bash
python -m jupyter notebook
```

4. No navegador, abra o arquivo `perceptron_adaline.ipynb`
5. No menu: **Kernel → Restart & Run All**

> A Parte 3 (predição interativa) vai pausar aguardando entrada do usuário. Digite o modelo desejado (`perceptron` ou `adaline`), os valores de `x1` e `x2`, e `sair` para encerrar e continuar o notebook.

## Estrutura do projeto

```
.
├── perceptron_adaline.ipynb   # notebook principal
├── curvas_aprendizado.png     # gerado ao executar a Parte 4
└── README.md
```

## Conteúdo do notebook

| Parte | Descrição |
|-------|-----------|
| 1 | Perceptron — Regra de Rosenblatt |
| 2 | Adaline — Regra Delta (Widrow-Hoff) |
| 3 | Predição interativa com tratamento de entrada inválida |
| 4 | Comparação: gráficos, tabela e análise textual |

## Convenção de dados

| x₁ | x₂ | d (saída desejada) |
|----|----|--------------------|
| 0  | 0  | -1                 |
| 0  | 1  | -1                 |
| 1  | 0  | -1                 |
| 1  | 1  | +1                 |

- Entradas binárias (0 e 1), saída bipolar (-1 e +1)
- Bias incluído como peso `w₀` com entrada fixa `x₀ = 1`
- Função de ativação na predição: sinal (`+1` se `w·x ≥ 0`, senão `-1`)
