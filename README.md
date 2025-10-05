# atv-gantt-crystal

```mermaid
gantt
    dateFormat  YYYY-MM-DD
    title Cronograma do Projeto - Sistema de Cadastro de Empresas Parceiras
    excludes weekends

    section Planejamento
    Req.                     :done,    reqs, 2025-10-01, 7d
    Doc. e Layout           :active,  docs, after reqs, 10d

    section Desenvolvimento
    Amb. Config.           :dev1, after docs, 7d
    Banco de Dados                  :dev2, after dev1, 10d
    Login e Autenticação            :dev3, after dev2, 12d
    CRUD de Empresas                :dev4, after dev3, 14d
    Upload Logotipo                 :dev5, after dev4, 10d
    Relat. PDF e Excel              :dev6, after dev5, 10d
    Painel Administrativo           :dev7, after dev6, 12d

    section Testes e Entrega
    Test. e Integ.                  :qa1, after dev7, 10d
    Usabilidade                     :qa2, after qa1, 7d
    Impla. Final                    :deliver, after qa2, 5d





  ```
```mermaid
graph TD
    subgraph Matriz
    A1("C8"):::branco --> A2("C20"):::amarelo --> A3("V50"):::laranja --> A4("V100"):::vermelho
    B1("D8"):::branco --> B2("C20"):::amarelo --> B3("E50"):::laranja --> B4("E100"):::vermelho
    C1("D8"):::branco --> C2("D20"):::amarelo --> C3("D50"):::laranja --> C4("D100"):::vermelho
    D1("C8"):::branco --> D2("C20"):::amarelo --> D3("C50"):::laranja --> D4("C100"):::vermelho
    end

    classDef branco fill:#FFF, stroke:#000, stroke-width:1px;
    classDef amarelo fill:#FFD84D, stroke:#000, stroke-width:1px;
    classDef laranja fill:#FFA233, stroke:#000, stroke-width:1px;
    classDef vermelho fill:#E64C3C, stroke:#000, stroke-width:1px;
```
