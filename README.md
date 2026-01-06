# 🚀 Estética IA: Personalização de Mensagens de Saúde e Bem-estar

Este projeto foi desenvolvido como parte do desafio da **Santander Dev Week 2025** promovido pela DIO. A solução original foi adaptada para o nicho de saúde e estética, utilizando Inteligência Artificial para gerar mensagens personalizadas para clientes.

## ⚠️ Adaptação Técnica Importante
Durante o desenvolvimento, identifiquei que a API oficial do Santander Dev Week estava inativa ou desabilitada. Para garantir a continuidade e entrega do projeto, realizei as seguintes modificações:
* **Banco de Dados Local:** Substituí as chamadas de API externa por um processamento de dados local via CSV.
* **Simulação de API:** Criei funções em Python que emulam o comportamento de métodos REST (como GET e PUT), garantindo que a lógica original de IDs e objetos fosse preservada.

## 📋 Descrição do Desafio
O objetivo principal foi criar um pipeline de **ETL (Extract, Transform, Load)** para processar dados de clientes e utilizar modelos de linguagem (IA) para enriquecer esses dados com conteúdos personalizados.

### Diferencial deste Projeto:
Este repositório foca em **procedimentos estéticos** (Botox, Limpeza de Pele, Preenchimento), transformando o cuidado com a beleza em um incentivo à saúde e ao bem-estar.

---

## ⚙️ O Fluxo ETL

### 1. **Extract (Extração)**
Os dados foram extraídos de um arquivo CSV personalizado (`saude_estetica.csv`). Implementei a função `get_user` para recuperar os dados de cada cliente individualmente, simulando o acesso a um banco de dados real.

### 2. **Transform (Transformação)**
Utilizei a API do **Google Gemini 2.5 Flash** para a geração das mensagens. 
* **Lógica:** A IA recebe o nome da cliente e o procedimento realizado.
* **Prompt:** A IA atua como uma especialista em estética, focando na conexão entre o procedimento e a saúde física e mental da cliente.

### 3. **Load (Carga)**
Os dados transformados foram salvos em um novo arquivo (`santander_dev_week_estetica_final.csv`). Este processo simulou o "Update" do CRUD, onde a informação gerada pela IA foi persistida para uso comercial.

---

## 🛠️ Tecnologias Utilizadas
* **Linguagem:** Python 🐍
* **Manipulação de Dados:** Pandas
* **Inteligência Artificial:** Google Generative AI (Gemini API)
* **Ambiente:** Google Colab ☁️

---

## 🛡️ Segurança de Dados
As chaves de API foram removidas do código antes do commit final. Recomenda-se o uso de **Secrets** do Google Colab para o gerenciamento seguro de credenciais em ambientes de desenvolvimento.

---

## 👨‍💻 Como Executar
1. Clone este repositório.
2. Certifique-se de ter os arquivos CSV no mesmo diretório.
3. Obtenha uma API Key no [Google AI Studio](https://aistudio.google.com).
4. Abra o notebook `Santander_Dev_Week_Estetica_IA.ipynb` no Google Colab e execute as células.

---
*Projeto realizado para fins educacionais no Bootcamp Santander Dev Week 2023.*

---
📫 **Contato:**
Tatiane Mares - www.linkedin.com/in/tatiane-mares-2061b8b6
