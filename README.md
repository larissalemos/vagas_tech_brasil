# Análise de Oferta vs. Demanda de Profissionais de Tecnologia no Brasil

## Visão Geral  
Este projeto teve como objetivo analisar a oferta e demanda por profissionais de tecnologia no Brasil a partir das vagas publicadas no LinkedIn e respectivas candidaturas. A análise considerou aspectos como localização, nível de senioridade, habilidades técnicas mais demandadas, formato de trabalho (presencial, híbrido ou remoto) e categorias profissionais.

Os resultados desta análise foram utilizados para embasar decisões estratégicas da **{reprograma}**, especialmente na definição do portfólio de cursos oferecidos. O foco foi identificar cargos com alta demanda e baixa oferta de profissionais, bem como mapear as habilidades técnicas mais requisitadas para cada posição.

Além da análise de vagas, este estudo fez parte de uma investigação de mercado mais ampla, que incluiu:

- Comparação do portfólio de cursos de organizações similares.  
- Criação de um banco de relatórios externos sobre tendências do mercado de tecnologia no Brasil e no mundo e análise dos mesmos.  
- Trocas com líderes do setor, incluindo representantes da **FIAP, GetOnBoard, Lumini e GOYN Colômbia**, que contribuíram para o planejamento e desenvolvimento da pesquisa.  

---

## Estrutura do Projeto  
O projeto contemplou as seguintes etapas:

### 1. Entendimento do Negócio  
- Contextualização sobre o mercado de trabalho de tecnologia no Brasil para construção de estratégias de desenvolvimento de profissionais demandados.

### 2. Coleta de Dados  
A coleta de dados foi realizada entre **janeiro e março de 2024**, utilizando **Octoparse** para extrair informações de vagas de emprego na área de tecnologia publicadas no LinkedIn.  

### 3. Preparação dos Dados  
Os dados extraídos foram processados e tratados utilizando **Python** no ambiente **Jupyter Notebook**, com o suporte das bibliotecas **pandas** e **numpy** para limpeza e organização das informações.  

- A classificação de **senioridade, modelo de trabalho e habilidades técnicas** foi feita a partir da descrição da vaga, com base em palavras-chave pré-definidas.  
- Vagas classificadas na categoria **"Outros"** não apresentavam nenhuma das palavras-chave utilizadas para agrupamento.  
- As vagas foram **categorizadas e subcategorizadas** com base em termos encontrados nos títulos dos anúncios.  
- O número de candidaturas consideradas variou entre **25 e 200 por vaga**.  

### 4. Análise Exploratória  
- Visualização de dados utilizando **Plotly e Tableau**.  
- Análise da distribuição de vagas por categoria, senioridade e tipo de trabalho (remoto, híbrido ou presencial).  

### 5. Visualização e Insights  
- Identificação de áreas com maior e menor demanda.  
- Comparação entre número de vagas abertas e quantidade de candidatos aplicando para cada tipo de cargo.  
- Mapeamento das principais ferramentas exigidas para cada posição.
- Distribuição geográfica das vagas

---

## Tecnologias Utilizadas  
- **Web Scraping:** Octoparse  
- **Manipulação de Dados:** Python (Jupyter Notebook, Pandas, NumPy)  
- **Visualização de Dados:** Tableau e Plotly

---

## Resultados Principais  
- Identificação de **desbalanceamento entre oferta e demanda** para diferentes perfis profissionais.  
- Mapeamento das **tecnologias mais requisitadas** para cada tipo de vaga.  
- Comparação entre **modelos de trabalho** (remoto, híbrido, presencial). 
- Distribuição **geográfica** das vagas
- Insights estratégicos para otimizar o **portfólio de cursos** na **{reprograma}**.  

---

## Próximos Passos 
- Agregar informações mais atualizadas de vagas. 
- Desenvolver modelos preditivos para antecipar tendências no mercado de tecnologia. 

---

