# Banco de Dados - Datasets

Neste seção serão utilizados os datasets utilizados na disciplina de banco de dados.

## Estou utilizando o Google Colab

Se você está seguindo a dica dos instrutores e utilizando o Google Colab para escrever seus notebooks, você pode baixar uma cópia dos dados no próprio Google Colab. Para isto, você precisa apenas adicionar o seguinte comando em uma célula de código do seu notebook:

```colab
!git lfs clone -l -s https://github.com/labeduc/datasets.git
```

| **Dica**                                                                                                                         |
| -------------------------------------------------------------------------------------------------------------------------------- |
| Ao organizar seu notebook, crie uma seção no início onde você inicializa o ambiente, incluindo realizar o download dos datasets. |

Este mesmo comando deve funcionar em outros ambientes similares ao Google Colab, como o Jupyter e Deepnote.

## Estou utilizando VSCode, PyCharm e outras IDEs

Isto significa que você está utilizando seu próprio computador para realizar o desenvolvimento dos seus notebooks. Por isso, a maneira mais simples é baixar o repositório em um local que você possa acessar facilmente a partir dos seus notebooks.

Escolha um diretório e utilize o seguinte comando a partir do seu prompt:

```bash
> git clone https://github.com/labeduc/datasets.git
```

## Dataset: clientes

Este é um dataset simples para mostrar os exemplos dos comandos SQL.
Segue estrutura de dados:

| **Coluna** | **Nome**                | **Valores Não-Nulo** | **Tipo de Dados** | **Descrição**                                    |
| ---------- | ----------------------- | -------------------- | ----------------- | ------------------------------------------------ |
| 0          | Codigo                  | 10                   | integer           | Código de cadastro do usuário                    |
| 1          | Nome                    | 10                   | string            | Nome do cliente                                  |
| 2          | Cidade                  | 10                   | string            | Cidade aonde o cliente reside                    |
| 3          | Estado                  | 10                   | string            | Estado aonde o cliente reside                    |
