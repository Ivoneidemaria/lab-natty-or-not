
# **Projeto: Gerador Automático de Roteiros de Viagem**

Este projeto utiliza ferramentas gratuitas e integrações via **Zapier** para criar roteiros de viagem personalizados de forma rápida e intuitiva. Os usuários preenchem um formulário simples, e o sistema gera automaticamente um roteiro detalhado em PDF, pronto para ser compartilhado.

---

## **Visão Geral do Projeto**

- **Objetivo**: Automatizar a criação de roteiros de viagem personalizados com o mínimo de esforço manual.
- **Ferramentas Utilizadas**:
  - **Google Forms**: Para coletar informações dos usuários.
  - **Google Sheets**: Para armazenar as respostas do formulário.
  - **ChatGPT (OpenAI)**: Para gerar o conteúdo do roteiro de viagem.
  - **Google Docs**: Para formatar o roteiro em um documento bonito.
  - **Zapier**: Para automatizar o fluxo entre as ferramentas.
  - **GoogleGmail** Para enviar os PDFs automaticamente aos usuários.

---

## **Fluxo de Trabalho**

1. **Entrada de Dados**:  
   O usuário preenche um formulário no **Google Forms** com informações básicas:
   - Destino da viagem.
   - Datas de início e fim.
   - Tipo de viagem (gastronomia, relaxamento, aventura, etc.).
   - Preferências ou comentários adicionais.

2. **Geração do Roteiro**:  
   O **Zapier** conecta o formulário ao **ChatGPT**, que usa os dados enviados para criar um roteiro personalizado, detalhado dia a dia.

3. **Formatação no Google Docs**:  
   O roteiro é inserido automaticamente em um modelo predefinido no **Google Docs**.
4. **Envio Automático (Opcional)**:  
   O PDF é enviado por e-mail ao usuário, caso um endereço tenha sido coletado.

---

## **Como Configurar o Projeto**

### **1. Crie o Formulário no Google Forms**
1. Acesse o [Google Forms](https://forms.google.com) e crie um formulário com as seguintes perguntas:
   - Destino da Viagem.
   - Datas de Início e Fim.
   - Tipo de Viagem.
   - Preferências Adicionais.
   - E-mail para envio do roteiro (opcional).
2. Conecte o formulário a uma planilha do **Google Sheets**.

### **2. Configure o Fluxo no Zapier**
1. Crie uma conta no [Zapier](https://zapier.com).
2. Configure o Zap com as seguintes etapas:
   - **Trigger**: Novo registro no Google Forms.
   - **Ação 1**: Enviar os dados para o ChatGPT (API do OpenAI).
   - **Ação 2**: Inserir o roteiro gerado em um modelo no Google Docs.
   - **Ação 3**: Exportar o documento como PDF.
   - **Ação 4 (opcional)**: Enviar o PDF para o e-mail do usuário.

### **3. Crie o Modelo no Google Docs**
1. Crie um documento no Google Docs com placeholders para os dados do roteiro, como:
   ```
   Roteiro de Viagem: {{Destino}}

   **Dia 1:**  
   - {{Atividade Dia 1}}

   **Dia 2:**  
   - {{Atividade Dia 2}}
   ```
2. Configure o Zapier para substituir os placeholders com os dados do ChatGPT.

---

## **Pré-requisitos**

- Conta no Google (para Forms, Sheets, Docs e Drive).
- Conta no Zapier (versão gratuita funciona para até 100 tarefas/mês).
- API Key do ChatGPT (OpenAI).

---

## **Personalização**

- **Estilo do Roteiro**: Você pode personalizar o texto e design do modelo no Google Docs para deixar o roteiro mais atrativo.
- **Integração com outras ferramentas**: Use WhatsApp, Slack ou outras plataformas para enviar os PDFs automaticamente.

---

## **Funcionalidades Futuras**
- Integração com APIs de viagem, como Google Places, para incluir mapas e sugestões automáticas de locais.
- Tradução automática do roteiro para outros idiomas.
- Recursos para incluir links de reservas de hotéis ou restaurantes.

---

## **Contribuições**

Sinta-se à vontade para sugerir melhorias ou abrir pull requests neste projeto.

