# Curso Data Analytics com KNIME (Dez2023)

> Status do Projeto: ⚠️ (em desenvolvimento)

## Análise de Dados da ANVISA com a ferramenta KNIME

Este repositório contém o workflow que desenvolvi durante o curso "Data Analytics com KNIME (Dez2023)", utilizando a poderosa ferramenta KNIME. O projeto foca na análise de dados disponibilizados pela ANVISA, abordando aspectos da farmacovigilância no Brasil através de dados do sistema VigiMed.

### Fontes de Dados

Os dados utilizados neste projeto foram extraídos do portal da [ANVISA](https://dados.anvisa.gov.br/dados/) e também constam no repositório "datasets":

- `VigiMed_Medicamentos-29-12-2023.csv`: Contém informações detalhadas sobre medicamentos, incluindo nome, fabricante, etc.
- `VigiMed_Notificacoes-29-12-2023.csv`: Registra notificações de eventos adversos e outras ocorrências relacionadas a medicamentos.
- `VigiMed_Reacoes-29-12-2023.csv`: Lista reações adversas reportadas, proporcionando insights valiosos sobre a segurança dos medicamentos.
- `DADOS_ABERTOS_MEDICAMENTOS.csv`: Uma base abrangente sobre medicamentos disponíveis no mercado brasileiro.

### Objetivo do Projeto

O principal objetivo deste projeto é analisar padrões e tendências nas notificações de eventos adversos e reações relacionadas a medicamentos, utilizando técnicas aprendidas neste curso de Data Analytics.

### Metodologia

Para estruturar este projeto, adotei a metodologia CRISP-DM (Cross-Industry Standard Process for Data Mining), que inclui as seguintes fases:

1. **Entendimento do Negócio**: Identificação das necessidades e objetivos da ANVISA em relação à segurança dos medicamentos.
2. **Entendimento dos Dados**: Exploração inicial dos conjuntos de dados para compreender sua estrutura e conteúdo.
3. **Preparação dos Dados**: Limpeza e transformação dos dados para análise.
4. **Modelagem**: Aplicação de técnicas de Data Analytics para extrair insights.
5. **Avaliação**: Avaliação dos resultados obtidos em relação aos objetivos do projeto.
6. **Implantação**: Preparação do workflow para uso prático e compartilhamento dos resultados.

### Workflow no KNIME

O workflow desenvolvido no KNIME integra todas as etapas do CRISP-DM, desde a importação e limpeza dos dados até a análise e visualização dos resultados. As técnicas aplicadas incluem análise exploratória de dados, estatísticas descritivas e visualizações interativas. O workflow desenvolvido no KNIME é composto de várias etapas, conforme ilustrado na imagem abaixo:

#### Carga de Dados
Iniciei com a leitura dos arquivos CSV, onde cada arquivo corresponde a um nó específico (`CSV Reader`). Após a leitura, utilizei nós de `Data Explorer` e `Statistics View` para realizar uma análise exploratória inicial, seguida de um registro dos dados através de `Table Writer`.

#### Pré-Processamento / Transformação
Nesta fase, os dados passaram por uma limpeza e preparação para análise. Utilizei nós como `Missing Value` para tratar valores ausentes e `Column Filter` para selecionar atributos relevantes. O `Joiner` foi aplicado para combinar diferentes conjuntos de dados em uma estrutura unificada. Metanós foram utilizados para agrupar transformações lógicas e simplificar o fluxo.

#### Modelos / Interpretação dos Resultados
Metanós também foram empregados nesta fase para encapsular a lógica de modelagem e análise, permitindo uma interpretação mais clara dos resultados processados.

#### Dashboard / Relatórios
A visualização dos resultados é feita por meio de um `Dashboard`, onde os insights podem ser explorados interativamente.

#### Modelos / Bases Finais
Por fim, os resultados processados são escritos em um arquivo final através do nó `Table Writer`, garantindo que o conhecimento gerado seja preservado para uso futuro.

## Conclusão

Este projeto não só reforçou meus conhecimentos em análise de dados mas também me proporcionou experiência prática com dados reais, preparando-me para enfrentar desafios analíticos no mundo real. Também proporcionou insights valiosos sobre a segurança dos medicamentos no Brasil, destacando a importância da análise de dados na farmacovigilância. Através deste trabalho, foi possível identificar padrões e tendências significativas que podem auxiliar na tomada de decisões e na formulação de políticas de saúde pública.

## Desenvolvedores/Contribuintes

| [![](https://media.licdn.com/dms/image/C4D03AQHFMOoH-OYCdA/profile-displayphoto-shrink_200_200/0/1576324910132?e=1709769600&v=beta&t=Wzn9PmIhgA52HRB0o3n5micuTe1bW7zofYoHT1bcI9U)  <br><sub>Perciliano</sub>](https://github.com/LuizPerciliano) | [![](https://media.licdn.com/dms/image/C4D03AQHUeLIPSa9c1Q/profile-displayphoto-shrink_800_800/0/1644213245938?e=1709769600&v=beta&t=lY-h-Eh-MuXo9cm0iZZ5AzlfbxRsG4r-SHB2rj8zCgc)  <br><sub>Lisandro Abulatif</sub>](https://www.linkedin.com/in/lisandro-abulatif/)
| :---: | :---: | 

## Licença

The MIT License (MIT)

Copyright ©️ 2023