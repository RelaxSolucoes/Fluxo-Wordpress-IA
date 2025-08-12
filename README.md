# Fluxo WordPress IA – n8n + Evolution API + OpenAI

Este repositório contém um fluxo do **n8n** que integra **WordPress**, **API Evolution** e **OpenAI** para criar um assistente virtual capaz de responder automaticamente via **WhatsApp**, **chat widget** ou **formulário web**.

---

## 🚀 Funcionalidades
- Detecta automaticamente a origem da mensagem (**WhatsApp direto**, **formulário**, **chat widget**).
- Aplica regras de atendimento personalizáveis.
- Usa **IA (OpenAI)** para gerar respostas claras e contextuais.
- Mantém memória de conversas recentes.
- Envia mensagens automáticas ou manuais conforme o canal.

---

## 📋 Pré-requisitos
Antes de importar e usar o fluxo, você precisará ter:
- Uma instância funcional do **n8n**.
- Credenciais de **OpenAI** (API Key).
- **API Evolution** configurada com URL, API Key e nome da instância.
- Acesso ao **WordPress** e/ou canal de entrada de mensagens (**WhatsApp**, **formulário**, **chat widget**).

---

## 📥 Como importar o fluxo no n8n

1. **Baixe o arquivo do fluxo**
   - Baixe o arquivo `Fluxo Wordpress IA.json` deste repositório.

2. **Acesse seu n8n**
   - Abra o painel do **n8n** no seu navegador.

3. **Importe o fluxo**
   - Clique em **Menu → Import**.  
   - Selecione o arquivo `Fluxo Wordpress IA.json`.  
   - Confirme a importação.

4. **Configure as credenciais**
   - Abra o nó **OpenAI Chat Model** e insira sua **API Key da OpenAI**.
   - Copie a **URL** do primeiro nó (**When chat message received**) e cole no plugin **[wp-whatsevolution](https://github.com/RelaxSolucoes/wp-whatsevolution)**.

---

## ⚙️ Personalização
- No nó **AI Agent**, edite a mensagem do **System Message** para personalizar o tom e as regras de atendimento.

---

## ▶️ Executando
- Após salvar e ativar o fluxo, o **n8n** ficará escutando novas mensagens e processará automaticamente conforme a origem.

---

## 🛠 Suporte
Se encontrar problemas:
- Verifique se suas credenciais estão corretas.
- Confirme que sua instância da **API Evolution** está ativa.
- Cheque os logs do **n8n** para mensagens de erro.

---
