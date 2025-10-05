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
    Test. e Integ.             :qa1, after dev7, 10d
    Usabilidade                     :qa2, after qa1, 7d
    Implantação Final               :deliver, after qa2, 5d





  ```
