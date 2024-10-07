# FinancialAnalyst Crew

Welcome to the FinancialAnalyst Crew project, powered by [crewAI](https://crewai.com). This template is designed to help you set up a multi-agent AI system with ease, leveraging the powerful and flexible framework provided by crewAI. Our goal is to enable your agents to collaborate effectively on complex tasks, maximizing their collective intelligence and capabilities.

## Installation

Ensure you have Python >=3.10 <=3.13 installed on your system. This project uses [Poetry](https://python-poetry.org/) for dependency management and package handling, offering a seamless setup and execution experience.

First, if you haven't already, install Poetry:

```bash
pip install poetry
```

Next, navigate to your project directory and install the dependencies:

1. First lock the dependencies and install them by using the CLI command:
```bash
crewai install
```
### Customizing

**Add your `OPENAI_API_KEY` into the `.env` file**

- Modify `src/financial_analyst/config/agents.yaml` to define your agents
- Modify `src/financial_analyst/config/tasks.yaml` to define your tasks
- Modify `src/financial_analyst/crew.py` to add your own logic, tools and specific args
- Modify `src/financial_analyst/main.py` to add custom inputs for your agents and tasks

## Running the Project

To kickstart your crew of AI agents and begin task execution, run this from the root folder of your project:

```bash
$ crewai run
```

This command initializes the financial_analyst Crew, assembling the agents and assigning them tasks as defined in your configuration.

This example, unmodified, will run the create a `report.md` file with the output of a research on LLMs in the root folder.

## Understanding Your Crew

The financial_analyst Crew is composed of multiple AI agents, each with unique roles, goals, and tools. These agents collaborate on a series of tasks, defined in `config/tasks.yaml`, leveraging their collective skills to achieve complex objectives. The `config/agents.yaml` file outlines the capabilities and configurations of each agent in your crew.

## Support

For support, questions, or feedback regarding the FinancialAnalyst Crew or crewAI.
- Docs  [documentation](https://docs.crewai.com)
- Git [GitHub repository](https://github.com/joaomdmoura/crewai)
- GPT Doc agent [Chat with our docs](https://chatg.pt/DWjSBZn)

Let's create wonders together with the power and simplicity of crewAI.

# Learning  

## Tools
What makes a great tool ? 
- Verasatile - Making agents use different data types JASON string Int
- Fault Tolerant 
  - Exception handling. Fail gracefully (Try again) 
  - Self healing
  - Use case : Able to handle large no of docs and numbers might not be easy to read, text is not easy to parse
- Caching
    - Cross-agent caching (Use common tools) 
    - Use Case: 
      - Prevent unnecessary requests
      - stay within rate limits (Number of requests per second allowed for an API call)
      - Save time( retrieving cached results is much faster than an API call)
    ### Examples
        Examples of tools
Examples of tools
• Search the internet
• Scrape a website
• Connect to a database
• Call an API
• Send notifications

and many more


    
