# Agent Definitions
```python
from langgraph.prebuilt import create_react_agent
from langchain_openai import ChatOpenAI

def get_research_agent(tools):
    model = ChatOpenAI(model="gpt-4o")
    return create_react_agent(model, tools)
```