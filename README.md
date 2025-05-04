markdown
🚀 FURIA - KNOW YOUR FAN (BETA) - README
🇧🇷 Português

🤖 Sobre o Projeto
Versão otimizada do sistema de cadastro para fãs da FURIA, derivada do projeto original [FURIA_Know_your_fan](https://github.com/seu-usuario/FURIA_Know_your_fan), com melhorias de performance para deploy em ambientes com recursos limitados.

Principais funcionalidades:

📝 Formulário inteligente com validações robustas
🔗 Integração com Discord, Google e Steam
✉️ Sistema de e-mails personalizados via SendGrid
🗄️ Armazenamento seguro no MongoDB
⚡ Versão otimizada para deploys gratuitos

🔴 Alterações em relação à versão original:
- Remoção do módulo EasyOCR para processamento de documentos (visando reduzir consumo de memória)
- Foco nas integrações sociais e experiência do usuário
- Melhorias no gerenciamento de sessões

📦 Dependências
Crie e ative um ambiente virtual (recomendado):
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows

Instale as dependências:
pip install -r requirements.txt

⚙️ Configuração
Crie um arquivo .env na raiz do projeto com:
MONGO_URI="sua_string_de_conexao"
MONGO_DB_NAME="nome_banco"
FLASK_SECRET_KEY='sua_chave_secreta'
CLIENT_ID="123456789123456789"
CLIENT_SECRET="Laba3pTiukWlmkos-Ri6ATAEuEqjTRLQ"
GOOGLE_CLIENT_ID="123456123456123456123456"
GOOGLE_CLIENT_SECRET="sua_chave_secreta"
STEAM_API_KEY="sua_chave_steam"
SENDER_EMAIL="endereco_de_email_configurado"
SENDER_NAME="nome_do_sender_configurado"
SENDGRID_API_KEY="sua_chave_sendgrid"

🔌 Integrações OAuth (obrigatórias):

Discord Developer Portal

Google Cloud Console

Steam Developer

🚀 Como Executar

python app.py
Acesse o sistema em:

Local: http://127.0.0.1:5000

Rede local: http://192.168.15.7:5000

📬 Fluxo do Sistema

1. Cadastro básico → 2. Upload de documento → 3. Conexão social → 4. Links de interesse → 5. Confirmação e envio automático de e-mail

📧 Envio de E-mails

Disparado automaticamente ao final do cadastro

Templates personalizados baseados nos interesses do fã

Requer chave API do SendGrid válida

📌 Nota sobre Documentos:
A versão BETA mantém o upload de documentos mas não realiza processamento automático do conteúdo, focando na experiência essencial do cadastro.

📬 Contato
Para dúvidas ou sugestões:
📧 [willbc.silva@gmail.com]

👨‍💻 Desenvolvido por:
[William Bruno Carlos Silva]

🇺🇸 English
🤖 About the Project
Optimized version of the FURIA fan registration system, derived from the original FURIA_Know_your_fan project, with performance improvements for resource-limited deployments.

Key features:
📝 Smart form with robust validations
🔗 Discord, Google, and Steam integration
✉️ Personalized email system via SendGrid
🗄️ Secure MongoDB storage
⚡ Performance-optimized for free-tier deploys

🔴 Changes from original version:

Removed EasyOCR document processing module (to reduce memory usage)

Focus on social integrations and user experience

Improved session management

📦 Dependencies
Create and activate a virtual environment (recommended):
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows

Install dependencies:
pip install -r requirements.txt

⚙️ Configuration
Create a .env file in the project root with:
MONGO_URI = "your_connection_string"
MONGO_DB_NAME = "database_name"
FLASK_SECRET_KEY = 'your_secret_key'
CLIENT_ID = "123456789123456789"
CLIENT_SECRET = "Laba3pTiukWlmkos-Ri6ATAEuEqjTRLQ"
GOOGLE_CLIENT_ID = "123456123456123456123456"
GOOGLE_CLIENT_SECRET = "your_secret_key"
STEAM_API_KEY = "your_steam_key"
SENDER_EMAIL = configured_email_address  #(Sendgrid)  
SENDER_NAME = configured_sender_name  #(Sendgrid)
SENDGRID_API_KEY = "your_sendgrid_key"

Required OAuth Integrations:
Create apps on the respective platforms:
Discord Developer Portal
Google Cloud Console
Steam Developer

🚀 How to Run
Start the Flask server:
python app.py

The system will be available at:
http://127.0.0.1:5000 (local)
http://192.168.15.7:5000 (for mobile devices on the same network)

📬 System Flow
1. Basic registration → 2. Document upload → 3. Social connection → 4. Interest links → 5. Confirmation and automatic email delivery

📧 Email System
Triggered automatically upon registration completion
Uses interest-based templates
Requires valid SendGrid API key

📬 Contact
For questions:
📧 [willbc.silva@gmail.com]

👨‍💻 Developed by:
[William Bruno Carlos Silva]