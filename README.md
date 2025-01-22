# Análise de Resultados com Madelyn API

Este repositório contém notebooks para pré-processamento, análise e visualização de dados gerados a partir da API **Madelyn**, utilizando um dataset legado do projeto **DoME**.

## Estrutura do Repositório

### Arquivos Principais

1. **`runtests.ipynb`**
   - Este notebook realiza o pré-processamento do dataset legado `dataset_dome.csv` e o utiliza para fazer chamadas à API **Madelyn**.
   - Após a execução, gera um arquivo `tests.csv` contendo os resultados obtidos da API.
   - Principais etapas do notebook:
     - Carregamento do dataset original.
     - Pré-processamento dos dados para adequação às especificações da API.
     - Envio dos dados à API **Madelyn** e obtenção de resultados.
     - Exportação dos resultados em formato CSV.

2. **`analyse_tests.ipynb`**
   - Realiza o pós-processamento do arquivo `tests.csv` gerado pelo notebook anterior.
   - Principais funcionalidades:
     - Análise dos acertos e identificação de discrepâncias.
     - Extração de informações relevantes a partir dos resultados.
     - Geração de gráficos para facilitar a interpretação dos dados.

3. **`dataset_dome.csv`**
   - Dataset legado do projeto **DoME**.
   - Utilizado como base para os testes realizados pela API **Madelyn**.

4. **`tests.csv`**
   - Arquivo gerado pelo notebook `runtests.ipynb`.
   - Contém os resultados das chamadas realizadas à API **Madelyn**.
   - Este arquivo é utilizado como entrada para o notebook `analyse_tests.ipynb`.

## Como Usar

1. Certifique-se de que todas as dependências necessárias estão instaladas.
2. Execute o notebook `runtests.ipynb` para gerar o arquivo `tests.csv`.
3. Em seguida, execute o notebook `analyse_tests.ipynb` para realizar a análise dos resultados.

## Requisitos

- Python 3.8 ou superior.
- Bibliotecas utilizadas:
  - Pandas
  - Matplotlib
  - Requests (para chamadas à API)

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir _issues_ ou enviar _pull requests_ com melhorias e novas funcionalidades.

## Licença

Este projeto é licenciado sob a [Licença MIT](LICENSE).
