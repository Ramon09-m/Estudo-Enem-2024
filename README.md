
🎯 Objetivo
Este projeto tem como objetivo analisar os microdados do ENEM 2024, verificando se fatores socioeconômicos — como renda média dos participantes e a quantidade de escolas particulares em cada município de São Paulo — impactam no desempenho dos alunos nas provas (notas de redação e áreas de conhecimento).

📂 Fonte dos Dados
Os dados utilizados foram extraídos do portal oficial do INEP: https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/microdados/enem

A análise combina:

CSV de participantes (informações socioeconômicas e perfil dos inscritos)

CSV de resultados (notas por área e redação)

Dados complementares sobre escolas particulares por município de SP

🛠 Metodologia
Carregamento dos dados

Utilização do pandas para leitura dos arquivos CSV.

Tratamento de encoding (latin-1) e separador (sep=";").

Limpeza e preparação

Seleção de colunas relevantes: notas, município, tipo de escola, renda declarada.

Normalização de valores faltantes e categóricos.

Agrupamento por município (SP)

Cálculo da média das notas por município.

Contagem de escolas particulares em cada município.

Cruzamento com renda média dos participantes.

Análise estatística

Correlação entre renda média e notas.

Correlação entre quantidade de escolas particulares e notas.

Comparação entre municípios com maior e menor presença de escolas privadas.

Visualizações
<img width="885" height="790" alt="image" src="https://github.com/user-attachments/assets/c07e46c8-bc62-4cf6-b7ae-24411ae4d391" />


Gráficos de dispersão (renda × nota).

Mapas ou heatmaps por município.

Boxplots comparando desempenho em municípios com diferentes perfis de escolaridade.

📊 Resultados
Municípios com maior concentração de escolas particulares apresentaram notas médias mais altas em todas as áreas avaliadas.

A renda média dos participantes também se mostrou correlacionada com o desempenho.

A análise confirma que a quantidade de escolas particulares em cada município de SP está associada ao desempenho dos alunos no ENEM 2024, reforçando que desigualdades socioeconômicas se traduzem em desigualdades educacionais.

🚀 Como Executar
Baixe os microdados do ENEM 2024 no site do INEP.

Extraia os arquivos CSV de participantes e resultados.

Coloque-os na pasta do projeto.

Execute o notebook com:

bash
jupyter notebook analise_enem_2024.ipynb
Certifique-se de ter instalados:

bash
pip install pandas numpy matplotlib seaborn
📌 Observações
Os resultados apresentados refletem apenas os dados disponíveis nos microdados do INEP.

A análise identifica associações estatísticas, não necessariamente causalidade.

Diferenças regionais dentro de SP podem ser exploradas em maior profundidade com dados adicionais.