## Observações
O arquivo de vagas disponibilizado neste repositório não contém toda a base original analisada devido à limitação de tamanho de arquivo permitido no github. Caso queira explorar a base completa, favor entrar em contato.

---
## Visualizações no Tableau

![tools](images/tools.jpg)  
*Figura 1: Exemplo de principais ferramentas demandadas para profissionais de ciência de dados considerando todos os níveis de senioridade.*  

![OfertaXDemanda](images/location.jpg)  
*Figura 2: Análise dos Estados com maior demanda de profissionais de tecnologia e empresas com maiores números de vagas no período.*  

## Visualizações no Jupyter
Ao rodar o notebook com o csv origingal (entre em contato para acesso), é possível visualizar:
- Distribuição de vagas por categoria
- Distribuição de vagas por senioridade
- Distribuição de vagas por modelo de trabalho
- Distribuição de vagas por categoria e senioridade
- Distribuição de vagas por senioridade e categoria
- Distribuição de candidaturas por vaga por categoria e senioridade
- 10 habilidade mais demandadas no geral
- 5 habilidades mais demandadas por categoria
- Sankey de distribuição de senioridade por categoria
- Mapas coropléticos de distribuição de vagas e de candidaturas por vaga por Estado.

## Conclusões e análises descritivas:

- **Categorias consideradas na análise:**  
- Desenvolvimento
  - ANÁLISE DE SISTEMAS
  - DADOS/BI
  - DESIGN/UX/UI
  - ANÁLISE DE NEGÓCIOS
  - LIDERANÇA
  - CLOUD/DEVOPS/INFRA
  - SEGURANÇA DA INFORMAÇÃO
  - QUALIDADE/TESTES

- **Níveis de senioridade considerados na análise:**
  - ESTÁGIO
  - JÚNIOR
  - PELNO-SÊNIOR
  - NÃO INFORMADO

- **Análise de vagas e candidaturas por categorias:**
  - A categoria com maior número de vagas disponíveis foi DESENVOLVIMENTO, representando 47% do total de 6389 vagas analisadas. 
  - As categorias DESENVOLVIMENTO (3023), ANÁLISE DE SISTEMAS (1549), DADOS/BI (734), DESIGN/UX/UI (620), juntas representam 92% do total de vagas.
  - A categoria QUALIDADE/TESTES e SEGURANÇA DA INFORMAÇÃO apresentaram o menor número de vagas, sendo 61 e 77, respectivamnte.
  - As três categorias com menor número de candidaturas por vaga são: CLOUD/DEVOPS/INFRA (26), DADOS/BI (32) e DESENVOLVIMENTO (32). As três categorias com maior número de candidaturas por vaga são ANÁLISE DE NEGÓCIOS (45), LIDERANÇA (46) e SEGURANÇA DA INFORMAÇÃO. Estas informações se contrapõem a relatórios de tendências que indicam lacunas de profissionais para cargos relacionados a segurança da informação e aumento do número de profissionais para cargos de desenvolvimento. Uma possível explicação para isso pode ser o gap do número de vagas de desenvolvimento vs segunraça da informação. 
  - Dentre todas as categorias, o número de candidaturas por vaga no nível JÚNIOR se destaca, com exceção das categorias LIDERANÇA, ANÁLISE DE SISTEMAS, DADOS/BI e CLOUD/DEVOPS/INFRA.
  - 
- **Análise de vagas e candidaturas por senioridade:**
  - Dentre os níveis de senioridade, 49% se referem ao nível ASSISTENTE, o que pode indicar falta de clareza sobre o nível de senioridade demandado nas vagas. 
  - 38% se referem ao nível PLENO-SÊNIOR. 
  - Apenas 2% são para o nível JÚNIOR. 
  - 6% das vagas não informaram nível de senioridade.
  - Apesar de representar apenas 2% das vagas, o nível JÚNIOR é o que apresenta a maior taxa de candidaturas por vaga (57). O nível ESTÁGIO apresenta 44 candidaturas por vaga, o PLENO-SÊNIOR apresenta 40 e o ASSISTENTE apresenta 29. Isso indica uma alta procura por vagas por profissionais em início de carreira.
  - 
