# Tools In LangChain

This repository showcases practical examples and patterns for building intelligent agents using LangChain's agent framework and custom tools. It demonstrates how to integrate external tools, manage agent memory, handle multi-step reasoning, and design dynamic tool-using agents.

## Introduction

LangChain is a powerful framework for developing applications powered by language models, and one of its key features is the ability to augment language models with tools. This repository provides a comprehensive set of examples that illustrate different approaches to creating and using tools within the LangChain ecosystem.

The examples in this repository progress from basic to advanced implementations, making it suitable for both beginners looking to understand the fundamentals and experienced developers seeking to implement more sophisticated tool patterns.

## Repository Contents

This repository contains several Jupyter notebooks, each focusing on a different aspect of tool implementation in LangChain:

### 1. Built-in Tools

The "1- Built-in-Tools.ipynb" notebook introduces LangChain's pre-built tools that are ready to use out of the box. It demonstrates how to leverage existing tools like search engines, calculators, and other utilities that LangChain provides. This notebook serves as an excellent starting point for understanding how tools function within the LangChain framework without having to implement custom functionality.

### 2. Custom Tools Using Decorators

The "2-Custom_Tool_Using_@Tool.ipynb" notebook explores how to create custom tools using LangChain's `@tool` decorator. This approach offers a straightforward way to transform Python functions into LangChain tools with minimal boilerplate code. The notebook demonstrates how to define tool names, descriptions, and input/output parameters, making it easy for language models to understand how to use these tools effectively.

### 3. Structured Output Tools

The "3-CustomToolUsingStructuredOutput.ipynb" notebook delves into creating tools that return structured data. It showcases how to use Pydantic models to define the schema for tool inputs and outputs, ensuring type safety and enabling more complex data handling. This approach is particularly valuable when working with tools that need to process or return structured information that follows specific formats.

### 4. Base Tool Class Implementation

The "4-CustomToolUsingBaseToolClass.ipynb" notebook demonstrates a more advanced approach by extending LangChain's BaseTool class. This method provides greater flexibility and control over tool behavior, including custom validation, error handling, and more complex execution logic. The notebook shows how to implement tools that can handle optional parameters and conditional execution paths.

### 5. Tool Kits

The "ToolKit.ipynb" notebook illustrates how to organize multiple related tools into a cohesive toolkit. This approach is useful when developing agents that need access to a suite of related functionalities. The notebook demonstrates how to create a toolkit class that provides a collection of tools that work together to solve more complex problems.

## Getting Started

To use the examples in this repository, you'll need to have Python installed along with the LangChain library and its dependencies. You can install the required packages using pip:

```
pip install langchain
```

Depending on the specific examples, you might also need additional packages such as:

```
pip install pydantic
```

Once you have the necessary dependencies installed, you can run the Jupyter notebooks to explore the different approaches to implementing tools in LangChain.

## Use Cases

The patterns demonstrated in this repository can be applied to a wide range of applications, including:

- Building conversational agents that can access external data sources
- Creating assistants that can perform calculations or data transformations
- Developing agents that can interact with APIs or databases
- Implementing systems that can reason through multi-step problems using a combination of tools

## Contributing

Contributions to this repository are welcome! If you have additional examples, improvements to existing notebooks, or documentation enhancements, please feel free to submit a pull request.

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

This repository was created to help developers understand and implement tool patterns in LangChain. Special thanks to the LangChain community for their ongoing contributions to the ecosystem.
