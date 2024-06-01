# LabEduc - Datasets

Olá, Cientista de Dados!!!

Aqui neste repositório, você encontrará todos os conjuntos de dados (datasets) que são utilizados nas aulas da trilha de ciências de dados do LabEduc e mais alguns outros repositórios para vocês praticarem!

Todos os datasets são públicos e foram obtidos em diversos sites. O arquivo readme.md em cada folder tem mais detalhes. Se você for utilizar estes arquivos em outras atividades, não esqueça de referenciar a origem do dataset.

Os datasets que não estão em um folder específico são datasets que estão em análise, portanto ainda não temos a descrição de cada um.

Abaixo seguem algumas orientações de como utilizar estes datasets.

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
> git clone https://github.com/labeduc/datasets.git && rm -rf datasets/.git
```

**AVISO**: esse comando funciona em sistemas operacionais linux e mac. Se você está usando Windows, o comando se divide em dois:

```cmd
> git clone https://github.com/labeduc/datasets.git 
> del datasets/.git
```


### Dependências

Para baixar os datasets no seu computador, você precisa ter o cliente do Git instalado em seu computador. Você pode obte-lo [aqui](https://git-scm.com/download).


## E se eu não quiser baixar os arquivos, como faço???

Se você não quiser baixar os arquivos, para poupar seus recursos de armazenamento, ainda existe uma alternativa: você pode acessar os arquivos de forma online através de uma URL especial do GitHub!

### URL

```
https://github.com/labeduc/datasets/blob/main/<diretorio>/<nome do arquivo>?raw=true
```

onde:
- `<diretorio>` - pasta de onde queremos ler o arquivo. Exemplo: pokemons é a pasta que contém o dataset de pokemons.
- `<nome do arquivo>` - nome do arquivo de dados. Exemplo: na pasta pokemons temos o arquivo all.csv.

Então, mostrando o exemplo completo:
Se quisermos carregar os dados de pokemons em um DataFrame do Pandas, o código seria esse:

```python
import pandas as pd

pokemons = pd.read_csv('https://github.com/labeduc/datasets/blob/main/pokemons/all.csv?raw=true')

print(pokemons.shape)
(1032, 44)
```

## Atualizações

Conforme for necessário, iremos atualizar os datasets existentes e também adicionar novos datasets, que estarão associados aos nossos exercícios, desafios e aulas!
