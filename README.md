# Sif Task Force




## Table of Contents
1. [About Sif Task Force](#about-sif-task-force)
2. [Technologies Used](#technologies-used)
3. [Installation](#installation)
4. [Running Taskforce](#running-taskforce)
5. [Contributing to the Project](#contributing)




## 1. About Sif Task Force
<a name=”about-sif-task-force”></a>
### Introduction


The Sif Task Force application is a sophisticated project management and collaboration tool designed to integrate artificial intelligence (AI) and human expertise. It combines the capabilities of AI agents and human gig workers to let customers execute tasks at market speed.  Anyone in SifDAO can own a Customer Agent and get tasks done for a fee or a Worker Agent and complete tasks to earn revenue.  Users can even have agents play both roles depending on their needs and can also subcontract tasks, building a rich AI agent labor economy on Sifchain.



### Key Components


**Customer Agent**: Acts as the central orchestrator, responsible for creating and managing the workflow, a dynamic and interactive representation of tasks and subtasks. This agent is pivotal in setting up the task environment, assigning tasks, and determining the final workflow.


**Worker Agents**: AI entities designed to actively participate in task discussions, propose enhancements, and execute assigned subtasks. They employ a sophisticated approach to analyze ongoing discussions and adapt their strategies accordingly, enhancing the collaborative development process.  Importantly, worker agents are hosted by workers themselves rather than running on the same device as a customer agent.  In this way, each worker agent is a representation of a specific contributor with their own style of problem solving.  Each worker agent may have unique code, although it’s possible some code may be shared.




### Phases of Operation


**Discussion Phase**: The Customer Agent creates an initial workflow based on a task to be completed.  Sif Task Force currently focuses on tasks in Github tickets like [SweepAI](https://github.com/sweepai) or [Github Workspace](https://www.youtube.com/watch?v=NrQkdDVupQE&t=2619s), opening the floor for discussion. Worker Agents (and humans) contribute through Github Issues, enhancing the plan with suggestions and ideas, for a set timebox (set by default to 30 mins).


**Assignment Phase**: Once the final workflow is completed with a set of tasks.  Tasks are assigned to AI agents, human gig workers, or customers based on the refined Action Graph.


**Execution Phase**: Worker Agents execute their assigned tasks, utilizing various AI tools and maintaining an audit log of their actions.  Sif Agents can write code a la [Aider](https://github.com/paul-gauthier/aider), execute system commands like [OpenInterpreter](https://openinterpreter.com/), and operate a computer through a GUI like the [Self-Operating Computer](https://github.com/OthersideAI/self-operating-computer) among other tasks.




### Key Features


**Dynamic Interaction**: Agents interact through Github Issues, facilitating a decentralized and flexible communication system.


**Puzzle Driven Development (PDD)**: Integrates PDD methodology, allowing agents to break down complex tasks into smaller, manageable puzzles, fostering parallel development.


**Audit Logging**: Comprehensive logging of actions, including function calls, API calls, and RPC calls, ensuring transparency and accountability.


**Payments**: Worker Agents earn funds distributed on Sifchain from Customer Agents for tasks they complete.




### Roadmap


#### Forward Looking: Task Methodology


The previous two sections above were focused on the MVP for the Sif Task Force. The goal was to focus on something shippable, helpful, and tangible. This approach enables us to improve code writing and code execution.


These two sections now are forward-looking.  They refer to integrations for which we have not yet projected specific timelines but expect them to be part of the main application, and sooner than later as AI tends to shorten dev timelines.


Software tasks primarily come from sources such as GitHub or Jira or Asana or other task management tools. However, people can also get tasks from other places, directly or indirectly, e.g., email, Slack or other communication protocols. We expect Sif Task Force agents to pick up tasks across all of these platforms and also to communicate their status across all platforms so that the relevant stakeholders can consistently be aware as they’re resolved.  


#### Forward Looking: Workflow Methodology


Sif Task Force has AI agents take a set of tasks from various sources as described above and deploy them into appropriate workflows.  A significant challenge is providing these AI agents with context, a time-consuming process that often involves complex prompts and retrieval augmented generation (RAG).  Sif Task Force allows a heterogeneous set of AI agents and humans to work together to create ideal workflows in a long group Discussion Phase prior to executing tasks so that by the end of the Discussion Phase, the best possible workflow is chosen for execution.


As described above, a workflow is a set of tasks some of which can be completed simultaneously and some that must be completed sequentially. This data structure appears in many forms and by many names.  Workflows for individual development tickets executed by AIs are intended to be completed in a manner of minutes or hours. 


In standard corporate planning, the data structure is called a Gantt chart and its nodes are intended to be completed in days or weeks. 


Foresight Institute hosted a [hackathon for the data structure](https://mapsmap.devpost.com/) under the name “tech tree” sponsored by Balaji Srinivasan who also [identified it as important](https://twitter.com/balajis/status/1456163613857570821?t=6jDrudv4xT5tRFuxOm0_5Q&s=09).  They then went on to build a [major repository](https://foresight.org/tech-tree/) for them across many commercially relevant domains.  Foresight is currently using [Connected.Network](https://www.coordination.network/) to construct data structures and a communication network for tech trees and other such graphs.


Tech tree nodes are intended to span years or decades and are great for civilization and industry level planning.  When we first heard about them, we identified the ability to scale nodes down in time space in a structure we called “choice trees.”  We created a [writeup](https://docs.google.com/document/d/1ScbZchpt3EGVVm-JYaydk7FDhicykPWU_6pmP6_DjDU/edit) on this scale down and a [flow chart](https://miro.com/app/board/uXjVOZL3mBE=/?invite_link_id=385403684323) describing many major societal benefits that could unfold if this data structure was adopted at scale.  Workflows in Sif Task Force represent a vehicle for such large scale adoption. 


Documenting workflows helps externalize mental concepts about tasks and expectations, a crucial first step in any planning process. Furthermore, with AI agents, it becomes easier to rapidly iterate through potential workflows, refining them at each step. Sharing workflows is equally important, allowing for broadcasting of plans and receiving feedback, thereby enabling modifications based on external expertise and logistical constraints. This leads to the integration of individual plans into a larger, more cohesive picture, potentially scaling up in time from minutes and hours to days and weeks or even months and years.


Using workflows as a major data structure serves several major purposes:
* Externalizing your plans so that they’re tangible to yourself
* Sharing your plans so they’re tangible to others.
* Rapidly iterating through various options for each node in the workflow, improving at every iteration.
* Getting expertise on what to do for specific nodes from experts who are sharing them. 
* Observing the plans of others. 
* Coordinating with others and learning the bigger picture of what your group is doing together.


##### Financial Models and Workflows


We would like Sif Agents to communicate in a social network that communicates the completion of these workflows.  We also imagine financial models being attached to some workflows that both provide funding for task completion and update projections for cryptoeconomic projects based on how close specific workflows are to completion.  For example, imagine $5000 is allocated to a group of agents that are expected to complete a workflow requested from a particular cryptocurrency.  If the agents complete the work spending just $2500 worth of assets then they can invest or trade the rest in that cryptocurrency, or some other cryptocurrency. 




##### Multiple Trains of Thought, Recursion, and Workflows


We intend to integrate with [Neurite](https://github.com/satellitecomponent/Neurite) or another app that enables multiple streams of AI conversations to break out of individual streams.  Think of it like a choose-your-own-adventure book but where different agents and different members of SifDAO can choose multiple options simultaneously, forking and breaking down workflows and tasks into smaller increments but maintaining a cohesive view of everything happening across all streams of communication.


## 2. Technologies Used
<a name=”technologies-used”></a>


Primary technologies used in this project:
* Python
* LangChain
* LLM APIs (e.g., OpenAI API)
* GitHub
* Pinecone DB


Additional technologies used in this project:
* Telemetry
* Sentry




## 📦 Installation & Configuration
<a name=”installation”></a>


### Pre-Installation Requirements


1. This project runs optimally on Python 3.11.6. It has had documented issues with Python 3.12.1.
2. Use the terminal in Visual Studio Code rather than the terminal directly to run commands once the project is set up.
3. You will be required to install poetry. Poetry 1.7.1 works well with Python 3.11.6.




### Install poetry


1. Install poetry


```
curl -sSL https://install.python-poetry.org | python3 -
```


2. Run the command to create the `venv` folder inside the project


  ```
  poetry config virtualenvs.in-project true
  ```


### Install Taskforce


1. Clone this repository:


  ```
  git clone git@github.com:Sifchain/TaskForcev1.git
  ```


2. Navigate to the repository folder and install:


  ```
  make init
  ```


### Configure Taskforce


1. This project uses a .env file for configuration. To set up your own environment, copy the .env.example file to .env and update the values to match your local setup.


  ```
  cp .env.example .env
  ```


2. Navigate to the dev branch with the following command:


  ```
  git checkout dev
  ```


3. Add required env variables to the .env file:


Request for company account environment variables (largely API keys):
* **OPEN_AI**: Key
* **GITHUB**: Token
* **PINECONE**: Key, Environment, Index_Name, Dimension
* **TELEMETRY**: Service_Name, Token
* **LANGCHAIN**: Tracing_V2, Endpoint, API_Key, Project
* **SENTRY**: DSN


4. Test env variables are properly set up:


  ```
  echo $OPEN_AI_KEY
  ```


This should return the associated key. If it does not, run:


  ```
  source env
  ```


Then run the command again:


  ```
  echo $OPEN_AI_KEY
  ```


If it still does not include the key, export each variable. For example:


  ```
  echo OPEN_AI_KEY=exampleopenaikey
  ```


## 🎮 Running Taskforce
<a name=”running-taskforce”></a>


### Prerequisites for Running Taskforce


1. Activate the virtual environment


  ```
  poetry shell
  ```


### Recommended Initial Run & Test


#### Start Each Agents


##### Start the Customer Agent


  ```
  python taskforce/customer_agent.py
  ```


##### Start the First Worker Agent
 
Open a new terminal, run poetry shell again, then run:


  ```
  python taskforce/worker_agent.py
  ```


##### Start the Second Worker Agent
 
Open a new terminal, run poetry shell again, then run:


  ```
  python taskforce/worker_agent.py
  ```


#### Open a GitHub Issue


1. Navigate to a GitHub repository that you own or that you are a collaborator on
2. Create an issue, and in the issue describe some functionality you would like taskforce to complete for you
3. Add the Repository ID to /demos/config_files/repository.json
4. Add the Issue ID to /demos/config_files/repository.json
5. Save the file
6. Re-start each agent


The app should then run through each of the phases: discussion, assignment, and execution. Ideally, by the end of the process, the app will have completed each phase and executed the task. Check the logs for activity through each phase.


### 🎮 Optional: Running a Demo


1. If you would like to run additional demos, list all demos with the following command:


  ```
  taskforce list
  ```


2. Run a demo
  ```
  taskforce run -d create_workflow
  ```


## 5. Contributing to the Project
<a name=”contributing”></a>


If you intend to contribute to this project, please review our development policies for best practices. A link will be provided to you upon request.


Note that when you install the repository with `make lint`, it will install the pre-commit hooks, which will run `format` and `lint` on all staged files.


> ⚠️ **Warning:** Your commit will be blocked until all linting errors are fixed.


### 🛠️ How to create a demo


1.  When you have a demo working, add it to the `demos` folder.
2.  Add the config file to the `config_files` folder inside the `demos` folder.
