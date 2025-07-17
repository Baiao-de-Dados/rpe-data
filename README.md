# RPE Data Repository

Este repositório contém os dados e notebooks utilizados para o processamento, limpeza e análise de avaliações no sistema RPE. Ele é organizado em diferentes pastas para facilitar o acesso e a manipulação dos dados.

---

## Estrutura do Repositório

### **1. Arquivos Principais**
- **`Primary-usuarios.xlsx`**: Contém a lista dos principais usuários do sistema.
- **`evaluations-to-import`**: Esta pasta contém as avaliações antigas dos usuários prontas para serem importadas no RPE.

---

### **2. Diretórios**

#### **`evaluations-to-import/`**
Contém os arquivos de avaliações dos usuários organizados por ciclo:
- `2024.1.xlsx`
- `2024.2.xlsx`
- `2025.1.xlsx`

#### **`notebooks/`**
Contém notebooks Jupyter para manipulação e análise de dados:
- **`cleaning.ipynb`**: Notebook para limpeza e padronização dos dados.
- **`merge.ipynb`**: Notebook para mesclar dados de avaliações dos usuários de cada ciclo.
- **`spaces.ipynb`**: Notebook para ajustes de formatação e remoção de inconsistências.
- **`Users.ipynb`**: Notebook para manipulação e geração de listas com os principais usuários.

#### **`OLD Data and Notebooks ---DEPRECATED/`**
Arquivos e notebooks antigos que não são mais utilizados:
- **`employee.ipynb`**
- **`users.csv`**

#### **`unclened-data/`**
Dados brutos que foram utilizados:
- **`compilado-evaluations/`**: Contém arquivos de avaliações individuais, como:
  - `ANA_DA_2024_2.xlsx`
  - `BRYAN_DIAS_2024_1.XLSX`
  - `DR__JOAQUIM_2025_1.XLSX`
- **`De-para de Critérios.xlsx`**: Mapeamento de critérios antigos para padronização dos novos critérios.

---

## Fluxo de Trabalho

1. **Mesclagem de Dados**:
   - Use o notebook `merge.ipynb` para combinar todos os dados de diferentes usuários em um único arquivo, dividindo os arquivos por ciclos.

2. **Limpeza de Dados**:
   - Utilize o notebook `cleaning.ipynb` para padronizar colunas como `Email` e `Name`.
   - Adicione sufixos ausentes, como `.com`, e remova inconsistências.
   - Remova tabelas desnecessárias e padronize os emails.
   - Corrija incoerências nos dados para garantir a consistência.

3. **Geração de Usuários**:
   - O notebook `Users.ipynb` é usado para extrair os principais usuários e gerar senhas e seus emails.

4. **Exportação Final**:
   - Após o processamento, os dados limpos e mesclados são exportados para arquivos finais prontos para análise ou importação no sistema.

---

## Observações

- **Consistência de Dados**: Certifique-se de que os arquivos no diretório `unclened-data/` sejam processados antes de serem utilizados. Se for utilizar os dados para importação, use a pasta `evaluations-to-import/`.
- **Depreciação**: Evite usar arquivos e notebooks no diretório `OLD Data and Notebooks ---DEPRECATED/`.
- **Automação**: Alguns processos ainda são feitos manualmente.

---

## Contato

Para dúvidas ou sugestões, entre em contato com os administradores do repositório.