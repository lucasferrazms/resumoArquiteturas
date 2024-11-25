# Projeto resumo de arquiteturas

# Data Warehouse:
- Introdução:
  - O ambiente corporativo moderno, especialmente em médias e grandes empresas, é caracterizado por um crescimento exponencial no volume de dados gerados diariamente. Esses dados, quando armazenados e gerenciados de forma estratégica, tornam-se um ativo crucial para a tomada de decisões assertivas e para o posicionamento competitivo no mercado. Nesse contexto, Data Warehouses (armazéns de dados) desempenham um papel central, ao consolidar informações provenientes de diversas fontes em um único repositório estruturado, facilitando a análise e a geração de insights. Combinando tecnologia de ponta com métodos avançados de processamento de informações, os Data Warehouses permitem a extração de dados relevantes para análises estratégicas. Essa abordagem é essencial em uma sociedade cada vez mais orientada pela informação, onde o tratamento adequado dos dados determina a eficiência operacional e a capacidade de inovação das organizações. Assim, o uso de tecnologias de armazéns de dados não só potencializa o aproveitamento desse manancial de informações, como também define os melhores caminhos a serem seguidos para alcançar o sucesso no ambiente de negócios cada vez mais dinâmico e competitivo.
 
- Arquitetura:
   - A arquitetura de um Data Warehouse (DW) é projetada para centralizar e organizar dados de forma que possam ser analisados de maneira eficiente. Ela é estruturada em camadas e envolve diversos componentes que trabalham em conjunto para garantir a coleta, transformação, armazenamento e acesso aos dados. A seguir, detalha-se cada camada: 
  - Camada de Origem de Dados (Fonte de Dados)
    Os dados são coletados de diferentes sistemas transacionais, como CRM, ERP, bases de dados relacionais, arquivos CSV, APIs, ou mesmo fontes externas como redes sociais.
    Estas fontes podem ser heterogêneas, possuindo diferentes formatos e padrões, exigindo transformação antes do armazenamento.
  - Camada de Extração, Transformação e Carga (ETL)
    * Extração: Os dados são retirados das fontes, frequentemente de maneira incremental ou em lote, para capturar atualizações ou novos registros.
    * Transformação: Os dados brutos são tratados e padronizados, como normalização de formatos de data, remoção de inconsistências, enriquecimento de dados e aplicação de regras de negócio.
    * Carga: Os dados tratados são carregados para o Data Warehouse em uma estrutura otimizada para consultas analíticas.
  - Camada de Armazenamento de Dados
   * Os dados consolidados são armazenados em um banco de dados centralizado.
   * Normalmente utiliza-se uma modelagem dimensional (esquema estrela ou floco de neve), otimizando a consulta e análise.
   * A arquitetura permite particionamento, indexação e compactação para lidar com grandes volumes de dados.
  - Camada de Acesso aos Dados (Data Access Layer)
   * Ferramentas de Business Intelligence (BI) acessam o Data Warehouse para fornecer dashboards, relatórios ou análises detalhadas.
   * Essa camada utiliza linguagens como SQL ou ferramentas como Tableau, Power BI e Qlik para tornar os dados acessíveis e compreensíveis para tomadores de decisão.
  - Camada de Gestão e Administração
   * Inclui sistemas de monitoramento e controle, garantindo o desempenho e a segurança dos dados armazenados.
   * Gerencia aspectos como escalabilidade, alta disponibilidade e backups regulares.
