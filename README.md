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
        A1[Semana 3 Login Entrega 1]:::branco --> A2[Semana 6 CRUD Empresas Entrega 2]:::amarelo
        A2 --> A3[Semana 8 Upload Logotipo Entrega 3]:::laranja
        A3 --> A4[Mês 6 Entrega Final]:::vermelho
        
        B1[Semana 10 Relatórios PDF/Excel Entrega 4]:::branco --> B2[Semana 12 Painel Administrativo Entrega 5]:::amarelo
        B2 --> B3[Testes e Usabilidade]:::laranja
        B3 --> B4[Mês 6 Sistema Validado]:::vermelho
    end

    classDef branco fill:#ffffff,stroke:#000,stroke-width:1px;
    classDef amarelo fill:#FFD700,stroke:#000,stroke-width:1px;
    classDef laranja fill:#FFA500,stroke:#000,stroke-width:1px;
    classDef vermelho fill:#E64C3C,stroke:#000,stroke-width:1px;
```
