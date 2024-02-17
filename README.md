- 👋 Hi, I’m @CAVILACA
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
CAVILACA/CAVILACA is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can 
click the Preview link to take a look at your changes.
--->
graph TD
    A[Envio de Pedido] -->|Pedido enviado| B(Envio de Orçamento)
    B -->|Orçamento enviado| C{Resposta a Orçamento}
    C -->|Aprovado| D[Envio de Pedido para Departamento de Planejamento]
    C -->|Não Aprovado| E[Arquivado]
    D -->|Pedido de atribuição| F[Atribuição de Operador]

    classDef inicio fill:#f9f,stroke:#333,stroke-width:4px;
    classDef processo fill:#bbf,stroke:#f66,stroke-width:2px;
    classDef decisao fill:#faa,stroke:#333,stroke-width:2px;
    classDef fim fill:#dfd,stroke:#333,stroke-width:2px;

    class A inicio;
    class B,C,D,E,F processo;
    class C decisao;
    class E,F fim;
