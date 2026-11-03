# 🚀 Como Enviar Arquivos Locais para o GitHub

Este guia prático foi criado para ajudar você a enviar seus projetos e arquivos locais (do seu computador) para um repositório no GitHub usando o terminal/prompt de comando.

---

## 🛠️ Pré-requisitos

Certifique-se de ter os seguintes itens instalados no seu computador:
1. **Git** instalado ([Baixe e instale aqui](https://git-scm.com/)).
2. Uma conta no [GitHub](https://github.com/).

---

## 📋 Passo a Passo

### 1. Configurar o Git (Apenas na primeira vez)
Se você acabou de instalar o Git, configure seu nome de usuário e e-mail (os mesmos da sua conta do GitHub):
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu-email@example.com"
2. Criar um Repositório no GitHub
Acesse o GitHub e faça login.

No canto superior direito, clique no botão + e selecione New repository (Novo repositório).

Dê um nome para o seu repositório (ex: meu-projeto).

Escolha se ele será Public (Público) ou Private (Privado).

Importante: Nãomarque a caixa "Add a README file" (já que você vai enviar arquivos que estão no seu computador).

Clique no botão Create repository.

3. Inicializar o Git na sua pasta local
Abra o terminal (no Windows, use o Git Bash, Prompt de Comando ou PowerShell; no Mac/Linux, use o Terminal) e navegue até a pasta onde estão os seus arquivos:

Bash
cd caminho/para/a/sua/pasta
Agora, transforme essa pasta em um repositório Git executando:

Bash
git init
4. Adicionar os arquivos
Para selecionar todos os arquivos da pasta para serem enviados, digite:

Bash
git add .
5. Salvar (comitar) as alterações
Crie um "ponto de salvamento" (commit) para os seus arquivos, adicionando uma mensagem que descreva o que você está enviando:

Bash
git commit -m "Primeiro commit: enviando arquivos locais"
6. Conectar ao GitHub e Enviar
Vá até a página do repositório que você criou no GitHub (Passo 2) e copie a URL do repositório (ex: https://github.com/seu-usuario/nome-do-repositorio.git).

No seu terminal, execute os comandos abaixo:

Bash
# Define a branch principal como 'main'
git branch -M main

# Conecta o seu repositório local ao GitHub
git remote add origin <URL-DO-SEU-REPOSITORIO-NO-GITHUB>

# Envia os arquivos para o GitHub
git push -u origin main
Nota: Na primeira vez que fizer o git push, o GitHub poderá solicitar a autenticação da sua conta (via navegador ou Personal Access Token).

🎉 Pronto!
Atualize a página do seu repositório no GitHub e você verá que todos os seus arquivos locais foram enviados com sucesso!

💡 Comandos úteis para o dia a dia
Depois que o projeto já estiver conectado, para enviar futuras atualizações, basta usar:

Bash
git add .
git commit -m "Atualizando arquivos"
git push

---

Se precisar de ajuda para personalizar esse README ou tiver alguma dúvida sobre os comandos, é só falar!