- **Análise de vagas e candidaturas por modelo de trabalho:**
  - Dentre os modelos de trabalho, a maioria (60%) não foi informado, o que indica que a maioria das vagas não especifica o modelo de trabalho ou a categorização não capturou adequadamente os modelos remoto/híbrido/presencial.
  - 28% é REMOTO, 9% é HÍBRIDO e 8% é PRESENCIAL.
  - Dentre os modelos de trabalho, o PRESENCIAL apresentou a menor taxa de candidaturas por vaga (27), enquanto o HÍBRIDO e o REMOTO apresentaram 39 e 38 respectivamente. Isso é esperado, já que os modelos híbrido e remoto oferecem uma maior flexibilidade e alcance geográfico, além de favorecerem pessoas com deficiência e pessoas que conciliam trabalhos de cuidado familiar, em especial, mulheres.
  - 
- **Análise de vagas e candidaturas por categorias e senioridade:**
  - Dentre todas as categorias, os níveis PLENO-SÊNIOR e ASSISTENTE se destacam. Para a categoria de DESENVOLVIMENTO, a quantidade de vagas para ASSISTENTE corresponde a quase o dobro das vagas para PLENO-SÊNIOR. Já nas categorias ANÁLISE DE SISTEMAS e DADOS/BI, os níveis PLENO-SÊNIOR se destacam.
  - Dentre todos os níveis de senioridade, as categorias DESENVOLVIMENTO e ANÁLISE DE SISTEMAS se destacam.
  - Dentre as vagas para o nível JÚNIOR, esta distribuição dentre as categorias é mais uniforme do que nos níveis ASSISTENTE e PLENO-SÊNIOR.

- **Habilidades:**:
  - Considerando todas as categorias e níveis, as habilidades mais demandadas foram, em ordem: CLOUD, SQL, FRONT, BACK, UI, UX, PYTHON, AUTOMAÇÃO, INGLÊS e CONTINUOUS INTEGRATION (CI).
  - As 5 habilidades mais demandadas de cada categoria são:
  - DESENVOLVIMENTO: FRONT, BACK, CLOUD, REACT, SQL
  - ANÁLISE DE SISTEMAS: CLOUD, SQL, AUTOMAÇÃO, MACHINE LEARNING, PYTHON
  - DADOS/BI: CLOUD, SQL, MACHINE LEARNING, PYTHON, ETL
  - DESIGN/UX/UI: AGILE, UX, UI, PHOTSHOP, FIGMA
  - CLOUD/DEVOPS/INFRA: CLOUD, AUTOMAÇÃO, LINUX, AWS, CI
  - ANÁLISE DE NEGÓCIOS: CLOUD, SQL, INGLÊS, CRM, INTELIGÊNCIA ARTIFICIAL
  - LIDERANÇA: CLOUD, AGILE, INGLÊS, UX, SCRUM
  - QUALIDADE/TESTES: AUTOMAÇÃO, TESTE, QA, API, AGILE
  - SEGURANÇA DA INFORMAÇÃO: CLOUD, LINUX, AWS, SEGURANÇA DA INFORMAÇÃO, CI

- **Distribuição Geográfica:**
  - Mair de 47% das vagas são para o Estado de São Paulo. 
  - No geral, a região sudeste apresenta a maior quantidade de vagas.
  - Porém, a maior taxa de candidaturas por vaga é no Estado da Paraíba, porém, apenas 11 vagas foram divulgadas neste Estado. 
  - Os Estados da região Norte e Centro-Oeste apresentam a menor taxa de candidaturas por vaga. 


Contribuições e sugestões são sempre bem-vindas! 😊