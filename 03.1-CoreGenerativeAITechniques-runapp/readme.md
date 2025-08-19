# Core Generative AI Techniques - Single-File Demos

> 💡 *This lesson uses the new `.NET run <file>.cs` feature available in .NET 10. If you're on an earlier version, please refer to [Lesson 03](../03-CoreGenerativeAITechniques/readme.md).*

Welcome to the modernized version of Core Generative AI Techniques! This lesson demonstrates the same powerful AI concepts as Lesson 03, but with simplified **single-file C# demos** that showcase the elegance of .NET 10's new `dotnet run` capability.

---

## What you'll learn

- 🌟 LLM completions with streamlined code
- 💬 Interactive chat flows  
- 🔧 Functions & plugins integration
- 🔍 Retrieval-Augmented Generation (RAG)
- 📊 Structured JSON outputs
- 👁️ Multimodal AI (vision analysis)

## Prerequisites

- **.NET 10 SDK** or later
- **GitHub Token** with access to GitHub Models
- Basic familiarity with C# and command line

## Setup

1. **Set your GitHub Token** (choose one method):
   ```bash
   # Option 1: Environment variable
   export GITHUB_TOKEN="your_github_token_here"
   
   # Option 2: User secrets (recommended for development)
   dotnet user-secrets set "GITHUB_TOKEN" "your_github_token_here"
   ```

2. **Navigate to the demo directory**:
   ```bash
   cd 03.1-CoreGenerativeAITechniques-runapp/src
   ```

## Single-File Demos

### 1. LLM Text Completion
**File**: `01-llm-completion.cs`  
**Concept**: Basic text completions for sentiment analysis

```bash
./run-demo.sh 01-llm-completion.cs
```

This demo shows how to:
- Set up a chat client with GitHub Models
- Create effective prompts for specific tasks
- Process single-turn AI responses
- Handle authentication and error scenarios

### 2. Interactive Chat Flow
**File**: `02-chat-flow.cs`  
**Concept**: Stateful conversations with memory

```bash
./run-demo.sh 02-chat-flow.cs
```

Learn how to:
- Maintain conversation history
- Create interactive chat experiences
- Stream responses for better UX
- Build context-aware conversations

### 3. Functions and Plugins
**File**: `03-functions-and-plugins.cs`  
**Concept**: Extending AI with custom tools

```bash
./run-demo.sh 03-functions-and-plugins.cs
```

Explore:
- Function calling with Microsoft.Extensions.AI
- Creating custom AI tools/plugins
- Automatic function invocation
- Tool descriptions and parameters

### 4. Retrieval-Augmented Generation (RAG)
**File**: `04-retrieval-augmented-generation.cs`  
**Concept**: AI + knowledge bases

```bash
./run-demo.sh 04-retrieval-augmented-generation.cs
```

Discover:
- Vector embeddings and similarity search
- In-memory vector stores
- Context injection for AI responses
- Building knowledge-aware applications

### 5. Structured Output
**File**: `05-structured-output.cs`  
**Concept**: Getting consistent JSON responses

```bash
./run-demo.sh 05-structured-output.cs
```

Master:
- Structured data extraction
- JSON schema compliance
- Type-safe AI responses
- Business data processing

### 6. Multimodal AI (Vision)
**File**: `06-multimodal.cs`  
**Concept**: Analyzing images with AI

```bash
./run-demo.sh 06-multimodal.cs
```

Learn about:
- Vision-enabled AI models
- Image analysis and description
- URL and local file processing
- Multimodal conversation flows

## Key Features of These Demos

### ✨ Simplified Architecture
- **No project files** - Pure single-file C# programs
- **Top-level statements** - Reduced boilerplate code
- **Minimal dependencies** - Focus on core AI concepts

### 🚀 Modern .NET 10 Features
- **Direct file execution** with `dotnet run file.cs`
- **Implicit global usings** for cleaner code
- **Latest AI libraries** - Microsoft.Extensions.AI integration

### 🎯 Educational Focus
- **Progressive complexity** - Start simple, build up
- **Clear examples** - Real-world, runnable scenarios
- **Best practices** - Error handling, authentication, logging

## Running the Demos

Since .NET 10 isn't released yet, we provide a helper script that simulates the single-file execution experience:

### Option 1: Using the Helper Script (Recommended)
```bash
# Make the script executable (first time only)
chmod +x run-demo.sh

# Run any demo
./run-demo.sh 01-llm-completion.cs
./run-demo.sh 02-chat-flow.cs
./run-demo.sh 03-functions-and-plugins.cs
# ... and so on
```

### Option 2: Manual Execution
Create a temporary project and copy the demo file as Program.cs, then run with `dotnet run`.

### Option 3: When .NET 10 is Available
```bash
# Future: Direct file execution with .NET 10
dotnet run 01-llm-completion.cs
dotnet run 02-chat-flow.cs
# ... and so on
```

## Common Issues & Solutions

### Authentication Errors
- Ensure your `GITHUB_TOKEN` has access to GitHub Models
- Check that the token is properly set in environment variables or user secrets

### .NET 10 Not Available?
- If you're using an earlier .NET version, the helper script `run-demo.sh` simulates the `.NET 10 run file.cs` experience
- The concepts and code are identical - only the execution method differs
- Refer to the full project-based examples in [Lesson 03](../03-CoreGenerativeAITechniques/readme.md) for traditional project structure

### Model Availability
- These demos use GitHub Models for accessibility
- You can modify the endpoint and credentials to use Azure OpenAI, Ollama, or other providers

## Next Steps

- **Experiment** with the prompts and parameters
- **Combine** techniques from multiple demos
- **Build** your own AI-powered applications
- **Explore** [Lesson 04 - Practical Samples](../04-PracticalSamples/readme.md) for complete applications

---

> 🙋 **Need help?** Check out the main [Lesson 03 documentation](../03-CoreGenerativeAITechniques/readme.md) for more detailed explanations, or open an issue in the repository.

**Happy coding with .NET and AI! 🚀**