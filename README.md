### integrantes da equipe:<br>

|Rm|Nome|Turma
|--|--|--|
RM99503|Arthur Koga|TDSA
RM552254|Gabriel Benjamim|TDSA
RM550684|Henry Ribeiro|TDSR
RM99538|Murilo José|TDSR
RM98021|Pedro Sena|TDSA

 Sprint 4 .Net
#### Uma Api com estrutura de um e-commerce com gerenciamento de contas

## Arquitetura da API 
### Microservices:
'Microservices' é vantajosa para aplicações de e-commerce devido a suas características de escalabilidade, flexibilidade e independência entre componentes. Em um sistema de e-commerce, vários serviços independentes, como pagamento, catálogo de produtos, carrinho de compras, estoque, e gerenciamento de usuários, podem ser gerenciados separadamente. Isso permite que cada serviço possa ser desenvolvido, escalado e mantido de forma independente.

### Vantagens:
- **Escalabilidade:** Permite escalar componentes específicos conforme a demanda. Por exemplo, em períodos de grande volume, o serviço de carrinho ou de checkout pode ser escalado sem necessidade de escalar o sistema inteiro, otimizando o uso de recursos e reduzindo custos.
- **Gerenciamento de Dados por Contexto:** Com microservices, dados podem ser gerenciados de acordo com o contexto. Assim, o serviço de estoque pode ter seu próprio banco de dados otimizado, enquanto o serviço de pagamento pode ter um sistema dedicado com alta segurança.
- **Atualizações e Implementações Contínuas:** A arquitetura facilita a CI/CD (Integração e Entrega Contínuas), permitindo que novos recursos e correções sejam lançados com mais frequência e menos riscos.
---

## Diferenças entre arquitetura Monolítica e Microservices

### Monolítica

#### A arquitetura monolítica é um estilo de construção de software no qual todas as funcionalidades de uma aplicação estão centralizadas em um único código-base. Esse tipo de arquitetura era amplamente utilizado em projetos de software no passado

- Facilidade inicial de desenvolvimento: Para projetos pequenos, é mais rápido e simples começar com uma arquitetura monolítica, já que tudo está centralizado e não há necessidade de gerenciar comunicações entre serviços.

- Dificuldade de escalabilidade: A escalabilidade é mais complexa, pois geralmente é preciso escalar toda a aplicação, mesmo que apenas uma parte dela necessite de mais recursos.

- Manutenção complicada em sistemas grandes: À medida que o sistema cresce, a manutenção torna-se difícil, com equipes maiores enfrentando desafios para gerenciar o código, os testes e a implantação.

- Unidade única: Todo o sistema (front-end, back-end, lógica de negócio, banco de dados) está em um único aplicativo ou código-base.

- Implantação conjunta: Todo o sistema é implantado como uma unidade, o que significa que qualquer mudança ou atualização requer a reimplantação completa da aplicação.

---

### Microservices

#### A arquitetura de microservices é um estilo de design de software em que uma aplicação é dividida em vários serviços pequenos e independentes, cada um responsável por uma função específica do sistema. Esses serviços são executados separadamente, se comunicam entre si por meio de APIs ou mensagens assíncronas, e podem ser desenvolvidos, implantados e escalados de forma autônoma.

- Divisão por serviços independentes: O sistema é dividido em vários serviços menores, onde cada um é responsável por uma funcionalidade específica. Cada serviço tem seu próprio ciclo de vida, banco de dados (ou compartilhado) e pode ser desenvolvido, implantado e escalado separadamente.

- Baixo acoplamento: Os serviços são fracamente acoplados e comunicam-se entre si por meio de APIs (geralmente usando HTTP/REST ou mensagens assíncronas). Isso facilita a alteração de um serviço sem impactar os demais.

- Desenvolvimento distribuído: Permite que diferentes equipes trabalhem em serviços distintos de forma autônoma, usando tecnologias e frameworks diferentes, se necessário.

- Maior resiliência: Como os serviços são independentes, falhas em um serviço específico não necessariamente afetam o sistema inteiro, aumentando a tolerância a falhas.

- Complexidade de gerenciamento: A complexidade de gerenciar uma arquitetura multiservice pode ser maior, pois cada serviço requer seu próprio monitoramento, manutenção, integração e gerenciamento de dependências.
