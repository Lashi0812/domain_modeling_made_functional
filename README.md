# Part 1 - Understanding the domain

## **Software Development as a Pipeline**

Think of software development as a pipeline: **requirements in, deliverables out**.The "garbage in, garbage out" rule applies—**poor input** (unclear requirements, bad design) leads to **bad output**, no matter the coding effort.coding effort.**DDD** emphasizes clear communication and shared domain knowledge to improve design and requirements.

## Understanding the problem

Understand the problem thoroughly before solving it—**incomplete understanding** leads to poor solutions.- Developers’ understanding is what gets implemented, not the domain experts’.- **Written specifications** often create a disconnect between domain experts and the development team.

![telephone_game](/assets/telephone_game.png)

Misunderstandings between developers and domain experts can **derail projects**. Involve **domain experts directly** in an iterative process with feedback loops to minimize misunderstandings.Agile development helps but **translating** domain knowledge into code can still cause **distortions**.

![agile](/assets/agile.png)

**Domain-Driven Design (DDD)** aims to create a **shared model** where the code directly reflects domain knowledge, minimizing translation errors.

![shared_mental_model](/assets/shared_mental_model.png)

### Guidelines for creating a Shared Model

- **Focus on business events and workflows** rather than just data structures.
- **Partition the problem domain** into smaller, manageable subdomains.
- **Model each subdomain** as part of the solution.
- Develop a **Ubiquitous Language**—a common language shared by everyone in the project and used consistently throughout the code.

### Domain Events

Focus on **business events** instead of just **data structures** to understand value creation through data transformation. Identify **Domain Events** that trigger business processes (e.g., “new order form received” starts order processing).

Recognize that static data alone does not add value; it requires triggers (external, time-based, or observational) to become useful.Domain Events are written in the **past tense**, reflecting completed actions that serve as factual references.

**Event Storming** is a collaborative workshop technique for identifying business events and workflows.
