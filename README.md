<p align="center">
  <!-- Opcional: Adicione o logo da "diretoai" aqui -->
  <img src="https://github.com/user-attachments/assets/8f56aa4f-5fc7-4e3b-a14f-55e2c254d477" alt="Logo diretoai" width="200"/>
</p>

<h1 align="center">DiretoAI - Gestão com IA - http://diretoai.shop</h1>

<p align="center">
  Plataforma web para gerenciamento de estoque, integrada a um agente de automação n8n para controle inteligente de reservas e baixas de produtos.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/status-ativo-success" alt="Status do Projeto">
  <img src="https://img.shields.io/badge/React-18.3-blue?logo=react" alt="React">
  <img src="https://img.shields.io/badge/TypeScript-5.5-blue?logo=typescript" alt="TypeScript">
  <img src="https://img.shields.io/badge/TailwindCSS-3.4-blue?logo=tailwindcss" alt="Tailwind CSS">
  <img src="https://img.shields.io/badge/Supabase-2.4-green?logo=supabase" alt="Supabase">
</p>

<p align="center">
  <a href="#-visão-geral">Visão Geral</a> •
  <a href="#-funcionalidades">Funcionalidades</a> •
  <a href="#-acesso-ao-sistema">Acesso</a> •
  <a href="#️-tecnologias-utilizadas">Tecnologias</a> •
  <a href="#-licença">Licença</a>
</p>

---

## 📖 Visão Geral

A **diretoai** é a interface de usuário (front-end) para um sistema de controle de estoque inteligente. A lógica de negócio principal, como a criação de reservas de produtos, é gerenciada por um **agente de automação ("IA") construído em n8n**.

O sistema foi desenvolvido para resolver a necessidade de um cliente de visualizar e gerenciar de forma clara e eficiente as reservas de produtos criadas pelo agente. Ele permite que os usuários autorizados não apenas monitorem o que foi reservado, mas também processem essas reservas ("dando baixa" no estoque) e administrem o catálogo de produtos de forma completa, com uma interface moderna e responsiva.

## ✨ Funcionalidades

- **🔐 Autenticação Segura:** Tela de login com usuário e senha gerenciada via Supabase.
- **📊 Dashboard de Reservas:** Visualização clara e em tempo real dos produtos reservados pelo agente n8n.
- **📈 Gráficos Interativos:** Painéis com gráficos (usando Recharts) para análise de dados do estoque.
- **✅ Baixa de Produtos:** Funcionalidade para processar uma reserva e efetivamente remover o item do estoque.
- **📦 Gestão de Produtos:** CRUD completo para cadastrar, editar e remover produtos, com informações detalhadas e grades.
- **🖼️ Upload de Imagens:** Suporte para upload de fotos com arrastar e soltar (Drag-and-Drop) para cada produto.
- **🌙 Tema Dark/Light:** Interface com suporte a temas claro e escuro para melhor conforto visual.
- **🔔 Notificações:** Feedbacks visuais elegantes (toasts) para ações do usuário, como "Produto salvo com sucesso".
- **📱 Design Responsivo:** A interface é totalmente compatível com desktops, tablets e celulares.

## 🚀 Acesso ao Sistema

Este é um aplicativo web (SaaS) e não requer instalação por parte do usuário final.

1.  **Acesse o link:** [**diretoai**](https://www.diretoai.shop/auth)
2.  **Faça o login:** Utilize o usuário e senha fornecidos.
3.  **Pronto!** Você já pode utilizar o sistema.

## 🎥 Screenshots

**Tela de Login:**
![image](https://github.com/user-attachments/assets/3483b3e8-11d8-4043-8c6c-a8ec9cc96289)


**Dashboard de Estoque (Exemplo):**
![image](https://github.com/user-attachments/assets/ae0b3a8e-8019-49c6-a48f-eaa1f339bd89)
![image](https://github.com/user-attachments/assets/68808ad9-edc9-4b6c-9a19-505f2b25ce16)


## 🛠️ Tecnologias Utilizadas

Este projeto foi construído com um stack de tecnologias moderno e robusto, focado em performance, escalabilidade e experiência do desenvolvedor.

| Categoria | Tecnologia | Descrição |
| :--- | :--- | :--- |
| **Framework & Build** | `React`, `Vite`, `TypeScript` | UI construída com React e tipada com TypeScript, utilizando Vite para um build e dev server ultra-rápido. |
| **Estilização & UI** | `Tailwind CSS`, `shadcn/ui` | Framework CSS utility-first e um sistema de componentes acessíveis e customizáveis. |
| **Backend & Database**| `Supabase` | Backend-as-a-Service para banco de dados PostgreSQL, autenticação e armazenamento de arquivos. |
| **Gerenciamento de Estado**| `TanStack Query`, `Context API` | Gerenciamento de estado do servidor (caching, re-fetching) e estado global da aplicação. |
| **Formulários & Validação**| `React Hook Form`, `Zod` | Construção de formulários performáticos com validação de schemas baseada em TypeScript. |
| **Roteamento** | `React Router DOM` | Gerenciamento de rotas e navegação na aplicação. |
| **Componentes & UX** | `Radix UI`, `Lucide Icons`, `Sonner` | Primitivos de UI, ícones, toasts, carrosséis, gráficos e outros componentes para uma UX rica. |
| **Agente de Automação**| `n8n` | Plataforma de automação que gerencia a lógica de negócio de reserva de produtos. |

<br>

<details>
  <summary><strong>🏗️ Arquitetura e Padrões de Projeto (Clique para expandir)</strong></summary>
  
  - **Arquitetura Modular:** O projeto é organizado em módulos de funcionalidades (produtos, usuários, auth) para facilitar a manutenção e escalabilidade.
  - **Tipagem Forte (Type Safety):** O uso intensivo de TypeScript e Zod garante a segurança dos tipos em toda a aplicação, do formulário ao banco de dados.
  - **Custom Hooks:** Lógica de componentes complexa e reutilizável é extraída para Hooks customizados, mantendo os componentes limpos.
  - **Camada de Serviço (Service Layer):** A comunicação com o Supabase e outras APIs é abstraída em uma camada de serviço, desacoplando a UI da lógica de dados.
  - **Sistema de Design (Design System):** Utiliza um sistema padronizado de tokens (cores, fontes, espaçamentos) e componentes reutilizáveis (baseados em `shadcn/ui`) para consistência visual.
</details>

## 🤝 Contribuição

Este é um projeto privado desenvolvido sob encomenda para um cliente específico. Portanto, **contribuições externas não são aceitas**.

## 📄 Licença

Todos os direitos reservados. O código-fonte é proprietário e não pode ser copiado, modificado ou distribuído sem permissão explícita do autor.

---

<p align="center">
  Feito com ❤️ por <a href="https://github.com/FelipeCM804">Felipe Costa Morais</a>
</p>
