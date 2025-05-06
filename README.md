
# Password Manager

Este é um gerenciador de senhas simples com interface gráfica (web) e modo de linha de comando (CLI), que permite armazenar e proteger senhas de forma segura utilizando criptografia.

## 📁 Estrutura do Projeto

```
password_manager/
│
├── app.py                     # Inicializa a aplicação web Flask
├── cli.py                     # Interface de linha de comando
├── cli_password_manager.py    # Lógica de gerenciamento via CLI
├── crypto.py                  # Funções de criptografia
├── main.py                    # Ponto de entrada principal
├── password_manager.py        # Lógica principal do gerenciador
│
├── templates/                 # Templates HTML (login, registro, dashboard)
│   ├── base.html
│   ├── login.html
│   ├── register.html
│   └── dashboard.html
│
├── static/                    # Arquivos estáticos (CSS e JS)
│   ├── css/
│   │   └── style.css
│   └── js/
│       └── main.js
│
├── data/                      # Armazena usuários e senhas em arquivos JSON
│   ├── users.json
│   └── *_passwords.json
│
└── README.md
```

## 🚀 Como executar

### Web (Flask)
```bash
python app.py
```

### CLI
```bash
python cli.py
```

## 🛡️ Segurança
As senhas são protegidas usando criptografia definida no arquivo `crypto.py`.

## ✅ Requisitos
- Python 3.x
- Flask (`pip install flask`)

> É recomendado criar um ambiente virtual:
```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate   # Windows
pip install flask
```

## 📌 Observações
- Os dados são salvos localmente em arquivos `.json`.
- Não armazene dados sensíveis em produção com este projeto sem adaptações de segurança adicionais.

---

Desenvolvido por [kauaonpercss](https://github.com/kauaonpercss)
