# AlgaWorks - Atualização para Angular 10

1. Instalar o **@angular/cli 10** globalmente:

    ```
    npm i -g @angular/cli@10
    ```

1. Remover dependências incompatíveis e não utilizadas:

    ```
    npm rm ng2-toasty
    ```

1. Remover os códigos das dependências removidas:

    angular.json
    ```json
    "styles": [
      "node_modules/ng2-toasty/style-bootstrap.css",
      // ...
    ],
    ```

1. Executar os passos do [Angular Update Guide](https://update.angular.io/#9.1:10.0):

    ```
    ng update @angular/core @angular/cli
    git add .
    git commit ...
    ng update @angular/cdk
    ```

1. Atualizar o PrimeNG e o PrimeIcons:

    ```
    ng update primeng primeicons
    git add .
    git commit ...
    ```

1. Instalar a dependência PrimeFlex:

    ```
    npm install primeflex --save
    ```

1. Adicionar as folhas de estilo do PrimeNG:

    ```json
    "styles": [
      "node_modules/primeicons/primeicons.css",
      "node_modules/primeflex/primeflex.css",
      "node_modules/primeng/resources/themes/saga-blue/theme.css",
      "node_modules/primeng/resources/primeng.min.css",
      // ...
    ],
    ```

1. Atualizar as classes CSS do PrimeNG:

    | Deprecated | v10 | Observação |
    |-|-|-|
    | ui-g | p-grid |  |
    | ui-g-x | p-col-x | x = 1~12 |
    | ui-md-x | p-md-x | x = 1~12 |
    | ui-lg-x | p-lg-x | x = 1~12 |
    | ui-fluid | p-fluid |  |
    | ui-button | p-button |  |
    | ui-button-* | p-button-* |  |
    | ui-dropdown | p-dropdown |  |
    | ui-message | p-message |  |
    | ui-messages-* | p-messages-* |  |

    **Commits**:

    - [407ffa458812e1b8f313e1eff22caee52dc42c0c](https://github.com/fagnerlima/algamoney-ui-ng10/commit/407ffa458812e1b8f313e1eff22caee52dc42c0c)
    - [65df6a4fa66968b7ddf241395f014e68ac6a266b](https://github.com/fagnerlima/algamoney-ui-ng10/commit/65df6a4fa66968b7ddf241395f014e68ac6a266b)

1. Atualizar regras CSS das colunas das tabelas:

    **Commits**:

    - [611ebfdf7b5a55ea5d0837398f50a0385778d346](https://github.com/fagnerlima/algamoney-ui-ng10/commit/611ebfdf7b5a55ea5d0837398f50a0385778d346)

1. Atualizar regra CSS do botão-link:

    **Commits**:

    - [c2fd8d9787349fab7a4362dbe13728c6880517eb](https://github.com/fagnerlima/algamoney-ui-ng10/commit/c2fd8d9787349fab7a4362dbe13728c6880517eb)

1. Corrigir regra CSS de `.container`:

    **Commits**:

    - [06c1e18668c9d0b925766912c88abe6b2053988b](https://github.com/fagnerlima/algamoney-ui-ng10/commit/06c1e18668c9d0b925766912c88abe6b2053988b)
