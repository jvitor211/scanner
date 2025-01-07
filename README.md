# Cyber Scanner

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)  
[![Python](https://img.shields.io/badge/python-3.10%2B-blue)](#)  
[![React](https://img.shields.io/badge/react-18.2.0-blue)](#)

Cyber Scanner é uma aplicação que escaneia redes públicas e privadas, exibindo informações detalhadas dos dispositivos conectados, como **IP**, **MAC address**, **nome do dispositivo** e **distância aproximada**. A aplicação conta com uma interface web amigável e um back-end robusto.

## 🔎 Funcionalidades

- Escaneamento de redes locais e públicas no formato CIDR.
- Exibição dos dispositivos conectados com informações:
  - Endereço IP
  - Endereço MAC
  - Nome do dispositivo
  - Distância aproximada baseada no RSSI.
- Interface web interativa.

## 📊 Tecnologias Utilizadas

### **Back-end**

- **[Python 3.10+](https://www.python.org/)**  
- **[Flask](https://flask.palletsprojects.com/)** – Framework web.
- **[Scapy](https://scapy.net/)** – Biblioteca de manipulação de pacotes de rede.
- **[SQLAlchemy](https://www.sqlalchemy.org/)** – ORM para banco de dados.

### **Front-end**

- **[React 18.2.0](https://reactjs.org/)**  
- **[Bootstrap 5](https://getbootstrap.com/)** – Framework de CSS.

## 🔧 Instalação

### **Requisitos**

- **Python 3.10+**
- **Node.js 16+**
- **Npcap** (para Windows)
- **Git**

### **Passo a passo**

#### **1. Clonar o repositório**

```bash
git clone https://github.com/seu-usuario/cyber-scanner.git
cd cyber-scanner
```

#### **2. Configurar o back-end**

```bash
cd backend
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate   # Windows
pip install -r requirements.txt
python app.py
```

#### **3. Configurar o front-end**

Abra outro terminal e execute:

```bash
cd frontend
npm install
npm start
```

## 💻 Como Usar

1. Acesse a interface web pelo navegador:  
   **`http://localhost:3000`**

2. A API pode ser acessada diretamente em:  
   **`http://localhost:5000/scan`**

3. O front-end exibirá os dispositivos conectados à rede local.

## 🗂️ Estrutura do Projeto

```plaintext
cyber-scanner/
│
├── backend/                 # Código do servidor Flask
│   ├── app.py               # Arquivo principal da API Flask
│   ├── scanner.py           # Lógica de escaneamento de rede
│   ├── distance.py          # Função para cálculo de distância
│   ├── models.py            # Modelos de banco de dados
│   └── requirements.txt     # Dependências do Python
│
├── frontend/                # Código da interface React
│   ├── public/              # Arquivos estáticos (HTML, favicon)
│   ├── src/                 # Código-fonte React
│   │   ├── components/      # Componentes da interface
│   │   ├── pages/           # Páginas principais
│   │   └── App.js           # Componente principal React
│   └── package.json         # Configuração do projeto React
│
└── README.md                # Documentação do projeto
```

## 💡 Contribuição

Contribuições são bem-vindas! Siga os passos abaixo para contribuir:

1. **Fork** este repositório.
2. Crie uma branch com sua feature:
   ```bash
   git checkout -b minha-feature
   ```
3. Commit suas alterações:
   ```bash
   git commit -m 'Adiciona minha nova feature'
   ```
4. Envie para a branch principal:
   ```bash
   git push origin minha-feature
   ```
5. Abra um **Pull Request**.

## 🛠️ Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
```

