# atv-gantt-crystal

```mermaid
 gantt
    dateFormat  YYYY-MM-DD
    title Cronograma do Projeto - Sistema de Cadastro de Empresas Parceiras
    excludes weekends

    section Planejamento
    Levantamento de Requisitos   :done,   reqs, 2025-10-01, 7d
    Documentação e Layout        :active, docs, after reqs, 10d

    section Desenvolvimento
    Ambiente Configurado         :dev1, after docs, 10d
    Banco de Dados               :dev2, after dev1, 12d
    Login e Autenticação         :dev3, after dev2, 12d
    CRUD de Empresas             :dev4, after dev3, 14d
    Upload de Logotipo           :dev5, after dev4, 12d
    Relatórios PDF e Excel       :dev6, after dev5, 12d
    Painel Administrativo        :dev7, after dev6, 12d

    section Testes e Entrega
    Testes e Integração          :qa1, after dev7, 10d
    Usabilidade                  :qa2, after qa1, 7d
    Implantação Final            :deliver, after qa2, 5d




  ```
