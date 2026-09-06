# My Agent Demo

## Project Overview

**My Agent Demo** is a lightweight framework that showcases how to build intelligent, conversational agents using OpenAI's GPT models. The project provides a modular architecture for creating, configuring, and deploying agents with custom tools, memory, and routing capabilities.

The repository includes:
- Core agent abstractions and utilities.
- Example agents demonstrating various use‑cases.
- A CLI for quick experimentation.
- Comprehensive documentation to get you started.

## Features

- **Modular design** – plug‑in custom tools, memory stores, and routing logic.
- **Easy configuration** – configure agents via YAML or Python dictionaries.
- **Extensible CLI** – run agents, test prompts, and debug interactions.
- **Test suite** – includes unit tests for core components.

## Setup Instructions

### Prerequisites

- Python 3.9 or newer
- An OpenAI API key (set as `OPENAI_API_KEY` environment variable)
- `git` installed

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/my-agent-demo.git
cd my-agent-demo

# Create a virtual environment
python -m venv .venv
source .venv/bin/activate  # On Windows use `.venv\Scripts\activate`

# Install dependencies
pip install -r requirements.txt
```

### Development Setup

For contributors, install the development dependencies:

```bash
pip install -r requirements-dev.txt
```

## Usage Examples

### Running the Demo Agent

```bash
python -m my_agent_demo.run --config examples/demo_config.yaml
```

### Interacting via the CLI

```bash
my-agent-cli "Summarize the latest news about AI advancements."
```

### Adding a Custom Tool

Create a new Python module in `my_agent_demo/tools/`:

```python
# my_agent_demo/tools/custom_tool.py
from my_agent_demo.core import Tool

class CustomTool(Tool):
    name = "custom_tool"
    description = "Performs a custom operation."

    def run(self, input_text: str) -> str:
        # Your implementation here
        return f"Processed: {input_text}"
```

Then register it in the agent configuration.

## Contribution Guidelines

We welcome contributions! Please see our [CONTRIBUTING.md](CONTRIBUTING.md) for details on:
- Setting up the development environment
- Submitting pull requests
- Coding standards and testing
- Reporting issues

## License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.