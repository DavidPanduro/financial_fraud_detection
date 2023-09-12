# Projeto: Financial Fraud Detection
Por David Panduro 💻<br><br>
![image](https://github.com/DavidPanduro/fraud_detection/assets/45201867/24c73bbf-9513-4e16-999b-de45021ee4b3)<br><br>
Desenvolvemos um Modelo para detecção de fraude financeiro de boletos bancários, para um Agente Financeiro muito relevante dentro do Sistema Financeiro Brasileiro.
A contrucção das variáveis será baseado no histórico transaccional dos clientes, nas características particulares do cliente - sem considerar dados sensíveis (cpf, rg, etc).
Os nomes das variáveis foram encapsulados para resguardar a privacidade dos dados.<br><br>

![image](https://github.com/DavidPanduro/financial_fraud_detection/assets/45201867/d731f9fb-fa6b-4a41-8e16-5e9093cdb05d)<br>
<p style="text-align: center;">Fig.01. Conjunto de Dados </p><br><br>
A nossa amostra para analise contou de 1.148 registros, e correpondendo a caracteristica do problema apresenta classes totalmente desbalanceadas, situação que foi atendida mediante aplicação de SMOTE.<br><br>

![image](https://github.com/DavidPanduro/financial_fraud_detection/assets/45201867/7dfa6b0e-5b56-47ba-b0e5-e22f7aad045e)<br>
<p style="text-align: center;">Fig.02. Proporção das Classes </p><br><br>
A princípio analisamos o conjunto de dados com o intuito de achar as features que podem ter maior significancia para a melhor generalização do nosso modelo. <br>
Para isso passamos pela **Analise Univariada**, para ver aspectos como distribuição, dispersão, medidas de resumo, com o objetivo de compreender as características de cada uma das variáveis individualmente.<br><br>

![image](https://github.com/DavidPanduro/financial_fraud_detection/assets/45201867/94925f82-7932-400f-9497-8e6f0a7979bf)<br>
<p style="text-align: center;">Fig.03. Distribuição da Classe Alvo (Fraude / Não Fraude) </p><br><br>






