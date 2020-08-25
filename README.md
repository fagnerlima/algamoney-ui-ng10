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
    ```

1. Adicionar as folhas de estilo do PrimeNG:

    ```json
    "styles": [
      "node_modules/primeicons/primeicons.css",
      "node_modules/primeng/resources/themes/saga-blue/theme.css",
      "node_modules/primeng/resources/primeng.min.css",
      // ...
    ],
    ```

1. Instalar a dependência PrimeFlex:

    ```
    npm install primeflex --save
    ```

1. Adicionar a folha de estilo do PrimeFlex:

    ```json
    "styles": [
      "node_modules/primeflex/primeflex.css",
      // ...
    ]
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

    **Commits**:

    - [407ffa458812e1b8f313e1eff22caee52dc42c0c](https://github.com/fagnerlima/algamoney-ui-ng10/commit/407ffa458812e1b8f313e1eff22caee52dc42c0c)
