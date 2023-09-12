# Projeto: Financial Fraud Detection
Por David Panduro 💻<br><br>
![image](https://github.com/DavidPanduro/financial_fraud_detection/assets/45201867/0205615e-7e3b-450d-a941-0c2b50afa1f8)<br>

Desenvolvemos um Modelo para detecção de fraude financeiro de boletos bancários, para um Agente Financeiro muito relevante dentro do Sistema Financeiro Brasileiro.
A contrucção das variáveis será baseado no histórico transaccional dos clientes, nas características particulares do cliente - sem considerar dados sensíveis (cpf, rg, etc).
Os nomes das variáveis foram encapsulados para resguardar a privacidade dos dados.<br><br>

![image](https://github.com/DavidPanduro/financial_fraud_detection/assets/45201867/d731f9fb-fa6b-4a41-8e16-5e9093cdb05d)<br>
<p style="text-align: center;">Fig.01. Conjunto de Dados </p><br><br>
A nossa amostra para analise contou de 1.148 registros, e correpondendo a caracteristica do problema apresenta classes totalmente desbalanceadas, situação que foi atendida mediante aplicação de SMOTE.<br><br>

![image](https://github.com/DavidPanduro/financial_fraud_detection/assets/45201867/7dfa6b0e-5b56-47ba-b0e5-e22f7aad045e)<br>
<p style="text-align: center;">Fig.02. Proporção das Classes </p><br><br>
A princípio analisamos o conjunto de dados com o intuito de achar as features que podem ter maior significancia para a melhor generalização do nosso modelo. <br>

Para isso passamos pela **Análise Univariada** para ver aspectos como distribuição, dispersão, medidas de resumo, com o objetivo de compreender as características de cada uma das variáveis individualmente.<br><br>

![image](https://github.com/DavidPanduro/financial_fraud_detection/assets/45201867/94925f82-7932-400f-9497-8e6f0a7979bf)<br>
<p style="text-align: center;">Fig.03. Distribuição da Classe Alvo (Fraude / Não Fraude) </p><br><br>

A continuação procedemos com a **Análise Bivariada**. Com isso, esperamos ver se cada uma das variáveis consegue ser significativa para discriminar uma classe da outra (fraude/não fraude).<br><br>
![image](https://github.com/DavidPanduro/financial_fraud_detection/assets/45201867/62da7abe-bd8f-4178-8d54-d9c444cd7ced)<br>
<p style="text-align: center;">Fig.04. Análise Bivariada (Fraude / Não Fraude) </p><br><br>
Além disso, temos a **Análise Multivariada** apresentando um quadro de Correlações incluindo o método Pearson.<br><br>

> [!IMPORTANT]
> As correlações são importantes para tentar evitar a Multicolinearidade <br><br>

![image](https://github.com/DavidPanduro/financial_fraud_detection/assets/45201867/8d1a033f-6098-4834-8d80-0198670e4429)<br>
<p style="text-align: center;">Fig.05. Correlações </p><br><br> 

Entre Análise Univariada e Análises Bivariada já conseguimos um _feeling_ de quais features consideraremos para aplicar a modelagem. Já com a Multivariada consideramos retirar alguma variável ou combinar com outra variável para evitar Multicolinearidade. <br>
Depois do _feeling_ precisamos aplicar métodos sofisticados como WOE (Peso das Evidencias), para saber quais variáveis, mediante tentativa de binarização, carregam um valor de informação significativo.<br> Também aplicamos o Método Boruta que cria variáveis sombras, aplica random forest e finaliza ccom uma distribuição binária para seleção das melhores features. <br> Random FOrest Best Selection é mais um método que implementamos na nossa análise. E finalmente, aplicamos Recursive Feature Elimination (RFE).<br>
![image](https://github.com/DavidPanduro/financial_fraud_detection/assets/45201867/2b8d5492-14c6-4e46-a0e4-bb834fd3d6eb)<br>
<p style="text-align: center;">Fig.06. Random Feature Best Selection </p><br><br> 








