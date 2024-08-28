# LangGraph Studio TypeScript Starter Template

[![CI](https://github.com/langchain-ai/langgraphjs-starter-template/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/langchain-ai/langgraphjs-starter-template/actions/workflows/unit-tests.yml)
[![Integration Tests](https://github.com/langchain-ai/langgraphjs-starter-template/actions/workflows/integration-tests.yml/badge.svg)](https://github.com/langchain-ai/langgraphjs-starter-template/actions/workflows/integration-tests.yml)

This is a (mostly empty) starter project to help you get started with developing [LangGraph.js](https://github.com/langchain-ai/langgraphjs) projects in [LangGraph Studio](https://github.com/langchain-ai/langgraph-studio).

![](/static/studio.png)

It contains a simple example graph exported from `src/agent.ts` that implements "graph" with a single node, as well as the required `langgraph.json` for opening the graph in LangGraph Studio.

## Getting Started

This template was designed for [LangGraph Studio](https://github.com/langchain-ai/langgraph-studio). To use, clone this repo locally and open the folder in LangGraph Studio.

Note that the `Deploy` button is currently not supported, but will be soon!

You will also need the latest versions of `@langchain/langgraph` and `@langchain/core`. See these instructions for help upgrading an [existing project](https://langchain-ai.github.io/langgraphjs/how-tos/manage-ecosystem-dependencies/).

You can also [click here](https://www.loom.com/share/81cafa32d57f4933bd5d9b08c70f460c?sid=4ebcb366-f27a-4c49-854d-169106b4f6fe) to see a (rough) video tour of Studio.

## Development

While iterating on your graph, you can edit past state and rerun your app from past states to debug specific nodes. Local changes will be automatically applied via hot reload. Try adding an interrupt before the agent calls tools, updating the default system message in `src/utils/state.ts` to take on a persona, or adding additional nodes and edges!

Follow up requests will be appended to the same thread. You can create an entirely new thread, clearing previous history, using the `+` button in the top right.

You can find the latest (under construction) docs on [LangGraph.js](https://langchain-ai.github.io/langgraphjs/) here, including examples and other references. Using those guides can help you pick the right patterns to adapt here for your use case.

LangGraph Studio also integrates with [LangSmith](https://smith.langchain.com/) for more in-depth tracing and collaboration with teammates.
