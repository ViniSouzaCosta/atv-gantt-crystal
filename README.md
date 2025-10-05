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
    subgraph Ciclo de Vida do Projeto (Crystal Clear)
        A[Levantamento de Requisitos e Documentação]:::design --> B{Design de Telas e Layout}:::design
        B --> C[Configuração do Ambiente]:::dev
        C --> D1[Semana 3: Entrega 1 - Login]:::dev
        D1 --> R1{Revisão e Validação da Diretoria (Entrega 1)}:::review
        R1 --> D2[Semana 6: Entrega 2 - CRUD de Empresas]:::dev
        D2 --> R2{Revisão e Validação da Diretoria (Entrega 2)}:::review
        R2 --> D3[Semana 8: Entrega 3 - Upload de Logotipo]:::dev
        D3 --> R3{Revisão e Validação da Diretoria (Entrega 3)}:::review
        R3 --> D4[Semana 10: Entrega 4 - Relatórios]:::dev
        D4 --> R4{Revisão e Validação da Diretoria (Entrega 4)}:::review
        R4 --> D5[Semana 12: Entrega 5 - Painel Administrativo]:::dev
        D5 --> R5{Revisão e Validação da Diretoria (Entrega 5)}:::review
        R5 --> T1[Testes Unitários e de Integração (QA)]:::test
        T1 --> T2[Testes de Usabilidade com Usuários Convidados]:::test
        T2 --> F[Mês 6: Implantação e Entrega Final Validada]:::final
    end

    classDef design fill:#ADD8E6,stroke:#000,stroke-width:2px;
    classDef dev fill:#FFD700,stroke:#000,stroke-width:2px;
    classDef review fill:#FFA233,stroke:#000,stroke-width:2px;
    classDef test fill:#90EE90,stroke:#000,stroke-width:2px;
    classDef final fill:#E64C3C,stroke:#000,stroke-width:2px;
```
