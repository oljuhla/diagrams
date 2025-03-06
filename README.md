# diagrams
Testing autogenerated mermaid diagrams

```mermaid
graph TD;
  subgraph Services
    A[database]
    B[inkvisitor]
  end

  subgraph Networks
    N[inkvisitor]
  end

  A -->|Network Connection| N
  B -->|Network Connection| N

  A -->|Exposes port| X(8080:8080 / 28015:28015)
  B -->|Exposes port| Y(3000:3000)

  B -->|Uses DB_HOST| A
```
