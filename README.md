# TCC_PUC_MINAS

<div stile="display: inline_block"><br/>
  <img align="center" alt="html5" src="https://img.shields.io/badge/Power%20BI-F2C811.svg?style=for-the-badge&logo=Power-BI&logoColor=black" >
  <img align="center" alt="html5" src="https://img.shields.io/badge/Knime-E0E5EC.svg?style=for-the-badge&logo=Knime&logoColor=#FDD800" >
  <img align="center" alt="html5" src="https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927.svg?style=for-the-badge&logo=Microsoft-SQL-Server&logoColor=white" />
</div>


Pasta destinada ao trabalho de conclusão de curso de pós graduação em **Gestão e Análise Estratégica de Dados** da Puc Minas.

Para este projeto foram utilizados as feramentas: *Knime Analytics*, *SQL Server* e *Power BI*

[Dashboard](https://app.powerbi.com/view?r=eyJrIjoiMDFlYzgzMTgtMTI2Mi00OTE0LThhYTYtZTc3YmU4OTBhMzg1IiwidCI6IjE0Y2JkNWE3LWVjOTQtNDZiYS1iMzE0LWNjMGZjOTcyYTE2MSIsImMiOjh9&embedImagePlaceholder=true&pageName=ReportSection)

<br>
<div align="left">
<img src="https://github.com/MendesRamon/TCC_PUC_MINAS/assets/141190770/08d0141e-2e95-4c16-887f-9b9ffeae5ce5" width="800px" />
<div/>


[Vídeo Apresentação](https://youtu.be/ZXHgTNob0AM?si=3hDRXE7hucAofXxt)

### Objetivo

Este trabalho tem como objetivo expor municípios onde ocorre acidentes de trânsito com maior frequência no estado de São Paulo, em quais sazonalidades e situações climáticas a fim de se criar estratégias que evitem ocorrências de acidentes fatais e não fatais. Para isso, será criada, um dashboard com níveis estratégico, tático e operacional, a fim de ter uma visão geral das ocorrências, análise climática ambiental e temporal. Tudo isso deve ocorrer de forma automatizada.

### Desenvolvimento

Foi utilizado a ferramenta _Knime Analitycs_ para criar o pipeline da extração dos arquivos na página _web_, onde está disponibilizado, e efetuado o input no banco de dados. Segue os seguintes passos:

- Acessa a página web e baixa os arquivos na pasta downloads;
- Faz normalização dos dados, criando uma tabela para as localidades dos acidentes;
- Acessa o banco de dados e caso não exista a tabela ele cria, e se existir, ele faz o comando de _drop table_ e cria a tabela.

![knime](https://github.com/MendesRamon/SQL/assets/141190770/e732b9a1-af42-4b3c-b601-34920a301b30)


**Modelo físico do banco de dados criado pelo pipeline de dados**


![SQL](https://github.com/MendesRamon/SQL/assets/141190770/1203a714-7f4a-4a48-8ae9-9c03ea8748b7)


**Modelo de dados _Snow Flake_ no Power BI**

![PowerBI](https://github.com/MendesRamon/SQL/assets/141190770/02601484-c197-401e-a7d9-85664a6a2457)


### Conclusão

Ao analisarmos ao longo dos 5 anos é possível ver que houve um aumento de 5,56% de acidentes de trânsito no estado de São Paulo. Em comparação nos anos de 2019 e 2020 observa-se uma diminuição de ocorrências em 9,37% no qual pode-se atribuir as restrições de circulação devido a pandemia, quando comparado ao ano de 2022 contra 2023 houve um aumento de 8,43%, quando começou a normalizar a circulação. OMS classifica coronavírus como pandemia. Gov.br, 11/03/2020. Disponível em: <https://www.gov.br/pt-br/noticias/saude-e-vigilancia-sanitaria/2020/03/oms-classifica-coronavirus-como-pandemia>.

Quanto as condições climáticas, no ano de 2023 é possível identificar que 54,4% dos casos ocorreram em condições climáticas documentadas como bom e cerca de 39,3% a luz do dia que ocorre com maior frequência entre sexta-feira e sábados. Nestes dados, podemos concluir que entre outros motivos, o excesso de confiança pode ter causado os acidentes.
Em feriados, o Carnaval atrai a atenção com um total no ano de 2022 de 807 casos, seguido pelo Natal com 618 casos registrados.  Entre 2019 à 2023 o feriado de Carnaval se posiciona em primeiro no ranking de acidentes de trânsito.

Quando olhamos para o tipo de via, as vias municipais ocorreram o maior índice de acidentes, sendo de 78,1% no ano de 2021, enquanto rodovias sendo de 17,7% e não informados de 4,2%. Acredita-se que devido a ter um grande fluxo de pessoas em vias municipais à maior incidência de casos. Porém, com 2,7% ocorrendo vitimas fatais enquanto em rodovias 9,6%, por ter um limite de velocidade maior do que em vias municipais.

A proposta para este projeto é de conscientização para a população e acesso aos dados de acidentes de trânsito no estado de São Paulo de forma resumida e clara. A fim de que seja possível traçar estratégias de prevenção à acidentes, em pontos específicos e em determinada sazonalidade de forma em que os recursos humanos, materiais e financeiros, do estado ou da iniciativa privada, sejam aplicados com maior eficiência e eficácia no objetivo final de prevenir acidentes e salvar vidas. 

***Limitações***

Durante o processo de desenvolvimento do projeto foi observado algumas limitações, como: acesso à informação, embora esteja em um site, a informação tratada no trabalho deve ser de interesse público, ou seja, são dados que devem ser divulgados e ter forma mais acessível a fim de conscientizar a população. Outro ponto no qual é possível se trabalhar são os dados categóricos do tipo idade, sexo, renda no intuito de se traçar um perfil que seja mais recorrente, porém, não está documentado nos arquivos.
