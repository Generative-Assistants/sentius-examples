# Getting started

## What is Sentius Teach and Repeat Platform?

Sentius Teach & Repeat Platform is an **agentic platform** that enables teams and companies to automate individual tasks and entire workflows using millions of concurrent autonomous AI agents working together humans under human supervision.

 <iframe width="560" height="315"
src="https://www.youtube.com/watch?v=zwLQnmHttGk" 
frameborder="0" 
allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" 
allowfullscreen></iframe>

AI agent, by definition, is a software component that is connected to one or more tools, and capable of figuring out how to solve a particular task on its own with minimal to no human intervention - **autonomously**. 

Our first AI agent is **browser agent**. It is designed to intelligently navigate websites to autonomously complete tasks like interacting with them or extracting data from them.

> For example, you can ask Sentius browser agent to find a quarterly financial results presentation of a public company:

<iframe width="560" height="315"
src="https://youtu.be/hzhXlfm8ELw" 
frameborder="0" 
allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" 
allowfullscreen></iframe>

Our second AI agent is **OpenAPI agent**. It is designed to interact with a given web service's REST APIs as long as those APIs are described based on OpenAPI standard.

> For example, you can configure Sentius OpenAPI agent to ask a e-commerces shipping service like [FreightOS](https://ship.freightos.com/api/shippingCalculator) to calculate shipping estimates for moving goods from China to US.

Our third AI agent is **Prompt agent**. It interacts with an LLM to perform tasks that do not require use of any tools, like providing a structured response to a question based on data obtained by other AI agents, or generating summaries etc.

> For example, you can ask Sentius prompt agent to look at the data collected by the **browser agent** and transform it into a form that is native for a given OpenAPI to be called by **OpenAPI agent**.

There are more AI agents currently in development, like **document agent** capable of finding answers to a given question within a provided document or set of documents, **desktop agent** designed to control desktop applications across Windows and macOS, with even more coming in the future.

> You can learn more about our vision of Agentic Enterprise in our [Whitepaper](https://www.sentius.ai/blog/sentius-white-paper).

Now that you have a grasp of what AI agents are and what they can do for you, imagine that you want to make your organization more efficient using their power:

1. You start with delegating small, individual tasks isolated from each other, to autonomous AI agents, like checking your customers' driver licenses on a DMV website of their driver license using our **browser agent**. 
2. As you start seeing the positive effect of having these tasks automated, you want to combine more and more such tasks delegated to various autonomous AI agents (**browser agent**, **OpenAPI agent**, **prompt agent** etc.) into multi-step workflows, to increase the level of automation. 
3. Over the time, you want to expand your workflows to more and more areas of work in your organization, but some tasks have to be done by people, and so you add people to the mix (**human-in-the-loop**). 
4. Finally, as you see your information work automated at the acceptable level for your company, you want to automate physical work, too, and so you delegate it to **physical robots** also powered by our AI agents combined together into multi-step workflows (coming in 2026+).

## How Sentius Teach & Repeat Platform Works

At conceptual level, Sentius **agentic platform** starts with **autonomous AI agents** that can work on their own, or organized to work together within the **agentic workflows**.

At user level, Sentius **agentic platform** starts with three components that make it easy to build autonomous agents and complex workflows:

* [Sentius Copilot+](platform-components/sentius-copilot-plus.md) - Electron-based desktop application that controls web browsers (and, later, desktop apps) across Windows, macOS, and Ubuntu.

* [Sentius Studio](platform-components/sentius-studio.md) - native desktop application that allows creation, editing, testing, deployment, and monitoring of complex workflows. Currently supports Windows 10+, with macOS support coming later in 2025.

* [Sentius Workflow Engine](platform-components/sentius-workflow-engine.md) - agentic workflow engine designed to run complex multi-agent workflows. Works in the cloud.

### End-Users

If you want to automate your work using Sentius **agentic platform**, you can start with [Sentius Copilot+](platform-components/sentius-copilot-plus.md). With it, you can ask the system to intelligently navigate websites to execute tasks for you, be that filling out the forms or extracting data. You can either ask it to figure out the task on its own, or you can show it how to execute that task by using its **Recorder** feature.

If you want to build more complex automations, you can download [Sentius Studio](platform-components/sentius-studio.md). With it, you can build workflows that involve multiple website automation tasks done by our **browser agent**, text manipulation using LLMs done by our **prompt agent**, and, if you are up to it, calls to REST APIs of the web services done by our **OpenAPI agent**.

With Sentius Studio, you can run your automations locally on your computer, or you can deploy them to Sentius cloud platform. 

### Developers

If you want to automate work using our **browser agent** by integrating it into your existing applications, you can use our [browser agent API](api/browser-agent-api.md).

If you want to incorporate more than one **browser agent** or multiple **autonomous AI agents**, you can use our [workflow engine API](api/workflow-engine-api.md).

Start with [Quick Start](quick-start).

## Get Support

Want to get in touch with the Sentius team? Reach out to us via [email](mailto:ask@sentius.ai).

You're all set! Discover how to use the API in the [Quick Start](quick-start).
