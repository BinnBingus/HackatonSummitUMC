# Hackathon de Ciência de Dados: O Desafio de 1936
**Apresentação para o Summit UMC - Universidade de Mogi das Cruzes**

O maior desastre preditivo da história estatística ocorreu nas eleições presidenciais dos Estados Unidos de 1936. A renomada revista *The Literary Digest* recolheu quase 2,4 milhões de respostas à sua pesquisa de intenção de voto e previu uma vitória esmagadora do candidato republicano Alf Landon. No entanto, nas urnas, Franklin D. Roosevelt venceu com 62% dos votos. Este projeto atua como uma investigação de ciência de dados forense para diagnosticar as causas metodológicas desse erro e aplicar modelos preditivos na tentativa de corrigir o viés histórico.

## Metodologia e Trilha de Dados
O desenvolvimento ocorreu em ambiente Jupyter Notebook (Python), estruturado em quatro etapas progressivas de análise:
* **Data Wrangling:** Limpeza de dados em larga escala, padronização dinâmica de cabeçalhos e conversão de formatos de texto para numéricos, utilizando Pandas com funções imunes a falhas de execução.
* **Estatística Descritiva:** Extração e cruzamento de proporções reais versus previstas nas pesquisas, isolando o viés estadual.
* **Diagnóstico de Viés:** Construção de visualizações analíticas de dispersão e densidade (Seaborn e Matplotlib) para comprovar graficamente a distorção da amostra em relação à realidade.
* **Modelagem Preditiva e Correção Ancorada:** Aplicação de Regressão Linear (Scikit-Learn) treinada com os dados eleitorais de 1932 e elaboração de um modelo secundário ancorado por estado, testando se correlações históricas poderiam salvar uma amostragem atual comprometida.

## Resultados Estatísticos e a Prova do Colapso
A aplicação do modelo ancorado resultou em um **R² negativo (-4.65)**. Longe de indicar um erro de código, essa métrica atesta matematicamente a falência metodológica da revista. A amostragem original baseou-se em listas telefônicas e registros automotivos, selecionando exclusivamente a elite econômica americana. Com a polarização causada pela Grande Depressão, a estrutura social do voto quebrou. A regressão prova que, quando os dados originais sofrem de viés de seleção extremo, a aplicação de modelos matemáticos baseados no passado não corrige o problema, apenas amplifica o ruído e agrava o erro.

## Conexão com os Desafios Éticos da IA Moderna
O caso de 1936 ilustra o princípio fundamental de *Garbage In, Garbage Out* (Lixo que entra, lixo que sai). A lição central para a engenharia de dados atual é que a volumetria ("Big Data") não substitui a representatividade. Modelos modernos de Inteligência Artificial e Machine Learning são cegos à realidade social se forem treinados em bases não auditadas. Alimentar redes neurais com dados excludentes — seja por classe, gênero ou raça — não gera inteligência, mas sim a automação e o agravamento de preconceitos históricos em grande escala.

---
**Tecnologias Utilizadas:** `Python`, `Pandas`, `NumPy`, `Scikit-Learn`, `Matplotlib`, `Seaborn`.  
**Laboratório: UMC**
