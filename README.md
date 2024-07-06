# AutoGen experiments

This project is a learning exercise on learning LLM agents using [AutoGen](https://microsoft.github.io/autogen/).

Examples of items to explore:

- How to use agents to solve a task.
- What are the limitations? For example, do we need GPT-4, or could a simpler (and cheaper) model do the job?
- How many tokens do we consume for the agents and the behind-the-scenes processing (the selection and coordination of the agents)?

## How to use this project

If you haven't done so yet, [prepare the environment](#preparing-the-environment). If you have already prepared the environment, activate it with `source venv/bin/activate`.

Each notebook is a self-contained experiment. You can run them in any order.

You may need to select a Python kernel the first time you open a notebook. Choose the kernel from the virtual environment you created.

- [Sequential chat](./sequential_chat_example.ipynb): Given a starting and ending number, select math operators (agents) to transform the starting number into the ending number.

## Preparing the environment

### OpenAI key

Create a file named `.env` in the root of the project with the following content:

```bash
OPENAI_API_KEY=your-openai-api-key
```

This file is in the `.gitignore`. It will never be committed to the repository.

### Python environment

This is a one-time step. If you have already done this, just activate the virtual environment with `source venv/bin/activate`.

Run the following commands to create a virtual environment and install the required packages.

```bash
python3 -m venv venv
source venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```
