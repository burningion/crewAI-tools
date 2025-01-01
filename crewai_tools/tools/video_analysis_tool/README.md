# Video Analysis Tool

## Description

This tool is used to analyze videos and extract information from them. You can pass an optional text prompt to let Video Jungle know what to search for, or pay attention to. 

You will need a Video Jungle account to get started. 


## Installation
Install the crewai_tools package
```shell
pip install 'crewai[tools]'
```

## Usage

In order to use the Video Editing Tool, the Video Jungle API key should be set in the environment variable `VJ_API_KEY`.

```python
from crewai_tools import VideoAnalysisTool

@agent
def researcher(self) -> Agent:
    return Agent(
        config=self.agents_config["researcher"],
        allow_delegation=False,
        tools=[VideoAnalysisTool]
    )
```