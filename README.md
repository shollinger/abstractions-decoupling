
# Abstractions

- Abstraction examples
  - Programming/Compiling
    - Binary (Processor)
    - Assembly (OS)
    - C/C++ (Browser Source)
    - Javascript (Browser Engine)
    - Coffeescript (Coffee Compiler)
  - Networking/Hardware
    - Sockets
    - Connections
    - Drivers
  - Frameworks
    - Layers
      - Model/View/Controller
      - Extract/Transform/Load
    - Process Cycle
      - Node Process Loop
      - Executors/Runners/Commands/Command Chains
        - Decision Tables
        - Rules Tables
      - Actors
      - Job Queues
    - Layout (Bootstrap)
      - Grid
      - Fluid
    - Ember
      - Routes
      - Bound Variables
      - Components
    - AI
      - Neural Nets
        - Neurons/Trees

# Decoupling

Elements are coupled if a change in one forces a change in the other. For example, if two classes inherit from a common parent, then a change in one class might require a change in the other. Think of a combo audio system: It’s tightly coupled because if we want to change from analog to digital radio, we must rebuild the whole system. If we assemble a system from separates, it would have low coupling and we could just swap out the receiver. “Loosely” coupled features (i.e., those with low coupling) are easier to maintain.

Some choices require you to tightly couple:

- Programming Language
- MVC Framework
- Database
- Job Queue System

With custom code that we're writing, we want to make a point to lessen the amount of coupling between our modules.  We'll have coupling with the libraries we use, but the way our modules interact with each other should be replaceable and modifiable with minimal touches.



# Finding ways to decouple (when it makes sense)

- (Seperation of Concerns)[https://en.wikipedia.org/wiki/Separation_of_concerns]

- Each module in our code should do something distinct, and the logic in the module should be grouped by something that makes sense. Using abstraction, we can divy our problem space up into various modules that each have their own purpose.  This promotes reuse and decoupling!

- In theory this makes your code much more testable as well, since each module can be tested on its own and has a clear interface. (TDD)




