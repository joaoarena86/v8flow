# ⚡ V8Flow Pro

### Workflow Manager Premium com Firebase

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![Firebase](https://img.shields.io/badge/Firebase-10.8.0-orange)
![License](https://img.shields.io/badge/license-MIT-green)

---

## 🎯 Sobre o Projeto

**V8Flow Pro** é um gerenciador de workflows profissional com design premium, desenvolvido para ajudar você a organizar projetos, tarefas e processos de forma visual e intuitiva.

Com ele, você pode criar workflows com etapas sequenciais (uma depende da outra), adicionar prazos, status, sub-etapas e comentários em cada etapa.

---

## ✨ Funcionalidades

| Funcionalidade | Descrição |
|----------------|-----------|
| 🔐 **Autenticação** | Login e registro com Firebase (email/senha real) |
| 📁 **Workflows** | Criar, selecionar e excluir workflows |
| 📌 **Etapas Sequenciais** | Etapa só libera após concluir a anterior |
| 🏷️ **Status** | Pendente / Em Andamento / Concluída |
| 📅 **Prazos** | Data de vencimento por etapa (atraso fica vermelho) |
| ✅ **Sub-etapas** | Checklist dentro de cada etapa |
| 💬 **Comentários** | Adicionar comentários por etapa |
| 📊 **Dashboard** | Estatísticas + Barra de progresso |
| 🕒 **Relógio** | Data e hora em tempo real |
| ⚙️ **Configurações** | Alterar senha, excluir conta, excluir todos workflows |
| 🎨 **Design Premium** | Glassmorphism, grid animado, partículas flutuantes |

---

## 🛠️ Tecnologias Utilizadas

| Tecnologia | O que faz |
|------------|-----------|
| **HTML5** | Estrutura da aplicação |
| **CSS3** | Estilização premium (glassmorphism, animações) |
| **JavaScript (Vanilla)** | Lógica do app, manipulação do DOM |
| **Firebase Auth** | Autenticação de usuários (email/senha) |
| **Firebase Firestore** | Banco de dados em tempo real na nuvem |
| **Font Awesome** | Ícones vetoriais |
| **Google Fonts (Inter)** | Tipografia moderna |

---

## 🎨 Design Features

| Feature | Descrição |
|---------|-----------|
| Glassmorphism | Cards com vidro fosco (blur + transparência 40%) |
| Grid Animado | Linhas se movendo no fundo |
| Radar Pulsante | Círculos concêntricos |
| Partículas Flutuantes | Pontinhos subindo pela tela |
| Hover Effects | Botões e cards com glow e elevação |
| Gradientes | Cores em degradê (azul → rosa) |
| Responsivo | Funciona em celular, tablet e desktop |

---

## 📦 Como Instalar e Executar

### Pré-requisitos

- Navegador moderno (Chrome, Firefox, Edge, Safari)
- Conta Firebase (opcional, o app já está configurado)

### Passos

1. **Baixar o arquivo** `v8flow_firebase.html`

2. **Abrir no navegador**
   - Clique duas vezes no arquivo
   - Ou arraste para dentro do navegador

3. **Criar uma conta**
   - Clique em "Criar Conta"
   - Digite nome, email e senha (mínimo 6 caracteres)

4. **Começar a usar**
   - Crie workflows
   - Adicione etapas com prazos
   - Marque como concluídas
   - Adicione sub-etapas e comentários

---

## 🗂️ Estrutura de Dados (Firebase)

```javascript
// Coleção: users
{
  uid: {
    name: "João",
    email: "joao@email.com"
  }
}

// Coleção: workflows
{
  id_do_workflow: {
    userId: "uid_do_usuario",
    name: "Nome do Workflow",
    currentIdx: 0,
    steps: [
      {
        name: "Etapa 1",
        dueDate: "2026-12-31",
        status: "pending" // pending, progress, completed
      }
    ],
    createdAt: timestamp
  }
}
