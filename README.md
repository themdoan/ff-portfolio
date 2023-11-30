# ff-portfolio

### Architect Diagram

```mermaid
flowchart LR;
 user(user)-- request -->frontend(frontend);
 subgraph serverless
 frontend-->backend(backend);
 backend-- cache -->cache[Redis];
 backend-->db[(Database)];
 end
```