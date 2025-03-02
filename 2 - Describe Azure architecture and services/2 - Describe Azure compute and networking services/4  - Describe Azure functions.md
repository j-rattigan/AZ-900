# Azure Functions Overview
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
- **Azure Functions** is an **event-driven**, **serverless compute** option.
- Unlike **VMs** or **containers**, there’s no need to keep resources running when not in use.
- **Functions** are triggered by events, and resources are automatically deallocated when finished.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **Azure Functions**: A serverless compute option that runs code in response to events without needing a dedicated infrastructure (like VMs or containers).
- **Event-Driven**: The function is triggered by an event, such as a REST request or timer.
- **Serverless**: No need to manage or provision servers; Azure automatically handles resources.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
- **Azure Functions** run **only when triggered** and **automatically scale** based on demand, making them ideal for **variable workloads**.
- You only pay for **CPU time** used when the function is running.

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- Example of **event-driven** trigger: A **REST request** starts the function, which runs quickly (in seconds) and then **shuts down** after completion.
- Functions can be **stateless** (restart on each event) or **stateful** (with context passed between events).

# Benefits of Azure Functions
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
- **Serverless model** means no need to maintain infrastructure.
- Functions are perfect for **quick tasks** like responding to events, timers, or messages from other Azure services.
- **Automatic scaling** ensures that functions handle variable demand with ease.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **Serverless Computing**: No infrastructure to manage; the cloud provider handles resources.
- **Stateless Functions**: Functions that do not maintain context between executions.
- **Stateful Functions (Durable Functions)**: Functions that maintain context and track prior activities.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
- **Stateless Functions** restart every time they respond to an event.
- **Stateful (Durable) Functions** can track activities and maintain context between function calls, useful for workflows.

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- If you need **workflow management**, **Durable Functions** (stateful) are ideal for tracking tasks over time.
- With **serverless**, you **only pay** for time spent executing the function, reducing costs.
  
# Flexibility of Azure Functions
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
- **Azure Functions** can easily transition from a serverless environment to other environments, like **virtual networks**, for more control over scaling and isolation.
- **Functions** are **general-purpose** and can run **any code**, providing flexibility based on the app's needs.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **Virtual Networks**: Private networks within Azure where resources can communicate securely.
- **Scaling**: The ability to increase or decrease the capacity of resources based on demand.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
- You can **isolate** functions or deploy them in environments that provide **scaling** and **network control** for more complex scenarios.

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- If your app requires more **control** over the environment, functions can be deployed in a more **traditional server-based setup**.
