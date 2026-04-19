# Lab-08---AI-topics

O Papel do Hiperparâmetro $\beta$ na Otimização de Preferências


Na Otimização de Preferências (como no DPO - Direct Preference Optimization), o parâmetro $\beta$ desempenha o papel crítico de coeficiente de regularização, controlando a força da divergência KL (Kullback-Leibler) entre a política do modelo atual ($\pi_{\theta}$) e o modelo de referência original ($\pi_{ref}$). Matematicamente, o $\beta$ atua como um "imposto sobre a divergência": ele dita o custo de se afastar da distribuição de probabilidade original.Quanto menor o valor de $\beta$, mais liberdade o modelo tem para maximizar a recompensa das preferências, o que pode levar ao reward hacking e à degradação da fluência. Por outro lado, um $\beta$ bem ajustado garante que o modelo aprenda os novos comportamentos desejados sem "destruir" a estrutura linguística e o conhecimento prévio do modelo base. Em suma, o $\beta$ é o mecanismo de controle que impede que a otimização transforme o modelo em um gerador de texto repetitivo ou sem nexo, mantendo-o ancorado na fluência natural da linguagem humana.
