# AlgaWorks - Atualização para Angular 10

- [ ] Instalar o **@angular/cli 10** globalmente:

    ```
    npm i -g @angular/cli@10
    ```

- [ ] Remover dependências incompatíveis e não utilizadas:

    ```
    npm rm ng2-toasty
    ```

- [ ] Remover os códigos das dependências removidas:

    angular.json
    ```json
    "styles": [
      "node_modules/ng2-toasty/style-bootstrap.css",
      // ...
    ],
    ```

- [ ] Executar os passos do [Angular Update Guide](https://update.angular.io/#9.1:10.0):

    ```
    ng update @angular/core @angular/cli
    ```

- [ ] Adicionar as folhas de estilo do PrimeNG:

    ```json
    "styles": [
      "node_modules/primeicons/primeicons.css",
      "node_modules/primeng/resources/themes/saga-blue/theme.css",
      "node_modules/primeng/resources/primeng.min.css",
      // ...
    ],
    ```

- [ ] Instalar a dependência PrimeFlex:

    ```
    npm install primeflex --save
    ```

- [ ] Adicionar a folha de estilo do PrimeFlex:

    ```json
    "styles": [
      "node_modules/primeflex/primeflex.css",
      // ...
    ]
    ```

- [ ] Atualizar as classes CSS do PrimeNG:

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

- [ ] Atualizar regras CSS das colunas das tabelas:

    **Commits**:

    - [611ebfdf7b5a55ea5d0837398f50a0385778d346](https://github.com/fagnerlima/algamoney-ui-ng10/commit/611ebfdf7b5a55ea5d0837398f50a0385778d346)
