# Workshop GitHub Actions - CI/CD

Projeto de exemplo para a prática de Integração Contínua com GitHub Actions.

## Estrutura

```
WorkShop-Git-Actions/
├── .github/
│   └── workflows/
│       └── ci.yml
├── src/
│   └── calculadora.py
├── tests/
│   └── test_calculadora.py
├── requirements.txt
└── README.md
```

## Como rodar localmente

```bash
python -m venv venv
source venv/bin/activate      # Windows: venv\Scripts\activate
pip install -r requirements.txt
pytest tests/ -v
```

## CI/CD

O pipeline de Integração Contínua roda automaticamente a cada `push` ou `pull request`
na branch `main`, executando lint (flake8) e os testes automatizados (pytest).

Veja o workflow em `.github/workflows/ci.yml`.
