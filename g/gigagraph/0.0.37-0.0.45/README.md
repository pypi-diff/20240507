# Comparing `tmp/gigagraph-0.0.37.tar.gz` & `tmp/gigagraph-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigagraph-0.0.37.tar", max compression
+gzip compressed data, was "gigagraph-0.0.45.tar", max compression
```

## Comparing `gigagraph-0.0.37.tar` & `gigagraph-0.0.45.tar`

### file list

```diff
@@ -1,40 +1,46 @@
--rw-r--r--   0        0        0     1067 2024-02-09 11:26:26.015908 gigagraph-0.0.37/LICENSE
--rw-r--r--   0        0        0    51559 2024-04-15 10:02:14.913807 gigagraph-0.0.37/README.md
--rw-r--r--   0        0        0       69 2024-03-06 08:45:49.220137 gigagraph-0.0.37/langgraph/__init__.py
--rw-r--r--   0        0        0      294 2024-02-09 11:26:26.068963 gigagraph-0.0.37/langgraph/channels/__init__.py
--rw-r--r--   0        0        0     1682 2024-04-15 10:02:15.008130 gigagraph-0.0.37/langgraph/channels/any_value.py
--rw-r--r--   0        0        0     4254 2024-04-15 10:02:15.008653 gigagraph-0.0.37/langgraph/channels/base.py
--rw-r--r--   0        0        0     2028 2024-04-15 10:02:15.009503 gigagraph-0.0.37/langgraph/channels/binop.py
--rw-r--r--   0        0        0     3180 2024-04-15 10:02:15.010265 gigagraph-0.0.37/langgraph/channels/context.py
--rw-r--r--   0        0        0     1917 2024-04-15 10:02:15.010661 gigagraph-0.0.37/langgraph/channels/ephemeral_value.py
--rw-r--r--   0        0        0     1706 2024-04-15 10:02:15.011057 gigagraph-0.0.37/langgraph/channels/last_value.py
--rw-r--r--   0        0        0     1715 2024-04-15 10:02:15.011411 gigagraph-0.0.37/langgraph/channels/named_barrier_value.py
--rw-r--r--   0        0        0     2584 2024-04-15 10:02:15.011871 gigagraph-0.0.37/langgraph/channels/topic.py
--rw-r--r--   0        0        0      302 2024-04-15 10:02:15.013003 gigagraph-0.0.37/langgraph/checkpoint/__init__.py
--rw-r--r--   0        0        0     5336 2024-04-15 10:02:15.014124 gigagraph-0.0.37/langgraph/checkpoint/aiosqlite.py
--rw-r--r--   0        0        0     4187 2024-04-15 10:02:15.015222 gigagraph-0.0.37/langgraph/checkpoint/base.py
--rw-r--r--   0        0        0     2958 2024-04-15 10:02:15.016282 gigagraph-0.0.37/langgraph/checkpoint/memory.py
--rw-r--r--   0        0        0     5570 2024-04-15 10:02:15.017297 gigagraph-0.0.37/langgraph/checkpoint/sqlite.py
--rw-r--r--   0        0        0      130 2024-04-15 10:02:15.018515 gigagraph-0.0.37/langgraph/constants.py
--rw-r--r--   0        0        0      197 2024-02-09 11:26:26.074907 gigagraph-0.0.37/langgraph/graph/__init__.py
--rw-r--r--   0        0        0    13150 2024-04-15 10:02:15.019737 gigagraph-0.0.37/langgraph/graph/graph.py
--rw-r--r--   0        0        0     1429 2024-04-15 10:02:15.020907 gigagraph-0.0.37/langgraph/graph/message.py
--rw-r--r--   0        0        0    10606 2024-04-15 10:02:15.021710 gigagraph-0.0.37/langgraph/graph/state.py
--rw-r--r--   0        0        0      372 2024-04-15 10:02:15.022782 gigagraph-0.0.37/langgraph/prebuilt/__init__.py
--rw-r--r--   0        0        0     5464 2024-04-15 10:02:15.023557 gigagraph-0.0.37/langgraph/prebuilt/agent_executor.py
--rw-r--r--   0        0        0     8356 2024-04-15 10:02:15.024860 gigagraph-0.0.37/langgraph/prebuilt/chat_agent_executor.py
--rw-r--r--   0        0        0     2232 2024-04-15 10:02:15.025852 gigagraph-0.0.37/langgraph/prebuilt/tool_executor.py
--rw-r--r--   0        0        0     3320 2024-04-15 10:02:15.026606 gigagraph-0.0.37/langgraph/prebuilt/tool_node.py
--rw-r--r--   0        0        0    46579 2024-04-15 10:02:15.028119 gigagraph-0.0.37/langgraph/pregel/__init__.py
--rw-r--r--   0        0        0     1240 2024-04-15 10:02:15.028845 gigagraph-0.0.37/langgraph/pregel/debug.py
--rw-r--r--   0        0        0     3305 2024-04-15 10:02:15.030157 gigagraph-0.0.37/langgraph/pregel/io.py
--rw-r--r--   0        0        0       53 2024-02-09 11:26:26.080872 gigagraph-0.0.37/langgraph/pregel/log.py
--rw-r--r--   0        0        0     7750 2024-04-15 10:02:15.031108 gigagraph-0.0.37/langgraph/pregel/read.py
--rw-r--r--   0        0        0      752 2024-04-15 10:02:15.031470 gigagraph-0.0.37/langgraph/pregel/types.py
--rw-r--r--   0        0        0     3057 2024-04-15 10:02:15.032091 gigagraph-0.0.37/langgraph/pregel/validate.py
--rw-r--r--   0        0        0     3867 2024-04-15 10:02:15.032754 gigagraph-0.0.37/langgraph/pregel/write.py
--rw-r--r--   0        0        0        0 2024-04-15 10:02:15.032946 gigagraph-0.0.37/langgraph/py.typed
--rw-r--r--   0        0        0     2282 2024-04-15 10:02:15.033610 gigagraph-0.0.37/langgraph/utils.py
--rw-r--r--   0        0        0      308 2024-03-06 08:45:49.226704 gigagraph-0.0.37/langgraph/version.py
--rw-r--r--   0        0        0     2240 2024-04-15 10:02:15.034893 gigagraph-0.0.37/pyproject.toml
--rw-r--r--   0        0        0    52186 1970-01-01 00:00:00.000000 gigagraph-0.0.37/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-02-09 11:26:26.015908 gigagraph-0.0.45/LICENSE
+-rw-r--r--   0        0        0    55971 2024-05-07 12:24:35.831230 gigagraph-0.0.45/README.md
+-rw-r--r--   0        0        0       69 2024-03-06 08:45:49.220137 gigagraph-0.0.45/langgraph/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 12:22:43.018411 gigagraph-0.0.45/langgraph/_api/__init__.py
+-rw-r--r--   0        0        0      999 2024-05-07 12:22:43.018975 gigagraph-0.0.45/langgraph/_api/deprecation.py
+-rw-r--r--   0        0        0      294 2024-02-09 11:26:26.068963 gigagraph-0.0.45/langgraph/channels/__init__.py
+-rw-r--r--   0        0        0     1682 2024-04-15 10:02:15.008130 gigagraph-0.0.45/langgraph/channels/any_value.py
+-rw-r--r--   0        0        0     4346 2024-05-07 12:22:43.019826 gigagraph-0.0.45/langgraph/channels/base.py
+-rw-r--r--   0        0        0     2028 2024-04-15 10:02:15.009503 gigagraph-0.0.45/langgraph/channels/binop.py
+-rw-r--r--   0        0        0     3180 2024-04-15 10:02:15.010265 gigagraph-0.0.45/langgraph/channels/context.py
+-rw-r--r--   0        0        0     2834 2024-04-25 14:37:42.876970 gigagraph-0.0.45/langgraph/channels/dynamic_barrier_value.py
+-rw-r--r--   0        0        0     1917 2024-04-15 10:02:15.010661 gigagraph-0.0.45/langgraph/channels/ephemeral_value.py
+-rw-r--r--   0        0        0     1706 2024-04-15 10:02:15.011057 gigagraph-0.0.45/langgraph/channels/last_value.py
+-rw-r--r--   0        0        0     1715 2024-04-15 10:02:15.011411 gigagraph-0.0.45/langgraph/channels/named_barrier_value.py
+-rw-r--r--   0        0        0     2584 2024-04-15 10:02:15.011871 gigagraph-0.0.45/langgraph/channels/topic.py
+-rw-r--r--   0        0        0      264 2024-05-07 12:22:43.020532 gigagraph-0.0.45/langgraph/checkpoint/__init__.py
+-rw-r--r--   0        0        0    10902 2024-05-07 12:22:43.021204 gigagraph-0.0.45/langgraph/checkpoint/aiosqlite.py
+-rw-r--r--   0        0        0     5028 2024-05-07 12:22:43.021627 gigagraph-0.0.45/langgraph/checkpoint/base.py
+-rw-r--r--   0        0        0     7175 2024-05-07 12:22:43.022096 gigagraph-0.0.45/langgraph/checkpoint/memory.py
+-rw-r--r--   0        0        0    14067 2024-05-07 12:22:43.022534 gigagraph-0.0.45/langgraph/checkpoint/sqlite.py
+-rw-r--r--   0        0        0      130 2024-04-15 10:02:15.018515 gigagraph-0.0.45/langgraph/constants.py
+-rw-r--r--   0        0        0      227 2024-05-07 12:22:43.024093 gigagraph-0.0.45/langgraph/graph/__init__.py
+-rw-r--r--   0        0        0    16889 2024-05-07 12:22:43.024636 gigagraph-0.0.45/langgraph/graph/graph.py
+-rw-r--r--   0        0        0     5193 2024-05-07 12:22:43.025088 gigagraph-0.0.45/langgraph/graph/message.py
+-rw-r--r--   0        0        0    14221 2024-05-07 12:22:43.025714 gigagraph-0.0.45/langgraph/graph/state.py
+-rw-r--r--   0        0        0      412 2024-04-25 14:37:42.883452 gigagraph-0.0.45/langgraph/prebuilt/__init__.py
+-rw-r--r--   0        0        0     6828 2024-05-07 12:22:43.026180 gigagraph-0.0.45/langgraph/prebuilt/agent_executor.py
+-rw-r--r--   0        0        0    12572 2024-05-07 12:22:43.064745 gigagraph-0.0.45/langgraph/prebuilt/chat_agent_executor.py
+-rw-r--r--   0        0        0     3799 2024-05-07 12:22:43.026542 gigagraph-0.0.45/langgraph/prebuilt/tool_executor.py
+-rw-r--r--   0        0        0     5415 2024-05-07 12:22:43.026941 gigagraph-0.0.45/langgraph/prebuilt/tool_node.py
+-rw-r--r--   0        0        0    56342 2024-05-07 12:22:43.028589 gigagraph-0.0.45/langgraph/pregel/__init__.py
+-rw-r--r--   0        0        0     4700 2024-05-07 12:22:43.029048 gigagraph-0.0.45/langgraph/pregel/debug.py
+-rw-r--r--   0        0        0     4037 2024-05-07 12:22:43.029383 gigagraph-0.0.45/langgraph/pregel/io.py
+-rw-r--r--   0        0        0       56 2024-04-25 14:37:42.892127 gigagraph-0.0.45/langgraph/pregel/log.py
+-rw-r--r--   0        0        0     7750 2024-04-15 10:02:15.031108 gigagraph-0.0.45/langgraph/pregel/read.py
+-rw-r--r--   0        0        0      939 2024-05-07 12:22:43.029710 gigagraph-0.0.45/langgraph/pregel/types.py
+-rw-r--r--   0        0        0     3273 2024-05-07 12:22:43.030069 gigagraph-0.0.45/langgraph/pregel/validate.py
+-rw-r--r--   0        0        0     3994 2024-04-25 14:37:42.892705 gigagraph-0.0.45/langgraph/pregel/write.py
+-rw-r--r--   0        0        0        0 2024-04-15 10:02:15.032946 gigagraph-0.0.45/langgraph/py.typed
+-rw-r--r--   0        0        0        0 2024-04-25 14:37:42.892851 gigagraph-0.0.45/langgraph/serde/__init__.py
+-rw-r--r--   0        0        0      425 2024-05-07 13:07:19.022804 gigagraph-0.0.45/langgraph/serde/base.py
+-rw-r--r--   0        0        0     3790 2024-05-07 12:22:43.030687 gigagraph-0.0.45/langgraph/serde/jsonplus.py
+-rw-r--r--   0        0        0     5843 2024-05-07 12:22:43.031261 gigagraph-0.0.45/langgraph/utils.py
+-rw-r--r--   0        0        0      308 2024-03-06 08:45:49.226704 gigagraph-0.0.45/langgraph/version.py
+-rw-r--r--   0        0        0     2240 2024-05-07 12:24:12.852406 gigagraph-0.0.45/pyproject.toml
+-rw-r--r--   0        0        0    56595 1970-01-01 00:00:00.000000 gigagraph-0.0.45/PKG-INFO
```

### Comparing `gigagraph-0.0.37/LICENSE` & `gigagraph-0.0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.37/README.md` & `gigagraph-0.0.45/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -22,18 +22,199 @@
 ```
 
 ## Быстрый старт
 
 Ниже приводится пример разработки агента, использующего несколько моделей и вызов функций.
 Агент отображает каждое свое состояние в виде отдельных сообщений в списке
 
-Для работы агента потребуется установить некоторые пакеты LangChain и использовать в качестве демонстрации сервис [Tavily](https://app.tavily.com/sign-in):
+Для работы агента потребуется установить некоторые пакеты GigaChain и использовать в качестве демонстрации сервис [Tavily](https://app.tavily.com/sign-in):
+
+State in LangGraph can be pretty general, but to keep things simpler to start, we'll show off an example where the graph's state is limited to a list of chat messages using the built-in `MessageGraph` class. This is convenient when using LangGraph with LangChain chat models because we can return chat model output directly.
+
+First, install the GigaChain OpenAI integration package:
+
+```python
+pip install gigachain_openai
+```
+
+We also need to export some environment variables:
 
 ```shell
-pip install -U langchain langchain_openai tavily-python
+export OPENAI_API_KEY=sk-...
+```
+
+And now we're ready! The graph below contains a single node called `"oracle"` that executes a chat model, then returns the result:
+
+```python
+from langchain_openai import ChatOpenAI
+from langchain_core.messages import HumanMessage
+from langgraph.graph import END, MessageGraph
+
+model = ChatOpenAI(temperature=0)
+
+graph = MessageGraph()
+
+graph.add_node("oracle", model)
+graph.add_edge("oracle", END)
+
+graph.set_entry_point("oracle")
+
+runnable = graph.compile()
+```
+
+Let's run it!
+
+```python
+runnable.invoke(HumanMessage("What is 1 + 1?"))
+```
+
+```
+[HumanMessage(content='What is 1 + 1?'), AIMessage(content='1 + 1 equals 2.')]
+```
+
+So what did we do here? Let's break it down step by step:
+
+1. First, we initialize our model and a `MessageGraph`.
+2. Next, we add a single node to the graph, called `"oracle"`, which simply calls the model with the given input.
+3. We add an edge from this `"oracle"` node to the special string `END`. This means that execution will end after current node.
+4. We set `"oracle"` as the entrypoint to the graph.
+5. We compile the graph, ensuring that no more modifications to it can be made.
+
+Then, when we execute the graph:
+
+1. LangGraph adds the input message to the internal state, then passes the state to the entrypoint node, `"oracle"`.
+2. The `"oracle"` node executes, invoking the chat model.
+3. The chat model returns an `AIMessage`. LangGraph adds this to the state.
+4. Execution progresses to the special `END` value and outputs the final state.
+
+And as a result, we get a list of two chat messages as output.
+
+### Interaction with LCEL
+
+As an aside for those already familiar with LangChain - `add_node` actually takes any function or runnable as input. In the above example, the model is used "as-is", but we could also have passed in a function:
+
+```python
+def call_oracle(messages: list):
+    return model.invoke(messages)
+
+graph.add_node("oracle", call_oracle)
+```
+
+Just make sure you are mindful of the fact that the input to the runnable is the **entire current state**. So this will fail:
+
+```python
+# This will not work with MessageGraph!
+from langchain_core.prompts import ChatPromptTemplate, MessagesPlaceholder
+
+prompt = ChatPromptTemplate.from_messages([
+    ("system", "You are a helpful assistant named {name} who always speaks in pirate dialect"),
+    MessagesPlaceholder(variable_name="messages"),
+])
+
+chain = prompt | model
+
+# State is a list of messages, but our chain expects a dict input:
+#
+# { "name": some_string, "messages": [] }
+#
+# Therefore, the graph will throw an exception when it executes here.
+graph.add_node("oracle", chain)
+```
+
+## Conditional edges
+
+Now, let's move onto something a little bit less trivial. Because math can be difficult for LLMs, let's allow the LLM to conditionally call a `"multiply"` node using tool calling.
+
+We'll recreate our graph with an additional `"multiply"` that will take the result of the most recent message, if it is a tool call, and calculate the result.
+We'll also [bind](https://api.python.langchain.com/en/latest/chat_models/langchain_openai.chat_models.base.ChatOpenAI.html#langchain_openai.chat_models.base.ChatOpenAI.bind_tools) the calculator to the OpenAI model as a tool to allow the model to optionally use the tool necessary to respond to the current state:
+
+```python
+from langchain_core.tools import tool
+from langgraph.prebuilt import ToolNode
+
+@tool
+def multiply(first_number: int, second_number: int):
+    """Multiplies two numbers together."""
+    return first_number * second_number
+
+model = ChatOpenAI(temperature=0)
+model_with_tools = model.bind_tools([multiply])
+
+graph = MessageGraph()
+
+graph.add_node("oracle", model_with_tools)
+
+tool_node = ToolNode([multiply])
+graph.add_node("multiply", tool_node)
+
+graph.add_edge("multiply", END)
+
+graph.set_entry_point("oracle")
+```
+
+Now let's think - what do we want to have happened?
+
+- If the `"oracle"` node returns a message expecting a tool call, we want to execute the `"multiply"` node
+- If not, we can just end execution
+
+We can achieve this using **conditional edges**, which routes execution to a node based on the current state using a function.
+
+Here's what that looks like:
+
+```python
+def router(state: List[BaseMessage]):
+    tool_calls = state[-1].additional_kwargs.get("tool_calls", [])
+    if len(tool_calls):
+        return "multiply"
+    else:
+        return "end"
+
+graph.add_conditional_edges("oracle", router, {
+    "multiply": "multiply",
+    "end": END,
+})
+```
+
+If the model output contains a tool call, we move to the `"multiply"` node. Otherwise, we end.
+
+Great! Now all that's left is to compile the graph and try it out. Math-related questions are routed to the calculator tool:
+
+```python
+runnable = graph.compile()
+
+runnable.invoke(HumanMessage("What is 123 * 456?"))
+```
+
+```
+
+[HumanMessage(content='What is 123 * 456?'),
+ AIMessage(content='', additional_kwargs={'tool_calls': [{'id': 'call_OPbdlm8Ih1mNOObGf3tMcNgb', 'function': {'arguments': '{"first_number":123,"second_number":456}', 'name': 'multiply'}, 'type': 'function'}]}),
+ ToolMessage(content='56088', tool_call_id='call_OPbdlm8Ih1mNOObGf3tMcNgb')]
+```
+
+While conversational responses are outputted directly:
+
+```python
+runnable.invoke(HumanMessage("What is your name?"))
+```
+
+```
+[HumanMessage(content='What is your name?'),
+ AIMessage(content='My name is Assistant. How can I assist you today?')]
+```
+
+## Cycles
+
+Now, let's go over a more general example with a cycle. We will recreate the `AgentExecutor` class from LangChain. The agent itself will use chat models and function calling.
+This agent will represent all its state as a list of messages.
+
+We will need to install some GigaChain packages, as well as [Tavily](https://app.tavily.com/sign-in) to use as an example tool.
+
+```shell
+pip install -U gigachain gigachain_openai tavily-python
 ```
 
 Также для доступа к OpenAI и Tavily API понадобится задать переменные среды:
 
 ```shell
 export OPENAI_API_KEY=sk-...
 export TAVILY_API_KEY=tvly-...
@@ -85,18 +266,15 @@
 model = ChatOpenAI(temperature=0, streaming=True)
 ```
 
 После подключения убедитесь, что модель знает, какие инструменты доступны ей.
 Для этого преобразуйте инструменты GigaGraph в формат OpenAI-функций и привяжите их к классу модели.
 
 ```python
-from langchain.tools.render import format_tool_to_openai_function
-
-functions = [format_tool_to_openai_function(t) for t in tools]
-model = model.bind_functions(functions)
+model = model.bind_tools(tools)
 ```
 
 ### Определите состояние агента
 
 Основным графом `gigagraph` является `StatefulGraph`.
 Этот граф параметризован объектом состояния, который он передает каждой вершине.
 В свою очередь каждая вершина возвращает операции для обновления состояния.
@@ -105,21 +283,22 @@
 
 В приведенном примере отслеживаемое состояние представлено в виде списка сообщений.
 Поэтому нужно чтобы каждая вершина добавляла сообщения в список.
 
 Для этого используйте `TypedDict` с одним ключом (`messages`) и аннотацией, указывающей на то, что в атрибут `messages` можно только добавлять данные.
 
 ```python
-from typing import TypedDict, Annotated, Sequence
-import operator
-from langchain_core.messages import BaseMessage
+from typing import TypedDict, Annotated
+from langgraph.graph.message import add_messages
 
 
 class AgentState(TypedDict):
-    messages: Annotated[Sequence[BaseMessage], operator.add]
+    # The `add_messages` function within the annotation defines
+    # *how* updates should be merged into the state.
+    messages: Annotated[list, add_messages]
 ```
 
 ### Определите вершины графа
 
 Теперь нужно определить несколько разных вершин графа.
 В `langgraph` вершина может быть представлена в виде функции или [исполняемого интерфейса](https://python.langchain.com/docs/expression_language/).
 Для описываемого примера понадобятся две основных вершины:
@@ -313,100 +492,15 @@
 
 ```
 content='' additional_kwargs={'function_call': {'arguments': '', 'name': 'tavily_search_results_json'}}
 content='' additional_kwargs={'function_call': {'arguments': '{\n', 'name': ''}}
 content='' additional_kwargs={'function_call': {'arguments': ' ', 'name': ''}}
 content='' additional_kwargs={'function_call': {'arguments': ' "', 'name': ''}}
 content='' additional_kwargs={'function_call': {'arguments': 'query', 'name': ''}}
-content='' additional_kwargs={'function_call': {'arguments': '":', 'name': ''}}
-content='' additional_kwargs={'function_call': {'arguments': ' "', 'name': ''}}
-content='' additional_kwargs={'function_call': {'arguments': 'weather', 'name': ''}}
-content='' additional_kwargs={'function_call': {'arguments': ' in', 'name': ''}}
-content='' additional_kwargs={'function_call': {'arguments': ' San', 'name': ''}}
-content='' additional_kwargs={'function_call': {'arguments': ' Francisco', 'name': ''}}
-content='' additional_kwargs={'function_call': {'arguments': '"\n', 'name': ''}}
-content='' additional_kwargs={'function_call': {'arguments': '}', 'name': ''}}
-content=''
-content=''
-content='I'
-content="'m"
-content=' sorry'
-content=','
-content=' but'
-content=' I'
-content=' couldn'
-content="'t"
-content=' find'
-content=' the'
-content=' current'
-content=' weather'
-content=' in'
-content=' San'
-content=' Francisco'
-content='.'
-content=' However'
-content=','
-content=' you'
-content=' can'
-content=' check'
-content=' the'
-content=' historical'
-content=' weather'
-content=' data'
-content=' for'
-content=' January'
-content=' '
-content='202'
-content='4'
-content=' in'
-content=' San'
-content=' Francisco'
-content=' ['
-content='here'
-content=']('
-content='https'
-content='://'
-content='we'
-content='athers'
-content='park'
-content='.com'
-content='/h'
-content='/m'
-content='/'
-content='557'
-content='/'
-content='202'
-content='4'
-content='/'
-content='1'
-content='/H'
-content='istorical'
-content='-'
-content='Weather'
-content='-in'
-content='-Jan'
-content='uary'
-content='-'
-content='202'
-content='4'
-content='-in'
-content='-S'
-content='an'
-content='-F'
-content='r'
-content='anc'
-content='isco'
-content='-Cal'
-content='ifornia'
-content='-'
-content='United'
-content='-'
-content='States'
-content=').'
-content=''
+...
 ```
 
 ## Область применения
 
 Используйте библиотеку если вам нужна поддержка циклов.
 
 Если обычной работы с цепочками для решения ваших задач достаточно, используйте основные возможности [LangChain Expression Language](https://python.langchain.com/docs/expression_language/).
@@ -434,15 +528,15 @@
 
 LangGraph comes with built-in support for human-in-the-loop workflows. This is useful when you want to have a human review the current state before proceeding to a particular node.
 For a walkthrough on how to do that, see [this documentation](https://github.com/langchain-ai/langgraph/blob/main/examples/human-in-the-loop.ipynb)
 
 ### Visualizing the graph
 
 Agents you create with LangGraph can be complex. In order to make it easier to understand what is happening under the hood, we've added methods to print out and visualize the graph.
-This can create both ascii art as well as pngs.
+This can create both ascii art and pngs.
 For a walkthrough on how to do that, see [this documentation](https://github.com/langchain-ai/langgraph/blob/main/examples/visualization.ipynb)
 
 ### "Time Travel"
 
 With "time travel" functionality you can jump to any point in the graph execution, modify the state, and rerun from there.
 This is useful for both debugging workflows, as well as end user-facing workflows to allow them to correct the state.
 For a walkthrough on how to do that, see [this documentation](https://github.com/langchain-ai/langgraph/blob/main/examples/time-travel.ipynb)
```

### Comparing `gigagraph-0.0.37/langgraph/channels/any_value.py` & `gigagraph-0.0.45/langgraph/channels/any_value.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.37/langgraph/channels/base.py` & `gigagraph-0.0.45/langgraph/channels/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,20 +121,22 @@
             await v.__aexit__(None, None, None)
 
 
 def create_checkpoint(
     checkpoint: Checkpoint, channels: Mapping[str, BaseChannel]
 ) -> Checkpoint:
     """Create a checkpoint for the given channels."""
+    ts = datetime.now(timezone.utc).isoformat()
+    assert ts > checkpoint["ts"], "Timestamps must be monotonically increasing"
     values: dict[str, Any] = {}
     for k, v in channels.items():
         try:
             values[k] = v.checkpoint()
         except EmptyChannelError:
             pass
     return Checkpoint(
         v=1,
-        ts=datetime.now(timezone.utc).isoformat(),
+        ts=ts,
         channel_values=values,
         channel_versions=checkpoint["channel_versions"],
         versions_seen=checkpoint["versions_seen"],
     )
```

### Comparing `gigagraph-0.0.37/langgraph/channels/binop.py` & `gigagraph-0.0.45/langgraph/channels/binop.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.37/langgraph/channels/context.py` & `gigagraph-0.0.45/langgraph/channels/context.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.37/langgraph/channels/ephemeral_value.py` & `gigagraph-0.0.45/langgraph/channels/ephemeral_value.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.37/langgraph/channels/last_value.py` & `gigagraph-0.0.45/langgraph/channels/last_value.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.37/langgraph/channels/named_barrier_value.py` & `gigagraph-0.0.45/langgraph/channels/named_barrier_value.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.37/langgraph/channels/topic.py` & `gigagraph-0.0.45/langgraph/channels/topic.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.37/langgraph/checkpoint/base.py` & `gigagraph-0.0.45/langgraph/pregel/write.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,151 +1,125 @@
-from abc import ABC
-from collections import defaultdict
-from copy import deepcopy
-from datetime import datetime, timezone
-from typing import (
-    Any,
-    AsyncIterator,
-    Iterator,
-    NamedTuple,
-    Optional,
-    Protocol,
-    TypedDict,
-)
-
-from langchain_core.runnables import ConfigurableFieldSpec, RunnableConfig
-
-from langgraph.utils import StrEnum
-
-
-class Checkpoint(TypedDict):
-    """State snapshot at a given point in time."""
-
-    v: int
-    """The version of the checkpoint format. Currently 1."""
-    ts: str
-    """The timestamp of the checkpoint in ISO 8601 format."""
-    channel_values: dict[str, Any]
-    """The values of the channels at the time of the checkpoint.
-    
-    Mapping from channel name to channel snapshot value.
-    """
-    channel_versions: defaultdict[str, int]
-    """The versions of the channels at the time of the checkpoint.
-    
-    The keys are channel names and the values are the logical time step
-    at which the channel was last updated.
-    """
-    versions_seen: defaultdict[str, defaultdict[str, int]]
-    """Map from node ID to map from channel name to version seen.
-    
-    This keeps track of the versions of the channels that each node has seen.
-    
-    Used to determine which nodes to execute next.
-    """
-
-
-def _seen_dict():
-    return defaultdict(int)
-
-
-def empty_checkpoint() -> Checkpoint:
-    return Checkpoint(
-        v=1,
-        ts=datetime.now(timezone.utc).isoformat(),
-        channel_values={},
-        channel_versions=defaultdict(int),
-        versions_seen=defaultdict(_seen_dict),
-    )
-
-
-def copy_checkpoint(checkpoint: Checkpoint) -> Checkpoint:
-    return Checkpoint(
-        v=checkpoint["v"],
-        ts=checkpoint["ts"],
-        channel_values=checkpoint["channel_values"].copy(),
-        channel_versions=checkpoint["channel_versions"].copy(),
-        versions_seen=deepcopy(checkpoint["versions_seen"]),
-    )
-
-
-class CheckpointAt(StrEnum):
-    END_OF_STEP = "end_of_step"
-    END_OF_RUN = "end_of_run"
+from __future__ import annotations
 
+import asyncio
+from typing import Any, Callable, NamedTuple, Optional, Sequence, TypeVar
 
-class CheckpointTuple(NamedTuple):
-    config: RunnableConfig
-    checkpoint: Checkpoint
-    parent_config: Optional[RunnableConfig] = None
+from langchain_core.runnables import Runnable, RunnableConfig
+from langchain_core.runnables.utils import ConfigurableFieldSpec
 
+from langgraph.constants import CONFIG_KEY_SEND
+from langgraph.utils import RunnableCallable
 
-CheckpointThreadId = ConfigurableFieldSpec(
-    id="thread_id",
-    annotation=str,
-    name="Thread ID",
-    description=None,
-    default="",
-    is_shared=True,
-)
+TYPE_SEND = Callable[[Sequence[tuple[str, Any]]], None]
+R = TypeVar("R", bound=Runnable)
 
-CheckpointThreadTs = ConfigurableFieldSpec(
-    id="thread_ts",
-    annotation=Optional[str],
-    name="Thread Timestamp",
-    description="Pass to fetch a past checkpoint. If None, fetches the latest checkpoint.",
-    default=None,
-    is_shared=True,
-)
 
+SKIP_WRITE = object()
+PASSTHROUGH = object()
 
-class SerializerProtocol(Protocol):
-    def dumps(self, obj: Any) -> bytes: ...
 
-    def loads(self, data: bytes) -> Any: ...
+class ChannelWriteEntry(NamedTuple):
+    channel: str
+    value: Any = PASSTHROUGH
+    skip_none: bool = False
+    mapper: Optional[Runnable] = None
 
 
-class BaseCheckpointSaver(ABC):
-    at: CheckpointAt = CheckpointAt.END_OF_STEP
-
-    serde: SerializerProtocol
+class ChannelWrite(RunnableCallable):
+    writes: Sequence[ChannelWriteEntry]
+    """
+    Sequence of write entries, each of which is a tuple of:
+    - channel name
+    - runnable to map input, or None to use the input, or any other value to use instead
+    - whether to skip writing if the mapped value is None
+    """
 
     def __init__(
-        self,
-        *,
-        serde: Optional[SerializerProtocol] = None,
-        at: Optional[CheckpointAt] = None,
-    ) -> None:
-        self.serde = serde or self.serde
-        self.at = at or self.at
+        self, writes: Sequence[ChannelWriteEntry], *, tags: Optional[list[str]] = None
+    ):
+        super().__init__(func=self._write, afunc=self._awrite, name=None, tags=tags)
+        self.writes = writes
+
+    def __repr_args__(self) -> Any:
+        return [("writes", self.writes)]
+
+    def get_name(
+        self, suffix: Optional[str] = None, *, name: Optional[str] = None
+    ) -> str:
+        if not name:
+            name = f"ChannelWrite<{','.join(chan for chan, _, _, _ in self.writes)}>"
+        return super().get_name(suffix, name=name)
 
     @property
     def config_specs(self) -> list[ConfigurableFieldSpec]:
-        return [CheckpointThreadId, CheckpointThreadTs]
-
-    def get(self, config: RunnableConfig) -> Optional[Checkpoint]:
-        if value := self.get_tuple(config):
-            return value.checkpoint
-
-    def get_tuple(self, config: RunnableConfig) -> Optional[CheckpointTuple]:
-        raise NotImplementedError
-
-    def list(self, config: RunnableConfig) -> Iterator[CheckpointTuple]:
-        raise NotImplementedError
-
-    def put(self, config: RunnableConfig, checkpoint: Checkpoint) -> RunnableConfig:
-        raise NotImplementedError
-
-    async def aget(self, config: RunnableConfig) -> Optional[Checkpoint]:
-        if value := await self.aget_tuple(config):
-            return value.checkpoint
-
-    async def aget_tuple(self, config: RunnableConfig) -> Optional[CheckpointTuple]:
-        raise NotImplementedError
-
-    async def alist(self, config: RunnableConfig) -> AsyncIterator[CheckpointTuple]:
-        raise NotImplementedError
-
-    async def aput(
-        self, config: RunnableConfig, checkpoint: Checkpoint
-    ) -> RunnableConfig:
-        raise NotImplementedError
+        return [
+            ConfigurableFieldSpec(
+                id=CONFIG_KEY_SEND,
+                name=CONFIG_KEY_SEND,
+                description=None,
+                default=None,
+                annotation=None,
+            ),
+        ]
+
+    def _write(self, input: Any, config: RunnableConfig) -> None:
+        values = [
+            input if write.value is PASSTHROUGH else write.value
+            for write in self.writes
+        ]
+        values = [
+            val if write.mapper is None else write.mapper.invoke(val, config)
+            for val, write in zip(values, self.writes)
+        ]
+        values = [
+            (write.channel, val)
+            for val, write in zip(values, self.writes)
+            if not write.skip_none or val is not None
+        ]
+        self.do_write(config, **dict(values))
+        return input
+
+    async def _awrite(self, input: Any, config: RunnableConfig) -> None:
+        values = [
+            input if write.value is PASSTHROUGH else write.value
+            for write in self.writes
+        ]
+        values = await asyncio.gather(
+            *(
+                _mk_future(val)
+                if write.mapper is None
+                else write.mapper.ainvoke(val, config)
+                for val, write in zip(values, self.writes)
+            )
+        )
+        values = [
+            (write.channel, val)
+            for val, write in zip(values, self.writes)
+            if not write.skip_none or val is not None
+        ]
+        self.do_write(config, **dict(values))
+        return input
+
+    @staticmethod
+    def do_write(config: RunnableConfig, **values: Any) -> None:
+        write: TYPE_SEND = config["configurable"][CONFIG_KEY_SEND]
+        write([(chan, val) for chan, val in values.items() if val is not SKIP_WRITE])
+
+    @staticmethod
+    def is_writer(runnable: Runnable) -> bool:
+        return (
+            isinstance(runnable, ChannelWrite)
+            or getattr(runnable, "_is_channel_writer", False) is True
+        )
+
+    @staticmethod
+    def register_writer(runnable: R) -> R:
+        # using object.__setattr__ to work around objects that override __setattr__
+        # eg. pydantic models and dataclasses
+        object.__setattr__(runnable, "_is_channel_writer", True)
+        return runnable
+
+
+def _mk_future(val: Any) -> asyncio.Future:
+    fut = asyncio.Future()
+    fut.set_result(val)
+    return fut
```

### Comparing `gigagraph-0.0.37/langgraph/graph/graph.py` & `gigagraph-0.0.45/langgraph/graph/graph.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 import logging
 from collections import defaultdict
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
+    Literal,
     NamedTuple,
     Optional,
     Sequence,
     Union,
     cast,
+    get_args,
+    get_origin,
+    get_type_hints,
 )
 
 from langchain_core.runnables import Runnable
-from langchain_core.runnables.base import RunnableLike, coerce_to_runnable
+from langchain_core.runnables.base import RunnableLike
 from langchain_core.runnables.config import RunnableConfig
 from langchain_core.runnables.graph import (
-    Graph as RunnableGraph,
-)
-from langchain_core.runnables.graph import (
     Node as RunnableGraphNode,
 )
 
 from langgraph.channels.ephemeral_value import EphemeralValue
 from langgraph.checkpoint import BaseCheckpointSaver
 from langgraph.constants import TAG_HIDDEN
 from langgraph.pregel import Channel, Pregel
 from langgraph.pregel.read import PregelNode
+from langgraph.pregel.types import All
 from langgraph.pregel.write import ChannelWrite, ChannelWriteEntry
-from langgraph.utils import RunnableCallable
+from langgraph.utils import DrawableGraph, RunnableCallable, coerce_to_runnable
 
 logger = logging.getLogger(__name__)
 
 START = "__start__"
 END = "__end__"
 
 
 class Branch(NamedTuple):
-    condition: Runnable[Any, Union[str, list[str]]]
+    path: Runnable[Any, Union[str, list[str]]]
     ends: Optional[dict[str, str]]
+    then: Optional[str] = None
 
     def run(
         self,
         writer: Callable[[list[str]], Optional[Runnable]],
         reader: Optional[Callable[[RunnableConfig], Any]] = None,
     ) -> None:
         return ChannelWrite.register_writer(
@@ -60,15 +63,15 @@
         self,
         input: Any,
         config: RunnableConfig,
         *,
         reader: Optional[Callable[[], Any]],
         writer: Callable[[list[str]], Optional[Runnable]],
     ) -> Runnable:
-        result = self.condition.invoke(reader(config) if reader else input, config)
+        result = self.path.invoke(reader(config) if reader else input, config)
         if not isinstance(result, list):
             result = [result]
         if self.ends:
             destinations = [self.ends[r] for r in result]
         else:
             destinations = result
         return writer(destinations) or input
@@ -77,17 +80,15 @@
         self,
         input: Any,
         config: RunnableConfig,
         *,
         reader: Optional[Callable[[], Any]],
         writer: Callable[[list[str]], Optional[Runnable]],
     ) -> Runnable:
-        result = await self.condition.ainvoke(
-            reader(config) if reader else input, config
-        )
+        result = await self.path.ainvoke(reader(config) if reader else input, config)
         if not isinstance(result, list):
             result = [result]
         if self.ends:
             destinations = [self.ends[r] for r in result]
         else:
             destinations = result
         return writer(destinations) or input
@@ -109,143 +110,215 @@
         if self.compiled:
             logger.warning(
                 "Adding a node to a graph that has already been compiled. This will "
                 "not be reflected in the compiled graph."
             )
         if key in self.nodes:
             raise ValueError(f"Node `{key}` already present.")
-        if key == END:
+        if key == END or key == START:
             raise ValueError(f"Node `{key}` is reserved.")
 
-        self.nodes[key] = coerce_to_runnable(action)
+        self.nodes[key] = coerce_to_runnable(action, name=key, trace=False)
 
     def add_edge(self, start_key: str, end_key: str) -> None:
         if self.compiled:
             logger.warning(
                 "Adding an edge to a graph that has already been compiled. This will "
                 "not be reflected in the compiled graph."
             )
         if start_key == END:
             raise ValueError("END cannot be a start node")
         if end_key == START:
             raise ValueError("START cannot be an end node")
-        if start_key not in self.nodes and start_key != START:
-            raise ValueError(f"Need to add_node `{start_key}` first")
-        if end_key not in self.nodes and end_key != END:
-            raise ValueError(f"Need to add_node `{end_key}` first")
-
         if not self.support_multiple_edges and start_key in set(
             start for start, _ in self.edges
         ):
             raise ValueError(
                 f"Already found path for node '{start_key}'.\n"
                 "For multiple edges, use StateGraph with an annotated state key."
             )
 
         self.edges.add((start_key, end_key))
 
     def add_conditional_edges(
         self,
-        start_key: str,
-        condition: Union[
+        source: str,
+        path: Union[
             Callable[..., Union[str, list[str]]],
             Callable[..., Awaitable[Union[str, list[str]]]],
             Runnable[Any, Union[str, list[str]]],
         ],
-        conditional_edge_mapping: Optional[dict[str, str]] = None,
+        path_map: Optional[Union[dict[str, str], list[str]]] = None,
+        then: Optional[str] = None,
     ) -> None:
+        """Add a conditional edge from the starting node to any number of destination nodes.
+
+        Args:
+            source (str): The starting node. This conditional edge will run when
+                exiting this node.
+            path (Union[Callable, Runnable]): The callable that determines the next
+                node or nodes. If not specifying `path_map` it should return one or
+                more nodes. If it returns END, the graph will stop execution.
+            path_map (Optional[dict[str, str]]): Optional mapping of paths to node
+                names. If ommitted the paths returned by `path` should be node names.
+            then (Optional[str]): The name of a node to execute after the nodes
+                selected by `path`.
+
+        Returns:
+            None
+        """  # noqa: E501
         if self.compiled:
             logger.warning(
                 "Adding an edge to a graph that has already been compiled. This will "
                 "not be reflected in the compiled graph."
             )
+        # coerce path_map to a dictionary
+        if isinstance(path_map, dict):
+            pass
+        elif isinstance(path_map, list):
+            path_map = {name: name for name in path_map}
+        elif rtn_type := get_type_hints(path).get("return"):
+            if get_origin(rtn_type) is Literal:
+                path_map = {name: name for name in get_args(rtn_type)}
         # find a name for the condition
-        condition = coerce_to_runnable(condition)
-        name = condition.name or "condition"
+        path = coerce_to_runnable(path, name=None, trace=True)
+        name = path.name or "condition"
         # validate the condition
-        if start_key not in self.nodes and start_key != START:
-            raise ValueError(f"Need to add_node `{start_key}` first")
-        if conditional_edge_mapping and set(
-            conditional_edge_mapping.values()
-        ).difference([END]).difference(self.nodes):
-            raise ValueError(
-                f"Missing nodes which are in conditional edge mapping. Mapping "
-                f"contains possible destinations: "
-                f"{list(conditional_edge_mapping.values())}. Possible nodes are "
-                f"{list(self.nodes.keys())}."
-            )
-        if name in self.branches[start_key]:
+        if name in self.branches[source]:
             raise ValueError(
-                f"Branch with name `{condition.name}` already exists for node "
-                f"`{start_key}`"
+                f"Branch with name `{path.name}` already exists for node " f"`{source}`"
             )
         # save it
-        self.branches[start_key][name] = Branch(condition, conditional_edge_mapping)
+        self.branches[source][name] = Branch(path, path_map, then)
 
     def set_entry_point(self, key: str) -> None:
+        """Specifies the first node to be called in the graph.
+
+        Parameters:
+            key (str): The key of the node to set as the entry point.
+
+        Returns:
+            None
+        """
         return self.add_edge(START, key)
 
     def set_conditional_entry_point(
         self,
-        condition: Union[
+        path: Union[
             Callable[..., str], Callable[..., Awaitable[str]], Runnable[Any, str]
         ],
-        conditional_edge_mapping: Optional[Dict[str, str]] = None,
+        path_map: Optional[Dict[str, str]] = None,
+        then: Optional[str] = None,
     ) -> None:
-        return self.add_conditional_edges(START, condition, conditional_edge_mapping)
+        """Sets a conditional entry point in the graph.
+
+        Args:
+            path (Union[Callable, Runnable]): The callable that determines the next
+                node or nodes. If not specifying `path_map` it should return one or
+                more nodes. If it returns END, the graph will stop execution.
+            path_map (Optional[dict[str, str]]): Optional mapping of paths to node
+                names. If ommitted the paths returned by `path` should be node names.
+            then (Optional[str]): The name of a node to execute after the nodes
+                selected by `path`.
+
+        Returns:
+            None
+        """
+        return self.add_conditional_edges(START, path, path_map, then)
 
     def set_finish_point(self, key: str) -> None:
+        """Marks a node as a finish point of the graph.
+
+        If the graph reaches this node, it will cease execution.
+
+        Parameters:
+            key (str): The key of the node to set as the finish point.
+
+        Returns:
+            None
+        """
         return self.add_edge(key, END)
 
     def validate(self, interrupt: Optional[Sequence[str]] = None) -> None:
-        all_starts = {src for src, _ in self._all_edges} | {
-            src for src in self.branches
-        }
+        # assemble sources
+        all_sources = {src for src, _ in self._all_edges}
+        for start, branches in self.branches.items():
+            for cond, branch in branches.items():
+                all_sources.add(start)
+                if branch.then is not None:
+                    if branch.ends is not None:
+                        for end in branch.ends.values():
+                            all_sources.add(end)
+                    else:
+                        for node in self.nodes:
+                            if node != start and node != branch.then:
+                                all_sources.add(node)
+        # validate sources
         for node in self.nodes:
-            if node not in all_starts:
-                raise ValueError(f"Node `{node}` is a dead-end")
-
-        all_branches = [
-            branch
-            for branches in self.branches.values()
-            for branch in branches.values()
-        ]
-        if all(branch.ends is not None for branch in all_branches):
-            all_ends = {end for _, end in self._all_edges} | {
-                end for branch in all_branches for end in branch.ends.values()
-            }
-
-            for node in self.nodes:
-                if node not in all_ends:
-                    raise ValueError(f"Node `{node}` is not reachable")
+            if node not in all_sources:
+                raise ValueError(f"Node '{node}' is a dead-end")
+        for source in all_sources:
+            if node not in self.nodes and node != START:
+                raise ValueError(f"Found edge starting at unkown node '{source}'")
 
+        # assemble targets
+        all_targets = {end for _, end in self._all_edges}
+        for start, branches in self.branches.items():
+            for cond, branch in branches.items():
+                if branch.then is not None:
+                    all_targets.add(branch.then)
+                if branch.ends is not None:
+                    for end in branch.ends.values():
+                        if end not in self.nodes and end != END:
+                            raise ValueError(
+                                f"At '{start}' node, '{cond}' branch found unknown target '{end}'"
+                            )
+                        all_targets.add(end)
+                else:
+                    all_targets.add(END)
+                    for node in self.nodes:
+                        if node != start and node != branch.then:
+                            all_targets.add(node)
+        # validate targets
+        for node in self.nodes:
+            if node not in all_targets:
+                raise ValueError(f"Node `{node}` is not reachable")
+        for target in all_targets:
+            if target not in self.nodes and target != END:
+                raise ValueError(f"Found edge ending at unknown node `{target}`")
+        # validate interrupts
         if interrupt:
             for node in interrupt:
                 if node not in self.nodes:
-                    raise ValueError(f"Node `{node}` is not present")
+                    raise ValueError(f"Interrupt node `{node}` not found")
 
         self.compiled = True
 
     def compile(
         self,
         checkpointer: Optional[BaseCheckpointSaver] = None,
-        interrupt_before: Optional[Sequence[str]] = None,
-        interrupt_after: Optional[Sequence[str]] = None,
+        interrupt_before: Optional[Union[All, Sequence[str]]] = None,
+        interrupt_after: Optional[Union[All, Sequence[str]]] = None,
         debug: bool = False,
     ) -> "CompiledGraph":
         # assign default values
         interrupt_before = interrupt_before or []
         interrupt_after = interrupt_after or []
 
         # validate the graph
-        self.validate(interrupt=interrupt_before + interrupt_after)
+        self.validate(
+            interrupt=(interrupt_before if interrupt_before != "*" else [])
+            + interrupt_after
+            if interrupt_after != "*"
+            else []
+        )
 
         # create empty compiled graph
         compiled = CompiledGraph(
-            graph=self,
+            builder=self,
             nodes={},
             channels={START: EphemeralValue(Any), END: EphemeralValue(Any)},
             input_channels=START,
             output_channels=END,
             stream_mode="values",
             stream_channels=[],
             checkpointer=checkpointer,
@@ -267,15 +340,15 @@
                 compiled.attach_branch(start, name, branch)
 
         # validate the compiled graph
         return compiled.validate()
 
 
 class CompiledGraph(Pregel):
-    graph: Graph
+    builder: Graph
 
     def attach_node(self, key: str, node: Runnable) -> None:
         self.channels[key] = EphemeralValue(Any)
         self.nodes[key] = (
             PregelNode(channels=[], triggers=[])
             | node
             | ChannelWrite([ChannelWriteEntry(key)], tags=[TAG_HIDDEN])
@@ -315,53 +388,70 @@
             if end != END:
                 channel_name = f"branch:{start}:{name}:{end}"
                 self.channels[channel_name] = EphemeralValue(Any)
                 self.nodes[end].triggers.append(channel_name)
                 self.nodes[end].channels.append(channel_name)
 
     def get_graph(
-        self, config: Optional[RunnableConfig] = None, *, xray: bool = False
-    ) -> RunnableGraph:
+        self,
+        config: Optional[RunnableConfig] = None,
+        *,
+        xray: Union[int, bool] = False,
+    ) -> DrawableGraph:
         """Returns a drawable representation of the computation graph."""
-        graph = RunnableGraph()
+        graph = DrawableGraph()
         start_nodes: dict[str, RunnableGraphNode] = {
             START: graph.add_node(self.get_input_schema(config), START)
         }
         end_nodes: dict[str, RunnableGraphNode] = {
             END: graph.add_node(self.get_output_schema(config), END)
         }
 
-        for key, node in self.graph.nodes.items():
+        for key, node in self.builder.nodes.items():
             if xray:
                 subgraph = (
-                    node.get_graph(config=config, xray=xray)
+                    node.get_graph(
+                        config=config,
+                        xray=xray - 1 if isinstance(xray, int) and xray > 0 else xray,
+                    )
                     if isinstance(node, CompiledGraph)
                     else node.get_graph(config=config)
                 )
                 subgraph.trim_first_node()
                 subgraph.trim_last_node()
                 if len(subgraph.nodes) > 1:
-                    graph.extend(subgraph)
-                    start_nodes[key] = subgraph.last_node()
-                    end_nodes[key] = subgraph.first_node()
+                    end_nodes[key], start_nodes[key] = graph.extend(
+                        subgraph, prefix=key
+                    )
                 else:
                     n = graph.add_node(node, key)
                     start_nodes[key] = n
                     end_nodes[key] = n
             else:
                 n = graph.add_node(node, key)
                 start_nodes[key] = n
                 end_nodes[key] = n
-        for start, end in sorted(self.graph._all_edges):
+        for start, end in sorted(self.builder._all_edges):
             graph.add_edge(start_nodes[start], end_nodes[end])
-        for start, branches in self.graph.branches.items():
-            for name, branch in branches.items():
-                cond = graph.add_node(branch.condition, name)
-                graph.add_edge(start_nodes[start], cond)
-                ends = branch.ends or {
-                    **{k: k for k in self.graph.nodes},
-                    END: END,
-                }
+        for start, branches in self.builder.branches.items():
+            default_ends = {
+                **{k: k for k in self.builder.nodes if k != start},
+                END: END,
+            }
+            for _, branch in branches.items():
+                if branch.ends is not None:
+                    ends = branch.ends
+                elif branch.then is not None:
+                    ends = {k: k for k in default_ends if k not in (END, branch.then)}
+                else:
+                    ends = default_ends
                 for label, end in ends.items():
-                    graph.add_edge(cond, end_nodes[end], label)
+                    graph.add_edge(
+                        start_nodes[start],
+                        end_nodes[end],
+                        label if label != end else None,
+                        conditional=True,
+                    )
+                    if branch.then is not None:
+                        graph.add_edge(start_nodes[end], end_nodes[branch.then])
 
         return graph
```

### Comparing `gigagraph-0.0.37/langgraph/graph/state.py` & `gigagraph-0.0.45/langgraph/graph/state.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import logging
 from functools import partial
 from inspect import signature
-from typing import Any, Optional, Sequence, Type, Union
+from typing import Any, Optional, Sequence, Type, Union, get_type_hints
 
+from langchain_core.pydantic_v1 import BaseModel
 from langchain_core.runnables import Runnable, RunnableConfig
 from langchain_core.runnables.base import RunnableLike
 
 from langgraph.channels.base import BaseChannel, InvalidUpdateError
 from langgraph.channels.binop import BinaryOperatorAggregate
+from langgraph.channels.dynamic_barrier_value import DynamicBarrierValue, WaitForNames
 from langgraph.channels.ephemeral_value import EphemeralValue
 from langgraph.channels.last_value import LastValue
 from langgraph.channels.named_barrier_value import NamedBarrierValue
 from langgraph.checkpoint import BaseCheckpointSaver
 from langgraph.constants import TAG_HIDDEN
 from langgraph.graph.graph import END, START, Branch, CompiledGraph, Graph
 from langgraph.pregel.read import ChannelRead, PregelNode
+from langgraph.pregel.types import All
 from langgraph.pregel.write import SKIP_WRITE, ChannelWrite, ChannelWriteEntry
 from langgraph.utils import RunnableCallable
 
 logger = logging.getLogger(__name__)
 
 
 class StateGraph(Graph):
@@ -26,34 +29,63 @@
     The signature of each node is State -> Partial<State>.
 
     Each state key can optionally be annotated with a reducer function that
     will be used to aggregate the values of that key received from multiple nodes.
     The signature of a reducer function is (Value, Value) -> Value.
     """
 
-    def __init__(self, schema: Type[Any]) -> None:
+    def __init__(
+        self, state_schema: Type[Any], config_schema: Optional[Type[Any]] = None
+    ) -> None:
         super().__init__()
-        self.schema = schema
-        self.channels = _get_channels(schema)
+        self.schema = state_schema
+        self.config_schema = config_schema
+        self.channels = _get_channels(state_schema)
         if any(isinstance(c, BinaryOperatorAggregate) for c in self.channels.values()):
             self.support_multiple_edges = True
         self.waiting_edges: set[tuple[tuple[str, ...], str]] = set()
 
     @property
     def _all_edges(self) -> set[tuple[str, str]]:
         return self.edges | {
             (start, end) for starts, end in self.waiting_edges for start in starts
         }
 
     def add_node(self, key: str, action: RunnableLike) -> None:
+        """Adds a new node to the state graph.
+
+        Args:
+            key (str): The key of the node.
+            action (RunnableLike): The action associated with the node.
+
+        Raises:
+            ValueError: If the key is already being used as a state key.
+
+        Returns:
+            None
+        """
         if key in self.channels:
             raise ValueError(f"'{key}' is already being used as a state key")
         return super().add_node(key, action)
 
     def add_edge(self, start_key: Union[str, list[str]], end_key: str) -> None:
+        """Adds a directed edge from the start node to the end node.
+
+        If the graph transitions to the start_key node, it will always transition to the end_key node next.
+
+        Args:
+            start_key (Union[str, list[str]]): The key(s) of the start node(s) of the edge.
+            end_key (str): The key of the end node of the edge.
+
+        Raises:
+            ValueError: If the start key is 'END' or if the start key or end key is not present in the graph.
+
+        Returns:
+            None
+        """
         if isinstance(start_key, str):
             return super().add_edge(start_key, end_key)
 
         if self.compiled:
             logger.warning(
                 "Adding an edge to a graph that has already been compiled. This will "
                 "not be reflected in the compiled graph."
@@ -69,31 +101,53 @@
             raise ValueError(f"Need to add_node `{end_key}` first")
 
         self.waiting_edges.add((tuple(start_key), end_key))
 
     def compile(
         self,
         checkpointer: Optional[BaseCheckpointSaver] = None,
-        interrupt_before: Optional[Sequence[str]] = None,
-        interrupt_after: Optional[Sequence[str]] = None,
+        interrupt_before: Optional[Union[All, Sequence[str]]] = None,
+        interrupt_after: Optional[Union[All, Sequence[str]]] = None,
         debug: bool = False,
     ) -> CompiledGraph:
+        """Compiles the state graph into a `CompiledGraph` object.
+
+        The compiled graph implements the `Runnable` interface and can be invoked,
+        streamed, batched, and run asynchronously.
+
+        Args:
+            checkpointer (Optional[BaseCheckpointSaver]): An optional checkpoint saver object.
+                This serves as a fully versioned "memory" for the graph, allowing
+                the graph to be paused and resumed, and replayed from any point.
+            interrupt_before (Optional[Sequence[str]]): An optional list of node names to interrupt before.
+            interrupt_after (Optional[Sequence[str]]): An optional list of node names to interrupt after.
+            debug (bool): A flag indicating whether to enable debug mode.
+
+        Returns:
+            CompiledGraph: The compiled state graph.
+        """
         # assign default values
         interrupt_before = interrupt_before or []
         interrupt_after = interrupt_after or []
 
         # validate the graph
-        self.validate(interrupt=interrupt_before + interrupt_after)
+        self.validate(
+            interrupt=(interrupt_before if interrupt_before != "*" else [])
+            + interrupt_after
+            if interrupt_after != "*"
+            else []
+        )
 
         # prepare output channels
         state_keys = list(self.channels)
         output_channels = state_keys[0] if state_keys == ["__root__"] else state_keys
 
         compiled = CompiledStateGraph(
-            graph=self,
+            builder=self,
+            config_type=self.config_schema,
             nodes={},
             channels={**self.channels, START: EphemeralValue(self.schema)},
             input_channels=START,
             stream_mode="updates",
             output_channels=output_channels,
             stream_channels=output_channels,
             checkpointer=checkpointer,
@@ -117,32 +171,51 @@
             for name, branch in branches.items():
                 compiled.attach_branch(start, name, branch)
 
         return compiled.validate()
 
 
 class CompiledStateGraph(CompiledGraph):
-    graph: StateGraph
+    builder: StateGraph
+
+    def get_input_schema(
+        self, config: Optional[RunnableConfig] = None
+    ) -> type[BaseModel]:
+        if isinstance(self.builder.schema, BaseModel):
+            return self.builder.schema
+
+        return super().get_input_schema(config)
+
+    def get_output_schema(self, config: Optional[RunnableConfig] = None) -> BaseModel:
+        if isinstance(self.builder.schema, BaseModel):
+            return self.builder.schema
+
+        return super().get_output_schema(config)
 
     def attach_node(self, key: str, node: Optional[Runnable]) -> None:
         def _get_state_key(input: dict, config: RunnableConfig, *, key: str) -> Any:
             if input is None:
                 return SKIP_WRITE
             elif not isinstance(input, dict):
                 raise InvalidUpdateError(f"Expected dict, got {input}")
             else:
                 return input.get(key, SKIP_WRITE)
 
-        state_keys = list(self.graph.channels)
+        state_keys = list(self.builder.channels)
         # state updaters
         state_write_entries = [
-            ChannelWriteEntry(key, None, skip_none=True)
-            if key == "__root__"
-            else ChannelWriteEntry(
-                key, RunnableCallable(_get_state_key, key=key, trace=False)
+            (
+                ChannelWriteEntry(key, skip_none=True)
+                if key == "__root__"
+                else ChannelWriteEntry(
+                    key,
+                    mapper=RunnableCallable(
+                        _get_state_key, key=key, trace=False, recurse=False
+                    ),
+                )
             )
             for key in state_keys
         ]
 
         # add node and output channel
         if key == START:
             self.nodes[key] = PregelNode(
@@ -163,20 +236,20 @@
                     if state_keys == ["__root__"]
                     else {chan: chan for chan in state_keys}
                 ),
                 # coerce state dict to schema class (eg. pydantic model)
                 mapper=(
                     None
                     if state_keys == ["__root__"]
-                    else partial(_coerce_state, self.graph.schema)
+                    else partial(_coerce_state, self.builder.schema)
                 ),
                 writers=[
                     # publish to this channel and state keys
                     ChannelWrite(
-                        [ChannelWriteEntry(key)] + state_write_entries,
+                        [ChannelWriteEntry(key, key)] + state_write_entries,
                         tags=[TAG_HIDDEN],
                     ),
                 ],
             ).pipe(node)
 
     def attach_edge(self, starts: Union[str, Sequence[str]], end: str) -> None:
         if isinstance(starts, str):
@@ -204,33 +277,53 @@
                 self.nodes[start] |= ChannelWrite(
                     [ChannelWriteEntry(channel_name, start)], tags=[TAG_HIDDEN]
                 )
 
     def attach_branch(self, start: str, name: str, branch: Branch) -> None:
         def branch_writer(ends: list[str]) -> Optional[ChannelWrite]:
             if filtered_ends := [end for end in ends if end != END]:
-                return ChannelWrite(
-                    [
-                        ChannelWriteEntry(f"branch:{start}:{name}:{end}", start)
-                        for end in filtered_ends
-                    ],
-                    tags=[TAG_HIDDEN],
-                )
+                writes = [
+                    ChannelWriteEntry(f"branch:{start}:{name}:{end}", start)
+                    for end in filtered_ends
+                ]
+                if branch.then and branch.then != END:
+                    writes.append(
+                        ChannelWriteEntry(
+                            f"branch:{start}:{name}:then",
+                            WaitForNames(set(filtered_ends)),
+                        )
+                    )
+                return ChannelWrite(writes, tags=[TAG_HIDDEN])
 
         # attach branch publisher
-        self.nodes[start] |= branch.run(branch_writer, _get_state_reader(self.graph))
+        self.nodes[start] |= branch.run(branch_writer, _get_state_reader(self.builder))
 
         # attach branch subscribers
-        ends = branch.ends.values() if branch.ends else [node for node in self.nodes]
+        ends = (
+            branch.ends.values()
+            if branch.ends
+            else [node for node in self.builder.nodes if node != branch.then]
+        )
         for end in ends:
             if end != END:
                 channel_name = f"branch:{start}:{name}:{end}"
                 self.channels[channel_name] = EphemeralValue(Any)
                 self.nodes[end].triggers.append(channel_name)
 
+        # attach then subscriber
+        if branch.then and branch.then != END:
+            channel_name = f"branch:{start}:{name}:then"
+            self.channels[channel_name] = DynamicBarrierValue(str)
+            self.nodes[branch.then].triggers.append(channel_name)
+            for end in ends:
+                if end != END:
+                    self.nodes[end] |= ChannelWrite(
+                        [ChannelWriteEntry(channel_name, end)], tags=[TAG_HIDDEN]
+                    )
+
 
 def _get_state_reader(graph: StateGraph) -> ChannelRead:
     state_keys = list(graph.channels)
     return partial(
         ChannelRead.do_read,
         channel=state_keys[0] if state_keys == ["__root__"] else state_keys,
         fresh=True,
@@ -243,26 +336,24 @@
 
 def _coerce_state(schema: Type[Any], input: dict[str, Any]) -> dict[str, Any]:
     return schema(**input)
 
 
 def _get_channels(schema: Type[dict]) -> dict[str, BaseChannel]:
     if not hasattr(schema, "__annotations__"):
-        return {
-            "__root__": _get_channel(schema),
-        }
-
-    channels: dict[str, BaseChannel] = {}
-    for name, typ in schema.__annotations__.items():
-        channels[name] = _get_channel(typ)
+        return {"__root__": _get_channel(schema)}
 
-    return channels
+    return {
+        name: _get_channel(typ)
+        for name, typ in get_type_hints(schema, include_extras=True).items()
+        if name != "__slots__"
+    }
 
 
-def _get_channel(annotation: Any) -> Optional[BaseChannel]:
+def _get_channel(annotation: Any) -> BaseChannel:
     if channel := _is_field_binop(annotation):
         return channel
     return LastValue(annotation)
 
 
 def _is_field_binop(typ: Type[Any]) -> Optional[BinaryOperatorAggregate]:
     if hasattr(typ, "__metadata__"):
```

### Comparing `gigagraph-0.0.37/langgraph/prebuilt/agent_executor.py` & `gigagraph-0.0.45/langgraph/prebuilt/agent_executor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import operator
 from typing import Annotated, Sequence, TypedDict, Union
 
 from langchain_core.agents import AgentAction, AgentFinish
 from langchain_core.messages import BaseMessage
 
+from langgraph._api.deprecation import deprecated
 from langgraph.graph import END, StateGraph
+from langgraph.graph.state import CompiledStateGraph
 from langgraph.prebuilt.tool_executor import ToolExecutor
 from langgraph.utils import RunnableCallable
 
 
 def _get_agent_state(input_schema=None):
     if input_schema is None:
 
@@ -35,15 +37,56 @@
             # Here we annotate this with `operator.add` to indicate that operations to
             # this state should be ADDED to the existing values (not overwrite it)
             intermediate_steps: Annotated[list[tuple[AgentAction, str]], operator.add]
 
     return AgentState
 
 
-def create_agent_executor(agent_runnable, tools, input_schema=None):
+@deprecated(
+    "0.0.44",
+    alternative="create_tool_calling_executor",
+    example="""
+from langgraph.prebuilt import chat_agent_executor
+
+chat_agent_executor.create_tool_calling_executor(...)
+""",
+)
+def create_agent_executor(
+    agent_runnable, tools, input_schema=None
+) -> CompiledStateGraph:
+    """This is a helper function for creating a graph that works with LangChain Agents.
+
+    Args:
+        agent_runnable (RunnableLike): The agent runnable.
+        tools (list): A list of tools to be used by the agent.
+        input_schema (dict, optional): The input schema for the agent. Defaults to None.
+
+    Returns:
+        The `CompiledStateGraph` object.
+
+
+    Examples:
+
+        # Since this is deprecated, you should use `create_tool_calling_executor` instead.
+        # Example usage:
+        from langgraph.prebuilt import chat_agent_executor
+        from langchain_openai import ChatOpenAI
+        from langchain_community.tools.tavily_search import TavilySearchResults
+
+        tools = [TavilySearchResults(max_results=1)]
+        model = ChatOpenAI()
+
+        app = chat_agent_executor.create_tool_calling_executor(model, tools)
+
+        inputs = {"messages": [("user", "what is the weather in sf")]}
+        for s in app.stream(inputs):
+            print(list(s.values())[0])
+            print("----")
+    """
+
     if isinstance(tools, ToolExecutor):
         tool_executor = tools
     else:
         tool_executor = ToolExecutor(tools)
 
     state = _get_agent_state(input_schema)
```

### Comparing `gigagraph-0.0.37/langgraph/prebuilt/chat_agent_executor.py` & `gigagraph-0.0.45/langgraph/prebuilt/chat_agent_executor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,59 @@
 import json
-from typing import Annotated, Sequence, TypedDict, Union
+from typing import Annotated, Callable, Optional, Sequence, TypedDict, Union
 
 from langchain_core.language_models import LanguageModelLike
-from langchain_core.messages import BaseMessage, FunctionMessage
-from langchain_core.runnables import RunnableLambda
+from langchain_core.messages import BaseMessage, FunctionMessage, SystemMessage
+from langchain_core.runnables import Runnable, RunnableLambda
 from langchain_core.tools import BaseTool
 from langchain_core.utils.function_calling import convert_to_openai_function
 
+from langgraph._api.deprecation import deprecated
+from langgraph.checkpoint import BaseCheckpointSaver
 from langgraph.graph import END, StateGraph
+from langgraph.graph.graph import CompiledGraph
 from langgraph.graph.message import add_messages
 from langgraph.prebuilt.tool_executor import ToolExecutor, ToolInvocation
 from langgraph.prebuilt.tool_node import ToolNode
 
 
 # We create the AgentState that we will pass around
 # This simply involves a list of messages
 # We want steps to return messages to append to the list
 # So we annotate the messages attribute with operator.add
 class AgentState(TypedDict):
+    """The state of the agent."""
+
     messages: Annotated[Sequence[BaseMessage], add_messages]
 
 
+@deprecated("0.0.44", "create_tool_calling_executor")
 def create_function_calling_executor(
     model: LanguageModelLike, tools: Union[ToolExecutor, Sequence[BaseTool]]
-):
+) -> CompiledGraph:
+    """Creates a graph that works with a chat model that utilizes function calling.
+
+    Examples:
+
+        # Since this is deprecated, you should use `create_tool_calling_executor` instead.
+        # Example usage:
+        from langgraph.prebuilt import chat_agent_executor
+        from langchain_openai import ChatOpenAI
+        from langchain_community.tools.tavily_search import TavilySearchResults
+
+        tools = [TavilySearchResults(max_results=1)]
+        model = ChatOpenAI()
+
+        app = chat_agent_executor.create_tool_calling_executor(model, tools)
+
+        inputs = {"messages": [("user", "what is the weather in sf")]}
+        for s in app.stream(inputs):
+            print(list(s.values())[0])
+            print("----")
+    """
     if isinstance(tools, ToolExecutor):
         tool_executor = tools
         tool_classes = tools.tools
     else:
         tool_executor = ToolExecutor(tools)
         tool_classes = tools
     model = model.bind(functions=[convert_to_openai_function(t) for t in tool_classes])
@@ -131,16 +157,59 @@
     # Finally, we compile it!
     # This compiles it into a LangChain Runnable,
     # meaning you can use it as you would any other runnable
     return workflow.compile()
 
 
 def create_tool_calling_executor(
-    model: LanguageModelLike, tools: Union[ToolExecutor, Sequence[BaseTool]]
-):
+    model: LanguageModelLike,
+    tools: Union[ToolExecutor, Sequence[BaseTool]],
+    messages_modifier: Optional[Union[SystemMessage, str, Callable, Runnable]] = None,
+    checkpointer: Optional[BaseCheckpointSaver] = None,
+    interrupt_before: Optional[Sequence[str]] = None,
+    interrupt_after: Optional[Sequence[str]] = None,
+    debug: bool = False,
+) -> CompiledGraph:
+    """Creates a graph that works with a chat model that utilizes tool calling.
+
+    Args:
+        model (LanguageModelLike): The chat model that supports OpenAI tool calling.
+        tools (Union[ToolExecutor, Sequence[BaseTool]]): A list of tools or a ToolExecutor instance.
+        messages_modifier: (Optional[Union[SystemMessage, str, Callable, Runnable]]): An optional
+            messages modifier. This applies to messages BEFORE they are passed into the LLM.
+            Can take a few different forms:
+            - SystemMessage: this is added to the beginning of the list of messages.
+            - str: This is converted to a SystemMessage and added to the beginning of the list of messages.
+            - Callable: This function should take in a list of messages and the output is then passed to the language model.
+            - Runnable: This runnable should take in a list of messages and the output is then passed to the language model.
+        checkpointer (Optional[BaseCheckpointSaver]): An optional checkpoint saver object.
+        interrupt_before (Optional[Sequence[str]]): An optional list of node names to interrupt before.
+        interrupt_after (Optional[Sequence[str]]): An optional list of node names to interrupt after.
+        debug (bool): A flag indicating whether to enable debug mode.
+
+    Returns:
+        Runnable: A compiled LangChain runnable that can be used for chat interactions.
+
+    Examples:
+
+            from langchain_community.tools.tavily_search import TavilySearchResults
+            from langchain_openai import ChatOpenAI
+
+            from langgraph.prebuilt import chat_agent_executor
+
+            tools = [TavilySearchResults(max_results=1)]
+            model = ChatOpenAI()
+
+            app = chat_agent_executor.create_tool_calling_executor(model, tools)
+
+            inputs = {"messages": [("user", "what is the weather in sf")]}
+            for s in app.stream(inputs):
+                print(list(s.values())[0])
+                print("----")
+    """
     if isinstance(tools, ToolExecutor):
         tool_classes = tools.tools
     else:
         tool_classes = tools
     model = model.bind_tools(tool_classes)
 
     # Define the function that determines whether to continue or not
@@ -150,24 +219,39 @@
         # If there is no function call, then we finish
         if not last_message.tool_calls:
             return "end"
         # Otherwise if there is, we continue
         else:
             return "continue"
 
+    # Add the message modifier, if exists
+    if messages_modifier is None:
+        model_runnable = model
+    elif isinstance(messages_modifier, str):
+        _system_message: BaseMessage = SystemMessage(content=messages_modifier)
+        model_runnable = (lambda messages: [_system_message] + messages) | model
+    elif isinstance(messages_modifier, SystemMessage):
+        model_runnable = (lambda messages: [messages_modifier] + messages) | model
+    elif isinstance(messages_modifier, (Callable, Runnable)):
+        model_runnable = messages_modifier | model
+    else:
+        raise ValueError(
+            f"Got unexpected type for `messages_modifier`: {type(messages_modifier)}"
+        )
+
     # Define the function that calls the model
     def call_model(state: AgentState):
         messages = state["messages"]
-        response = model.invoke(messages)
+        response = model_runnable.invoke(messages)
         # We return a list, because this will get added to the existing list
         return {"messages": [response]}
 
     async def acall_model(state: AgentState):
         messages = state["messages"]
-        response = await model.ainvoke(messages)
+        response = await model_runnable.ainvoke(messages)
         # We return a list, because this will get added to the existing list
         return {"messages": [response]}
 
     # Define a new graph
     workflow = StateGraph(AgentState)
 
     # Define the two nodes we will cycle between
@@ -202,8 +286,13 @@
     # We now add a normal edge from `tools` to `agent`.
     # This means that after `tools` is called, `agent` node is called next.
     workflow.add_edge("action", "agent")
 
     # Finally, we compile it!
     # This compiles it into a LangChain Runnable,
     # meaning you can use it as you would any other runnable
-    return workflow.compile()
+    return workflow.compile(
+        checkpointer=checkpointer,
+        interrupt_before=interrupt_before,
+        interrupt_after=interrupt_after,
+        debug=debug,
+    )
```

### Comparing `gigagraph-0.0.37/langgraph/prebuilt/tool_executor.py` & `gigagraph-0.0.45/langgraph/prebuilt/tool_executor.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,30 +9,79 @@
 INVALID_TOOL_MSG_TEMPLATE = (
     "{requested_tool_name} is not a valid tool, "
     "try one of [{available_tool_names_str}]."
 )
 
 
 class ToolInvocationInterface:
-    """Interface for invoking a tool"""
+    """Interface for invoking a tool.
+
+    Attributes:
+        tool (str): The name of the tool to invoke.
+        tool_input (Union[str, dict]): The input to pass to the tool.
+
+    """
 
     tool: str
     tool_input: Union[str, dict]
 
 
 class ToolInvocation(Serializable):
-    """Information about how to invoke a tool."""
+    """Information about how to invoke a tool.
+
+    Attributes:
+        tool (str): The name of the Tool to execute.
+        tool_input (Union[str, dict]): The input to pass in to the Tool.
+
+    Examples:
+
+            invocation = ToolInvocation(
+                tool="search",
+                tool_input="What is the capital of France?"
+            )
+    """
 
     tool: str
-    """The name of the Tool to execute."""
     tool_input: Union[str, dict]
-    """The input to pass in to the Tool."""
 
 
 class ToolExecutor(RunnableCallable):
+    """Executes a tool invocation.
+
+    Args:
+        tools (Sequence[BaseTool]): A sequence of tools that can be invoked.
+        invalid_tool_msg_template (str, optional): The template for the error message
+            when an invalid tool is requested. Defaults to INVALID_TOOL_MSG_TEMPLATE.
+
+    Examples:
+
+            from langchain_core.tools import tool
+            from langgraph.prebuilt.tool_executor import ToolExecutor, ToolInvocation
+
+
+            @tool
+            def search(query: str) -> str:
+                \"\"\"Search engine.\"\"\"
+                return f"Searching for: {query}"
+
+
+            tools = [search]
+            executor = ToolExecutor(tools)
+
+            invocation = ToolInvocation(tool="search", tool_input="What is the capital of France?")
+            result = executor.invoke(invocation)
+            print(result)  # Output: "Searching for: What is the capital of France?"
+
+            invocation = ToolInvocation(
+                tool="nonexistent", tool_input="What is the capital of France?"
+            )
+            result = executor.invoke(invocation)
+            print(result)  # Output: "nonexistent is not a valid tool, try one of [search]."
+    """
+
     def __init__(
         self,
         tools: Sequence[BaseTool],
         *,
         invalid_tool_msg_template: str = INVALID_TOOL_MSG_TEMPLATE,
     ) -> None:
         super().__init__(self._execute, afunc=self._aexecute, trace=False)
```

### Comparing `gigagraph-0.0.37/langgraph/pregel/__init__.py` & `gigagraph-0.0.45/langgraph/pregel/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     Literal,
     Mapping,
     Optional,
     Sequence,
     Type,
     Union,
     cast,
+    get_type_hints,
     overload,
 )
 
 from langchain_core.globals import get_debug
 from langchain_core.load.dump import dumpd
 from langchain_core.pydantic_v1 import BaseModel, Field, root_validator
 from langchain_core.runnables import (
@@ -50,38 +51,45 @@
     AsyncChannelsManager,
     BaseChannel,
     ChannelsManager,
     EmptyChannelError,
     InvalidUpdateError,
     create_checkpoint,
 )
-from langgraph.channels.last_value import LastValue
 from langgraph.checkpoint.base import (
     BaseCheckpointSaver,
     Checkpoint,
-    CheckpointAt,
     copy_checkpoint,
     empty_checkpoint,
 )
 from langgraph.constants import (
     CONFIG_KEY_READ,
     CONFIG_KEY_SEND,
     INTERRUPT,
+    TAG_HIDDEN,
+)
+from langgraph.pregel.debug import (
+    map_debug_checkpoint,
+    map_debug_task_results,
+    map_debug_tasks,
+    print_step_checkpoint,
+    print_step_tasks,
+    print_step_writes,
 )
-from langgraph.pregel.debug import print_checkpoint, print_step_start
 from langgraph.pregel.io import (
     map_input,
     map_output_updates,
     map_output_values,
     read_channel,
     read_channels,
 )
 from langgraph.pregel.log import logger
 from langgraph.pregel.read import PregelNode
 from langgraph.pregel.types import (
+    All,
     PregelExecutableTask,
     PregelTaskDescription,
     StateSnapshot,
 )
 from langgraph.pregel.validate import validate_graph, validate_keys
 from langgraph.pregel.write import ChannelWrite, ChannelWriteEntry
 
@@ -159,72 +167,78 @@
         *channels: str,
         **kwargs: WriteValue,
     ) -> ChannelWrite:
         """Writes to channels the result of the lambda, or None to skip writing."""
         return ChannelWrite(
             [ChannelWriteEntry(c) for c in channels]
             + [
-                ChannelWriteEntry(k, _coerce_write_value(v), True)
+                ChannelWriteEntry(k, skip_none=True, mapper=coerce_to_runnable(v))
+                if isinstance(v, Runnable) or callable(v)
+                else ChannelWriteEntry(k, value=v)
                 for k, v in kwargs.items()
             ]
         )
 
 
-StreamMode = Literal["values", "updates"]
+StreamMode = Literal["values", "updates", "debug"]
 
 
 class Pregel(
     RunnableSerializable[Union[dict[str, Any], Any], Union[dict[str, Any], Any]]
 ):
     nodes: Mapping[str, PregelNode]
 
     channels: Mapping[str, BaseChannel] = Field(default_factory=dict)
 
-    default_channel_cls: Type[BaseChannel] = Field(default=LastValue)
-
     auto_validate: bool = True
 
     stream_mode: StreamMode = "values"
 
-    output_channels: Union[str, Sequence[str]] = "output"
+    output_channels: Union[str, Sequence[str]]
     """Channels to output, defaults to channel named 'output'."""
 
     stream_channels: Optional[Union[str, Sequence[str]]] = None
     """Channels to stream, defaults to all channels not in reserved channels"""
 
-    interrupt_after_nodes: Sequence[str] = Field(default_factory=list)
+    interrupt_after_nodes: Union[All, Sequence[str]] = Field(default_factory=list)
 
-    interrupt_before_nodes: Sequence[str] = Field(default_factory=list)
+    interrupt_before_nodes: Union[All, Sequence[str]] = Field(default_factory=list)
 
-    input_channels: Union[str, Sequence[str]] = "input"
+    input_channels: Union[str, Sequence[str]]
 
     step_timeout: Optional[float] = None
 
     debug: bool = Field(default_factory=get_debug)
 
     checkpointer: Optional[BaseCheckpointSaver] = None
 
+    config_type: Optional[Type[Any]] = None
+
     name: str = "LangGraph"
 
     class Config:
         arbitrary_types_allowed = True
 
+    @classmethod
+    def is_lc_serializable(cls) -> bool:
+        """Return whether the graph can be serialized by Langchain."""
+        return True
+
     @root_validator(skip_on_failure=True)
     def validate_on_init(cls, values: dict[str, Any]) -> dict[str, Any]:
         if not values["auto_validate"]:
             return values
         validate_graph(
             values["nodes"],
             values["channels"],
             values["input_channels"],
             values["output_channels"],
             values["stream_channels"],
             values["interrupt_after_nodes"],
             values["interrupt_before_nodes"],
-            values["default_channel_cls"],
         )
         if values["interrupt_after_nodes"] or values["interrupt_before_nodes"]:
             if not values["checkpointer"]:
                 raise ValueError("Interrupts require a checkpointer")
         return values
 
     def validate(self) -> Self:
@@ -232,15 +246,14 @@
             self.nodes,
             self.channels,
             self.input_channels,
             self.output_channels,
             self.stream_channels,
             self.interrupt_after_nodes,
             self.interrupt_before_nodes,
-            self.default_channel_cls,
         )
         if self.interrupt_after_nodes or self.interrupt_before_nodes:
             if not self.checkpointer:
                 raise ValueError("Interrupts require a checkpointer")
         return self
 
     @property
@@ -250,14 +263,22 @@
             for spec in get_unique_config_specs(
                 [spec for node in self.nodes.values() for spec in node.config_specs]
                 + (
                     self.checkpointer.config_specs
                     if self.checkpointer is not None
                     else []
                 )
+                + (
+                    [
+                        ConfigurableFieldSpec(id=name, annotation=typ)
+                        for name, typ in get_type_hints(self.config_type).items()
+                    ]
+                    if self.config_type is not None
+                    else []
+                )
             )
             # these are provided by the Pregel class
             if spec.id not in [CONFIG_KEY_READ, CONFIG_KEY_SEND]
         ]
 
     @property
     def InputType(self) -> Any:
@@ -292,97 +313,113 @@
             return create_model(  # type: ignore[call-overload]
                 self.get_name("Output"),
                 **{k: (self.channels[k].ValueType, None) for k in self.output_channels},
             )
 
     @property
     def stream_channels_list(self) -> Sequence[str]:
+        stream_channels = self.stream_channels_asis
         return (
-            [self.stream_channels]
-            if isinstance(self.stream_channels, str)
-            else self.stream_channels or [k for k in self.channels]
+            [stream_channels] if isinstance(stream_channels, str) else stream_channels
         )
 
+    @property
+    def stream_channels_asis(self) -> Union[str, Sequence[str]]:
+        return self.stream_channels or [k for k in self.channels]
+
     def get_state(self, config: RunnableConfig) -> StateSnapshot:
+        """Get the current state of the graph."""
         if not self.checkpointer:
             raise ValueError("No checkpointer set")
 
         saved = self.checkpointer.get_tuple(config)
         checkpoint = saved.checkpoint if saved else empty_checkpoint()
-        config = saved.config if saved else config
         with ChannelsManager(self.channels, checkpoint) as channels:
             _, next_tasks = _prepare_next_tasks(
                 checkpoint, self.nodes, channels, for_execution=False
             )
-            values = read_channels(channels, self.stream_channels_list)
             return StateSnapshot(
-                values[self.stream_channels]
-                if isinstance(self.stream_channels, str)
-                else values,
+                read_channels(channels, self.stream_channels_asis),
                 tuple(name for name, _ in next_tasks),
-                config,
+                saved.config if saved else config,
+                saved.metadata if saved else None,
+                saved.parent_config if saved else None,
             )
 
     async def aget_state(self, config: RunnableConfig) -> StateSnapshot:
+        """Get the current state of the graph."""
         if not self.checkpointer:
             raise ValueError("No checkpointer set")
 
         saved = await self.checkpointer.aget_tuple(config)
         checkpoint = saved.checkpoint if saved else empty_checkpoint()
-        config = saved.config if saved else config
         async with AsyncChannelsManager(self.channels, checkpoint) as channels:
             _, next_tasks = _prepare_next_tasks(
                 checkpoint, self.nodes, channels, for_execution=False
             )
-            values = read_channels(channels, self.stream_channels_list)
             return StateSnapshot(
-                values[self.stream_channels]
-                if isinstance(self.stream_channels, str)
-                else values,
+                read_channels(channels, self.stream_channels_asis),
                 tuple(name for name, _ in next_tasks),
-                config,
+                saved.config if saved else config,
+                saved.metadata if saved else None,
+                saved.parent_config if saved else None,
             )
 
-    def get_state_history(self, config: RunnableConfig) -> Iterator[StateSnapshot]:
+    def get_state_history(
+        self,
+        config: RunnableConfig,
+        *,
+        before: Optional[RunnableConfig] = None,
+        limit: Optional[int] = None,
+    ) -> Iterator[StateSnapshot]:
+        """Get the history of the state of the graph."""
         if not self.checkpointer:
             raise ValueError("No checkpointer set")
 
-        for config, checkpoint, parent_config in self.checkpointer.list(config):
+        for config, checkpoint, metadata, parent_config in self.checkpointer.list(
+            config, before=before, limit=limit
+        ):
             with ChannelsManager(self.channels, checkpoint) as channels:
                 _, next_tasks = _prepare_next_tasks(
                     checkpoint, self.nodes, channels, for_execution=False
                 )
-                values = read_channels(channels, self.stream_channels_list)
                 yield StateSnapshot(
-                    values[self.stream_channels]
-                    if isinstance(self.stream_channels, str)
-                    else values,
+                    read_channels(channels, self.stream_channels_asis),
                     tuple(name for name, _ in next_tasks),
                     config,
+                    metadata,
                     parent_config,
                 )
 
     async def aget_state_history(
-        self, config: RunnableConfig
+        self,
+        config: RunnableConfig,
+        *,
+        before: Optional[RunnableConfig] = None,
+        limit: Optional[int] = None,
     ) -> AsyncIterator[StateSnapshot]:
+        """Get the history of the state of the graph."""
         if not self.checkpointer:
             raise ValueError("No checkpointer set")
 
-        async for config, checkpoint, parent_config in self.checkpointer.alist(config):
+        async for (
+            config,
+            checkpoint,
+            metadata,
+            parent_config,
+        ) in self.checkpointer.alist(config, before=before, limit=limit):
             async with AsyncChannelsManager(self.channels, checkpoint) as channels:
                 _, next_tasks = _prepare_next_tasks(
                     checkpoint, self.nodes, channels, for_execution=False
                 )
-                values = read_channels(channels, self.stream_channels_list)
                 yield StateSnapshot(
-                    values[self.stream_channels]
-                    if isinstance(self.stream_channels, str)
-                    else values,
+                    read_channels(channels, self.stream_channels_asis),
                     tuple(name for name, _ in next_tasks),
                     config,
+                    metadata,
                     parent_config,
                 )
 
     def update_state(
         self,
         config: RunnableConfig,
         values: dict[str, Any] | Any,
@@ -392,16 +429,16 @@
         node `as_node`. If `as_node` is not provided, it will be set to the last node
         that updated the state, if not ambiguous.
         """
         if not self.checkpointer:
             raise ValueError("No checkpointer set")
 
         # get last checkpoint
-        checkpoint = self.checkpointer.get(config)
-        checkpoint = copy_checkpoint(checkpoint) if checkpoint else empty_checkpoint()
+        saved = self.checkpointer.get_tuple(config)
+        checkpoint = copy_checkpoint(saved.checkpoint) if saved else empty_checkpoint()
         # find last node that updated the state, if not provided
         if as_node is None:
             last_seen_by_node = sorted(
                 (v, n)
                 for n, seen in checkpoint["versions_seen"].items()
                 for v in seen.values()
             )
@@ -420,14 +457,16 @@
             if not writers:
                 raise InvalidUpdateError(f"Node {as_node} has no writers")
             task = PregelExecutableTask(
                 as_node,
                 values,
                 RunnableSequence(*writers) if len(writers) > 1 else writers[0],
                 deque(),
+                None,
+                [INTERRUPT],
             )
             # execute task
             task.proc.invoke(
                 task.input,
                 patch_config(
                     config,
                     run_name=self.name + "UpdateState",
@@ -439,29 +478,36 @@
                         ),
                     },
                 ),
             )
             # apply to checkpoint and save
             _apply_writes(checkpoint, channels, task.writes)
             return self.checkpointer.put(
-                config, create_checkpoint(checkpoint, channels)
+                saved.config if saved else config,
+                create_checkpoint(checkpoint, channels),
+                {
+                    "source": "update",
+                    "step": saved.metadata.get("step", 0) + 1
+                    if saved.metadata
+                    else None,
+                },
             )
 
     async def aupdate_state(
         self,
         config: RunnableConfig,
         values: dict[str, Any] | Any,
         as_node: Optional[str] = None,
     ) -> RunnableConfig:
         if not self.checkpointer:
             raise ValueError("No checkpointer set")
 
         # get last checkpoint
-        checkpoint = await self.checkpointer.aget(config)
-        checkpoint = copy_checkpoint(checkpoint) if checkpoint else empty_checkpoint()
+        saved = await self.checkpointer.aget_tuple(config)
+        checkpoint = copy_checkpoint(saved.checkpoint) if saved else empty_checkpoint()
         # find last node that updated the state, if not provided
         if as_node is None:
             last_seen_by_node = sorted(
                 (v, n)
                 for n, seen in checkpoint["versions_seen"].items()
                 for v in seen.values()
             )
@@ -480,14 +526,16 @@
             if not writers:
                 raise InvalidUpdateError(f"Node {as_node} has no writers")
             task = PregelExecutableTask(
                 as_node,
                 values,
                 RunnableSequence(*writers) if len(writers) > 1 else writers[0],
                 deque(),
+                None,
+                [INTERRUPT],
             )
             # execute task
             await task.proc.ainvoke(
                 task.input,
                 patch_config(
                     config,
                     run_name=self.name + "UpdateState",
@@ -499,128 +547,165 @@
                         ),
                     },
                 ),
             )
             # apply to checkpoint and save
             _apply_writes(checkpoint, channels, task.writes)
             return await self.checkpointer.aput(
-                config, create_checkpoint(checkpoint, channels)
+                saved.config if saved else config,
+                create_checkpoint(checkpoint, channels),
+                {
+                    "source": "update",
+                    "step": saved.metadata.get("step", 0) + 1 if saved else None,
+                },
             )
 
     def _defaults(
         self,
+        config: Optional[RunnableConfig] = None,
         *,
         stream_mode: Optional[StreamMode] = None,
         input_keys: Optional[Union[str, Sequence[str]]] = None,
         output_keys: Optional[Union[str, Sequence[str]]] = None,
-        interrupt_before_nodes: Optional[Sequence[str]] = None,
-        interrupt_after_nodes: Optional[Sequence[str]] = None,
+        interrupt_before: Optional[Union[All, Sequence[str]]] = None,
+        interrupt_after: Optional[Union[All, Sequence[str]]] = None,
         debug: Optional[bool] = None,
     ) -> tuple[
         bool,
         StreamMode,
         Union[str, Sequence[str]],
         Union[str, Sequence[str]],
         Optional[Sequence[str]],
         Optional[Sequence[str]],
     ]:
         debug = debug if debug is not None else self.debug
         if output_keys is None:
-            output_keys = (
-                [chan for chan in self.channels]
-                if self.stream_channels is None
-                else self.stream_channels
-            )
+            output_keys = self.stream_channels_asis
         else:
             validate_keys(output_keys, self.channels)
         if input_keys is None:
             input_keys = self.input_channels
         else:
             validate_keys(input_keys, self.channels)
-        interrupt_before_nodes = interrupt_before_nodes or self.interrupt_before_nodes
-        interrupt_after_nodes = interrupt_after_nodes or self.interrupt_after_nodes
+        interrupt_before = interrupt_before or self.interrupt_before_nodes
+        interrupt_after = interrupt_after or self.interrupt_after_nodes
+        stream_mode = stream_mode if stream_mode is not None else self.stream_mode
+        if config is not None and config.get("configurable", {}).get(CONFIG_KEY_READ):
+            # if being called as a node in another graph, always use values mode
+            stream_mode = "values"
         return (
             debug,
-            stream_mode if stream_mode is not None else self.stream_mode,
+            stream_mode,
             input_keys,
             output_keys,
-            interrupt_before_nodes,
-            interrupt_after_nodes,
+            interrupt_before,
+            interrupt_after,
         )
 
     def stream(
         self,
         input: Union[dict[str, Any], Any],
         config: Optional[RunnableConfig] = None,
         *,
         stream_mode: Optional[StreamMode] = None,
         output_keys: Optional[Union[str, Sequence[str]]] = None,
         input_keys: Optional[Union[str, Sequence[str]]] = None,
-        interrupt_before_nodes: Optional[Sequence[str]] = None,
-        interrupt_after_nodes: Optional[Sequence[str]] = None,
+        interrupt_before: Optional[Union[All, Sequence[str]]] = None,
+        interrupt_after: Optional[Union[All, Sequence[str]]] = None,
         debug: Optional[bool] = None,
     ) -> Iterator[Union[dict[str, Any], Any]]:
+        """Stream graph steps for a single input."""
         config = ensure_config(config)
         callback_manager = get_callback_manager_for_config(config)
         run_manager = callback_manager.on_chain_start(
-            dumpd(self), input, name=config.get("run_name", self.get_name())
+            dumpd(self),
+            input,
+            name=config.get("run_name", self.get_name()),
+            run_id=config.get("run_id"),
         )
         try:
+            bg: list[concurrent.futures.Future] = []
             if config["recursion_limit"] < 1:
                 raise ValueError("recursion_limit must be at least 1")
+            if self.checkpointer and not config.get("configurable"):
+                raise ValueError(
+                    f"Checkpointer requires one or more of the following 'configurable' keys: {[s.id for s in self.checkpointer.config_specs]}"
+                )
             # assign defaults
             (
                 debug,
                 stream_mode,
                 input_keys,
                 output_keys,
-                interrupt_before_nodes,
-                interrupt_after_nodes,
+                interrupt_before,
+                interrupt_after,
             ) = self._defaults(
+                config,
                 stream_mode=stream_mode,
                 input_keys=input_keys,
                 output_keys=output_keys,
-                interrupt_before_nodes=interrupt_before_nodes,
-                interrupt_after_nodes=interrupt_after_nodes,
+                interrupt_before=interrupt_before,
+                interrupt_after=interrupt_after,
                 debug=debug,
             )
             # copy nodes to ignore mutations during execution
             processes = {**self.nodes}
             # get checkpoint from saver, or create an empty one
-            checkpoint_config = config
-            checkpoint = (
-                self.checkpointer.get(checkpoint_config) if self.checkpointer else None
-            )
-            checkpoint = checkpoint or empty_checkpoint()
+            saved = self.checkpointer.get_tuple(config) if self.checkpointer else None
+            checkpoint = saved.checkpoint if saved else empty_checkpoint()
+            checkpoint_config = saved.config if saved else config
+            start = saved.metadata.get("step", -2) + 1 if saved else -1
             # create channels from checkpoint
             with ChannelsManager(
                 self.channels, checkpoint
             ) as channels, get_executor_for_config(config) as executor:
                 # map inputs to channel updates
                 if input_writes := deque(map_input(input_keys, input)):
                     # discard any unfinished tasks from previous checkpoint
                     checkpoint, _ = _prepare_next_tasks(
                         checkpoint, processes, channels, for_execution=True
                     )
                     # apply input writes
                     _apply_writes(checkpoint, channels, input_writes)
+                    # save input checkpoint
+                    if self.checkpointer is not None:
+                        checkpoint = create_checkpoint(checkpoint, channels)
+                        bg.append(
+                            executor.submit(
+                                self.checkpointer.put,
+                                checkpoint_config,
+                                copy_checkpoint(checkpoint),
+                                {"source": "input", "step": start},
+                            )
+                        )
+                        checkpoint_config = {
+                            "configurable": {
+                                "thread_id": checkpoint_config["configurable"][
+                                    "thread_id"
+                                ],
+                                "thread_ts": checkpoint["ts"],
+                            }
+                        }
+                    # increment start to 0
+                    start += 1
                 else:
                     # if received no input, take that as signal to proceed
                     # past previous interrupt, if any
                     checkpoint = copy_checkpoint(checkpoint)
                     for k in self.stream_channels_list:
                         version = checkpoint["channel_versions"][k]
                         checkpoint["versions_seen"][INTERRUPT][k] = version
 
                 # Similarly to Bulk Synchronous Parallel / Pregel model
                 # computation proceeds in steps, while there are channel updates
                 # channel updates from step N are only visible in step N+1
                 # channels are guaranteed to be immutable for the duration of the step,
                 # with channel updates applied only at the transition between steps
-                for step in range(config["recursion_limit"] + 1):
+                stop = start + config["recursion_limit"] + 1
+                for step in range(start, stop):
                     next_checkpoint, next_tasks = _prepare_next_tasks(
                         checkpoint, processes, channels, for_execution=True
                     )
 
                     # if no more tasks, we're done
                     if not next_tasks:
                         if step == 0:
@@ -633,24 +718,27 @@
                             "without hitting a stop condition. You can increase the "
                             "limit by setting the `recursion_limit` config key."
                         )
 
                     # before execution, check if we should interrupt
                     if _should_interrupt(
                         checkpoint,
-                        interrupt_before_nodes,
+                        interrupt_before,
                         self.stream_channels_list,
                         next_tasks,
                     ):
                         break
                     else:
                         checkpoint = next_checkpoint
 
                     if debug:
-                        print_step_start(step, next_tasks)
+                        print_step_tasks(step, next_tasks)
+                    if stream_mode == "debug":
+                        for chunk in map_debug_tasks(step, next_tasks):
+                            yield chunk
 
                     # prepare tasks with config
                     tasks_w_config = [
                         (
                             proc,
                             input,
                             patch_config(
@@ -662,15 +750,15 @@
                                     CONFIG_KEY_SEND: writes.extend,
                                     CONFIG_KEY_READ: partial(
                                         _local_read, checkpoint, channels, writes
                                     ),
                                 },
                             ),
                         )
-                        for name, input, proc, writes, proc_config in next_tasks
+                        for name, input, proc, writes, proc_config, _ in next_tasks
                     ]
 
                     futures = [
                         executor.submit(proc.invoke, input, config)
                         for proc, input, config in tasks_w_config
                     ]
 
@@ -683,149 +771,209 @@
                     )
 
                     # panic on failure or timeout
                     _panic_or_proceed(done, inflight, step)
 
                     # combine pending writes from all tasks
                     pending_writes = deque[tuple[str, Any]]()
-                    for _, _, _, writes, _ in next_tasks:
+                    for _, _, _, writes, _, _ in next_tasks:
                         pending_writes.extend(writes)
 
+                    if debug:
+                        print_step_writes(
+                            step, pending_writes, self.stream_channels_list
+                        )
+
                     # apply writes to channels
                     _apply_writes(checkpoint, channels, pending_writes)
 
                     if debug:
-                        print_checkpoint(step, channels)
+                        print_step_checkpoint(step, channels, self.stream_channels_list)
 
                     # yield current value or updates
                     if stream_mode == "values":
                         yield from map_output_values(
                             output_keys, pending_writes, channels
                         )
+                    elif stream_mode == "debug":
+                        yield from map_debug_task_results(
+                            step, next_tasks, self.stream_channels_list
+                        )
                     else:
                         yield from map_output_updates(output_keys, next_tasks)
 
                     # save end of step checkpoint
-                    if self.checkpointer is not None and (
-                        self.checkpointer.at == CheckpointAt.END_OF_STEP
-                    ):
+                    if self.checkpointer is not None:
                         checkpoint = create_checkpoint(checkpoint, channels)
-                        checkpoint_config = self.checkpointer.put(
-                            checkpoint_config, checkpoint
+                        bg.append(
+                            executor.submit(
+                                self.checkpointer.put,
+                                checkpoint_config,
+                                copy_checkpoint(checkpoint),
+                                {"source": "loop", "step": step},
+                            )
+                        )
+                        checkpoint_config = {
+                            "configurable": {
+                                "thread_id": checkpoint_config["configurable"][
+                                    "thread_id"
+                                ],
+                                "thread_ts": checkpoint["ts"],
+                            }
+                        }
+                    # yield debug checkpoint
+                    if stream_mode == "debug":
+                        yield map_debug_checkpoint(
+                            step,
+                            checkpoint_config if self.checkpointer else None,
+                            channels,
+                            self.stream_channels_asis,
                         )
 
                     # after execution, check if we should interrupt
                     if _should_interrupt(
                         checkpoint,
-                        interrupt_after_nodes,
+                        interrupt_after,
                         self.stream_channels_list,
                         next_tasks,
                     ):
                         break
 
                 # set final channel values as run output
                 run_manager.on_chain_end(read_channels(channels, output_keys))
-
-                # save end of run checkpoint
-                if (
-                    self.checkpointer is not None
-                    and self.checkpointer.at == CheckpointAt.END_OF_RUN
-                ):
-                    checkpoint = create_checkpoint(checkpoint, channels)
-                    self.checkpointer.put(checkpoint_config, checkpoint)
         except BaseException as e:
             run_manager.on_chain_error(e)
             raise
         finally:
             # cancel any pending tasks when generator is interrupted
             try:
                 for task in futures:
                     task.cancel()
             except NameError:
                 pass
+            # wait for all background tasks to finish
+            done, _ = concurrent.futures.wait(
+                bg, return_when=concurrent.futures.ALL_COMPLETED
+            )
+            for task in done:
+                task.result()
 
     async def astream(
         self,
         input: Union[dict[str, Any], Any],
         config: Optional[RunnableConfig] = None,
         *,
         stream_mode: Optional[StreamMode] = None,
         output_keys: Optional[Union[str, Sequence[str]]] = None,
         input_keys: Optional[Union[str, Sequence[str]]] = None,
-        interrupt_before_nodes: Optional[Sequence[str]] = None,
-        interrupt_after_nodes: Optional[Sequence[str]] = None,
+        interrupt_before: Optional[Union[All, Sequence[str]]] = None,
+        interrupt_after: Optional[Union[All, Sequence[str]]] = None,
         debug: Optional[bool] = None,
     ) -> AsyncIterator[Union[dict[str, Any], Any]]:
         config = ensure_config(config)
         callback_manager = get_async_callback_manager_for_config(config)
         run_manager = await callback_manager.on_chain_start(
-            dumpd(self), input, name=config.get("run_name", self.get_name())
+            dumpd(self),
+            input,
+            name=config.get("run_name", self.get_name()),
+            run_id=config.get("run_id"),
         )
         # if running from astream_log() run each proc with streaming
         do_stream = next(
             (
                 h
                 for h in run_manager.handlers
                 if isinstance(h, LogStreamCallbackHandler)
             ),
             None,
         )
         try:
+            bg: list[asyncio.Task] = []
             if config["recursion_limit"] < 1:
                 raise ValueError("recursion_limit must be at least 1")
+            if self.checkpointer and not config.get("configurable"):
+                raise ValueError(
+                    f"Checkpointer requires one or more of the following 'configurable' keys: {[s.id for s in self.checkpointer.config_specs]}"
+                )
             # assign defaults
             (
                 debug,
                 stream_mode,
                 input_keys,
                 output_keys,
-                interrupt_before_nodes,
-                interrupt_after_nodes,
+                interrupt_before,
+                interrupt_after,
             ) = self._defaults(
+                config,
                 stream_mode=stream_mode,
                 input_keys=input_keys,
                 output_keys=output_keys,
-                interrupt_before_nodes=interrupt_before_nodes,
-                interrupt_after_nodes=interrupt_after_nodes,
+                interrupt_before=interrupt_before,
+                interrupt_after=interrupt_after,
                 debug=debug,
             )
             # copy nodes to ignore mutations during execution
             processes = {**self.nodes}
             # get checkpoint from saver, or create an empty one
-            checkpoint_config = config
-            checkpoint = (
-                await self.checkpointer.aget(checkpoint_config)
+            saved = (
+                await self.checkpointer.aget_tuple(config)
                 if self.checkpointer
                 else None
             )
-            checkpoint = checkpoint or empty_checkpoint()
+            checkpoint = saved.checkpoint if saved else empty_checkpoint()
+            checkpoint_config = saved.config if saved else config
+            start = saved.metadata.get("step", -2) + 1 if saved else -1
             # create channels from checkpoint
             async with AsyncChannelsManager(self.channels, checkpoint) as channels:
                 # map inputs to channel updates
                 if input_writes := deque(map_input(input_keys, input)):
                     # discard any unfinished tasks from previous checkpoint
                     checkpoint, _ = _prepare_next_tasks(
                         checkpoint, processes, channels, for_execution=True
                     )
                     # apply input writes
                     _apply_writes(checkpoint, channels, input_writes)
+                    # save input checkpoint
+                    if self.checkpointer is not None:
+                        checkpoint = create_checkpoint(checkpoint, channels)
+                        bg.append(
+                            asyncio.create_task(
+                                self.checkpointer.aput(
+                                    checkpoint_config,
+                                    copy_checkpoint(checkpoint),
+                                    {"source": "input", "step": start},
+                                )
+                            )
+                        )
+                        checkpoint_config = {
+                            "configurable": {
+                                "thread_id": checkpoint_config["configurable"][
+                                    "thread_id"
+                                ],
+                                "thread_ts": checkpoint["ts"],
+                            }
+                        }
+                    # increment start to 0
+                    start += 1
                 else:
                     # if received no input, take that as signal to proceed
                     # past previous interrupt, if any
                     checkpoint = copy_checkpoint(checkpoint)
                     for k in self.stream_channels_list:
                         version = checkpoint["channel_versions"][k]
                         checkpoint["versions_seen"][INTERRUPT][k] = version
 
                 # Similarly to Bulk Synchronous Parallel / Pregel model
                 # computation proceeds in steps, while there are channel updates
                 # channel updates from step N are only visible in step N+1,
                 # channels are guaranteed to be immutable for the duration of the step,
                 # channel updates being applied only at the transition between steps
-                for step in range(config["recursion_limit"] + 1):
+                start = saved.metadata.get("step", -1) + 1 if saved else 0
+                stop = start + config["recursion_limit"] + 1
+                for step in range(start, stop):
                     next_checkpoint, next_tasks = _prepare_next_tasks(
                         checkpoint, processes, channels, for_execution=True
                     )
 
                     # if no more tasks, we're done
                     if not next_tasks:
                         if step == 0:
@@ -838,24 +986,27 @@
                             "without hitting a stop condition. You can increase the limit"
                             "by setting the `recursion_limit` config key."
                         )
 
                     # before execution, check if we should interrupt
                     if _should_interrupt(
                         checkpoint,
-                        interrupt_before_nodes,
+                        interrupt_before,
                         self.stream_channels_list,
                         next_tasks,
                     ):
                         break
                     else:
                         checkpoint = next_checkpoint
 
                     if debug:
-                        print_step_start(step, next_tasks)
+                        print_step_tasks(step, next_tasks)
+                    if stream_mode == "debug":
+                        for chunk in map_debug_tasks(step, next_tasks):
+                            yield chunk
 
                     # prepare tasks with config
                     tasks_w_config = [
                         (
                             proc,
                             input,
                             patch_config(
@@ -867,15 +1018,15 @@
                                     CONFIG_KEY_SEND: writes.extend,
                                     CONFIG_KEY_READ: partial(
                                         _local_read, checkpoint, channels, writes
                                     ),
                                 },
                             ),
                         )
-                        for name, input, proc, writes, proc_config in next_tasks
+                        for name, input, proc, writes, proc_config, _ in next_tasks
                     ]
 
                     futures = (
                         [
                             asyncio.create_task(_aconsume(proc.astream(input, config)))
                             for proc, input, config in tasks_w_config
                         ]
@@ -895,98 +1046,140 @@
                     )
 
                     # panic on failure or timeout
                     _panic_or_proceed(done, inflight, step)
 
                     # combine pending writes from all tasks
                     pending_writes = deque[tuple[str, Any]]()
-                    for _, _, _, writes, _ in next_tasks:
+                    for _, _, _, writes, _, _ in next_tasks:
                         pending_writes.extend(writes)
 
+                    if debug:
+                        print_step_writes(
+                            step, pending_writes, self.stream_channels_list
+                        )
+
                     # apply writes to channels
                     _apply_writes(checkpoint, channels, pending_writes)
 
                     if debug:
-                        print_checkpoint(step, channels)
+                        print_step_checkpoint(step, channels, self.stream_channels_list)
 
                     # yield current value or updates
                     if stream_mode == "values":
                         for chunk in map_output_values(
                             output_keys, pending_writes, channels
                         ):
                             yield chunk
+                    elif stream_mode == "debug":
+                        for chunk in map_debug_task_results(
+                            step, next_tasks, self.stream_channels_list
+                        ):
+                            yield chunk
                     else:
                         for chunk in map_output_updates(output_keys, next_tasks):
                             yield chunk
 
                     # save end of step checkpoint
-                    if self.checkpointer is not None and (
-                        self.checkpointer.at == CheckpointAt.END_OF_STEP
-                    ):
+                    if self.checkpointer is not None:
                         checkpoint = create_checkpoint(checkpoint, channels)
-                        checkpoint_config = await self.checkpointer.aput(
-                            checkpoint_config, checkpoint
+                        bg.append(
+                            asyncio.create_task(
+                                self.checkpointer.aput(
+                                    checkpoint_config,
+                                    checkpoint,
+                                    {"source": "loop", "step": step},
+                                )
+                            )
+                        )
+                        checkpoint_config = {
+                            "configurable": {
+                                "thread_id": checkpoint_config["configurable"][
+                                    "thread_id"
+                                ],
+                                "thread_ts": checkpoint["ts"],
+                            }
+                        }
+                    # yield debug checkpoint
+                    if stream_mode == "debug":
+                        yield map_debug_checkpoint(
+                            step,
+                            checkpoint_config if self.checkpointer else None,
+                            channels,
+                            self.stream_channels_asis,
                         )
 
                     # after execution, check if we should interrupt
                     if _should_interrupt(
                         checkpoint,
-                        interrupt_after_nodes,
+                        interrupt_after,
                         self.stream_channels_list,
                         next_tasks,
                     ):
                         break
 
                 # set final channel values as run output
                 await run_manager.on_chain_end(read_channels(channels, output_keys))
-
-                # save end of run checkpoint
-                if (
-                    self.checkpointer is not None
-                    and self.checkpointer.at == CheckpointAt.END_OF_RUN
-                ):
-                    checkpoint = create_checkpoint(checkpoint, channels)
-                    await self.checkpointer.aput(checkpoint_config, checkpoint)
         except BaseException as e:
             await run_manager.on_chain_error(e)
             raise
         finally:
             # cancel any pending tasks when generator is interrupted
             try:
                 for task in futures:
                     task.cancel()
+                    bg.append(task)
             except NameError:
                 pass
+            # wait for all background tasks to finish
+            await asyncio.gather(*bg)
 
     def invoke(
         self,
         input: Union[dict[str, Any], Any],
         config: Optional[RunnableConfig] = None,
         *,
         stream_mode: StreamMode = "values",
         output_keys: Optional[Union[str, Sequence[str]]] = None,
         input_keys: Optional[Union[str, Sequence[str]]] = None,
-        interrupt_before_nodes: Optional[Sequence[str]] = None,
-        interrupt_after_nodes: Optional[Sequence[str]] = None,
+        interrupt_before: Optional[Union[All, Sequence[str]]] = None,
+        interrupt_after: Optional[Union[All, Sequence[str]]] = None,
         debug: Optional[bool] = None,
         **kwargs: Any,
     ) -> Union[dict[str, Any], Any]:
+        """Run the graph with a single input and config.
+
+        Args:
+            input: The input data for the graph. It can be a dictionary or any other type.
+            config: Optional. The configuration for the graph run.
+            stream_mode: Optional[str]. The stream mode for the graph run. Default is "values".
+            output_keys: Optional. The output keys to retrieve from the graph run.
+            input_keys: Optional. The input keys to provide for the graph run.
+            interrupt_before: Optional. The nodes to interrupt the graph run before.
+            interrupt_after: Optional. The nodes to interrupt the graph run after.
+            debug: Optional. Enable debug mode for the graph run.
+            **kwargs: Additional keyword arguments to pass to the graph run.
+
+        Returns:
+            The output of the graph run. If stream_mode is "values", it returns the latest output.
+            If stream_mode is not "values", it returns a list of output chunks.
+        """
         output_keys = output_keys if output_keys is not None else self.output_channels
         if stream_mode == "values":
             latest: Union[dict[str, Any], Any] = None
         else:
             chunks = []
         for chunk in self.stream(
             input,
             config,
             stream_mode=stream_mode,
             output_keys=output_keys,
             input_keys=input_keys,
-            interrupt_before_nodes=interrupt_before_nodes,
-            interrupt_after_nodes=interrupt_after_nodes,
+            interrupt_before=interrupt_before,
+            interrupt_after=interrupt_after,
             debug=debug,
             **kwargs,
         ):
             if stream_mode == "values":
                 latest = chunk
             else:
                 chunks.append(chunk)
@@ -999,32 +1192,50 @@
         self,
         input: Union[dict[str, Any], Any],
         config: Optional[RunnableConfig] = None,
         *,
         stream_mode: StreamMode = "values",
         output_keys: Optional[Union[str, Sequence[str]]] = None,
         input_keys: Optional[Union[str, Sequence[str]]] = None,
-        interrupt_before_nodes: Optional[Sequence[str]] = None,
-        interrupt_after_nodes: Optional[Sequence[str]] = None,
+        interrupt_before: Optional[Union[All, Sequence[str]]] = None,
+        interrupt_after: Optional[Union[All, Sequence[str]]] = None,
         debug: Optional[bool] = None,
         **kwargs: Any,
     ) -> Union[dict[str, Any], Any]:
+        """Asynchronously invoke the graph on a single input.
+
+        Args:
+            input: The input data for the computation. It can be a dictionary or any other type.
+            config: Optional. The configuration for the computation.
+            stream_mode: Optional. The stream mode for the computation. Default is "values".
+            output_keys: Optional. The output keys to include in the result. Default is None.
+            input_keys: Optional. The input keys to include in the result. Default is None.
+            interrupt_before: Optional. The nodes to interrupt before. Default is None.
+            interrupt_after: Optional. The nodes to interrupt after. Default is None.
+            debug: Optional. Whether to enable debug mode. Default is None.
+            **kwargs: Additional keyword arguments.
+
+        Returns:
+            The result of the computation. If stream_mode is "values", it returns the latest value.
+            If stream_mode is "chunks", it returns a list of chunks.
+        """
+
         output_keys = output_keys if output_keys is not None else self.output_channels
         if stream_mode == "values":
             latest: Union[dict[str, Any], Any] = None
         else:
             chunks = []
         async for chunk in self.astream(
             input,
             config,
             stream_mode=stream_mode,
             output_keys=output_keys,
             input_keys=input_keys,
-            interrupt_before_nodes=interrupt_before_nodes,
-            interrupt_after_nodes=interrupt_after_nodes,
+            interrupt_before=interrupt_before,
+            interrupt_after=interrupt_after,
             debug=debug,
             **kwargs,
         ):
             if stream_mode == "values":
                 latest = chunk
             else:
                 chunks.append(chunk)
@@ -1056,28 +1267,36 @@
             inflight.pop().cancel()
         # raise timeout error
         raise TimeoutError(f"Timed out at step {step}")
 
 
 def _should_interrupt(
     checkpoint: Checkpoint,
-    interrupt_nodes: Sequence[str],
+    interrupt_nodes: Union[All, Sequence[str]],
     snapshot_channels: Sequence[str],
     tasks: list[PregelExecutableTask],
 ) -> bool:
     # defaultdicts are mutated on access :( so we need to copy
     seen = checkpoint["versions_seen"].copy()[INTERRUPT].copy()
     return (
         # interrupt if any of snapshopt_channels has been updated since last interrupt
         any(
             checkpoint["channel_versions"][chan] > seen[chan]
             for chan in snapshot_channels
         )
         # and any channel written to is in interrupt_nodes list
-        and any(node for node, _, _, _, _ in tasks if node in interrupt_nodes)
+        and any(
+            node
+            for node, _, _, _, config, _ in tasks
+            if (
+                (not config or TAG_HIDDEN not in config.get("tags"))
+                if interrupt_nodes == "*"
+                else node in interrupt_nodes
+            )
+        )
     )
 
 
 def _local_read(
     checkpoint: Checkpoint,
     channels: Mapping[str, BaseChannel],
     writes: Sequence[tuple[str, Any]],
@@ -1159,21 +1378,22 @@
     checkpoint = copy_checkpoint(checkpoint)
     tasks: Union[list[PregelTaskDescription], list[PregelExecutableTask]] = []
     # Check if any processes should be run in next step
     # If so, prepare the values to be passed to them
     for name, proc in processes.items():
         seen = checkpoint["versions_seen"][name]
         # If any of the channels read by this process were updated
-        if any(
-            checkpoint["channel_versions"][chan] > seen[chan]
+        if triggers := [
+            chan
             for chan in proc.triggers
             if not isinstance(
                 read_channel(channels, chan, return_exception=True), EmptyChannelError
             )
-        ):
+            and checkpoint["channel_versions"][chan] > seen[chan]
+        ]:
             # If all trigger channels subscribed by this process are not empty
             # then invoke the process with the values of all non-empty channels
             if isinstance(proc.channels, dict):
                 try:
                     val: Any = {
                         k: read_channel(channels, chan, catch=chan not in proc.triggers)
                         for k, chan in proc.channels.items()
@@ -1206,15 +1426,17 @@
                         for chan in proc.triggers
                     }
                 )
 
             if for_execution:
                 if node := proc.get_node():
                     tasks.append(
-                        PregelExecutableTask(name, val, node, deque(), proc.config)
+                        PregelExecutableTask(
+                            name, val, node, deque(), proc.config, triggers
+                        )
                     )
             else:
                 tasks.append(PregelTaskDescription(name, val))
     return checkpoint, tasks
 
 
 async def _aconsume(iterator: AsyncIterator[Any]) -> None:
```

### Comparing `gigagraph-0.0.37/langgraph/pregel/read.py` & `gigagraph-0.0.45/langgraph/pregel/read.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.37/langgraph/pregel/validate.py` & `gigagraph-0.0.45/langgraph/pregel/validate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,54 @@
-from typing import Any, Mapping, Optional, Sequence, Type, Union
+from typing import Mapping, Optional, Sequence, Union
 
 from langgraph.channels.base import BaseChannel
 from langgraph.constants import INTERRUPT
 from langgraph.pregel.read import PregelNode
+from langgraph.pregel.types import All
 
 
 def validate_graph(
     nodes: Mapping[str, PregelNode],
     channels: dict[str, BaseChannel],
     input_channels: Union[str, Sequence[str]],
     output_channels: Union[str, Sequence[str]],
     stream_channels: Optional[Union[str, Sequence[str]]],
-    interrupt_after_nodes: Sequence[str],
-    interrupt_before_nodes: Sequence[str],
-    default_channel_cls: Type[BaseChannel],
+    interrupt_after_nodes: Union[All, Sequence[str]],
+    interrupt_before_nodes: Union[All, Sequence[str]],
 ) -> None:
+    for chan in channels:
+        if chan == INTERRUPT:
+            raise ValueError(f"Channel name {INTERRUPT} is reserved")
+
     subscribed_channels = set[str]()
     for name, node in nodes.items():
         if name == INTERRUPT:
             raise ValueError(f"Node name {INTERRUPT} is reserved")
         if isinstance(node, PregelNode):
             subscribed_channels.update(node.triggers)
         else:
             raise TypeError(
                 f"Invalid node type {type(node)}, expected Channel.subscribe_to()"
             )
 
     for chan in subscribed_channels:
         if chan not in channels:
-            channels[chan] = default_channel_cls(Any)  # type: ignore[arg-type]
+            raise ValueError(f"Subscribed channel '{chan}' not in 'channels'")
 
     if isinstance(input_channels, str):
         if input_channels not in channels:
-            channels[input_channels] = default_channel_cls(Any)  # type: ignore[arg-type]
+            raise ValueError(f"Input channel '{input_channels}' not in 'channels'")
         if input_channels not in subscribed_channels:
             raise ValueError(
                 f"Input channel {input_channels} is not subscribed to by any node"
             )
     else:
         for chan in input_channels:
             if chan not in channels:
-                channels[chan] = default_channel_cls(Any)  # type: ignore[arg-type]
+                raise ValueError(f"Input channel '{chan}' not in 'channels'")
         if all(chan not in subscribed_channels for chan in input_channels):
             raise ValueError(
                 f"None of the input channels {input_channels} are subscribed to by any node"
             )
 
     all_output_channels = set[str]()
     if isinstance(output_channels, str):
@@ -54,22 +58,24 @@
     if isinstance(stream_channels, str):
         all_output_channels.add(stream_channels)
     elif stream_channels is not None:
         all_output_channels.update(stream_channels)
 
     for chan in all_output_channels:
         if chan not in channels:
-            channels[chan] = default_channel_cls(Any)  # type: ignore[arg-type]
+            raise ValueError(f"Output channel '{chan}' not in 'channels'")
 
-    for node in interrupt_after_nodes:
-        if node not in nodes:
-            raise ValueError(f"Node {node} not in nodes")
-    for node in interrupt_before_nodes:
-        if node not in nodes:
-            raise ValueError(f"Node {node} not in nodes")
+    if interrupt_after_nodes != "*":
+        for node in interrupt_after_nodes:
+            if node not in nodes:
+                raise ValueError(f"Node {node} not in nodes")
+    if interrupt_before_nodes != "*":
+        for node in interrupt_before_nodes:
+            if node not in nodes:
+                raise ValueError(f"Node {node} not in nodes")
 
 
 def validate_keys(
     keys: Optional[Union[str, Sequence[str]]],
     channels: Mapping[str, BaseChannel],
 ) -> None:
     if isinstance(keys, str):
```

### Comparing `gigagraph-0.0.37/pyproject.toml` & `gigagraph-0.0.45/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 [tool.poetry]
 name = "gigagraph"
-version = "0.0.37"
+version = "0.0.45"
 description = "langgraph"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ai-forever/gigagraph"
 packages = [
     {include = "langgraph"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9.0,<4.0"
-gigachain-core = "^0.1.42rc1"
+gigachain-core = "^0.1.48"
 
 
 [tool.poetry.group.test.dependencies]
 # The only dependencies that should be added are
 # dependencies used for running tests (e.g., pytest, freezegun, response).
 # Any dependencies that do not meet that criteria will be removed.
 pytest = "^7.3.0"
 pytest-cov = "^4.0.0"
 pytest-dotenv = "^0.5.2"
 pytest-asyncio = "^0.20.3"
 pytest-mock  = "^3.10.0"
 syrupy = "^4.0.2"
 httpx = "^0.26.0"
 pytest-watcher = "^0.4.1"
-gigachain = "^0.1.0"
+gigachain = "^0.1.17"
 aiosqlite = "^0.19.0"
 grandalf = "^0.8"
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.4"
 
 [tool.poetry.group.typing.dependencies]
 mypy = "^1.6.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
-gigachain = "^0.1.0"
+gigachain = "^0.1.16"
 langchainhub = "^0.1.14"
-gigachain-openai = "^0.1.2"
+gigachain-openai = ">=0.1.1"
 
 [tool.ruff]
 select = [ "E", "F", "I" ]
 ignore = [ "E501" ]
 
 [tool.mypy]
 ignore_missing_imports = "True"
```

### Comparing `gigagraph-0.0.37/PKG-INFO` & `gigagraph-0.0.45/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: gigagraph
-Version: 0.0.37
+Version: 0.0.45
 Summary: langgraph
 Home-page: https://github.com/ai-forever/gigagraph
 License: MIT
 Requires-Python: >=3.9.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: gigachain-core (>=0.1.42rc1,<0.2.0)
+Requires-Dist: gigachain-core (>=0.1.48,<0.2.0)
 Project-URL: Repository, https://github.com/ai-forever/gigagraph
 Description-Content-Type: text/markdown
 
 # GigaGraph
 
 ⚡ Разработка языковых агентов в виде графов ⚡
 
@@ -39,18 +39,199 @@
 ```
 
 ## Быстрый старт
 
 Ниже приводится пример разработки агента, использующего несколько моделей и вызов функций.
 Агент отображает каждое свое состояние в виде отдельных сообщений в списке
 
-Для работы агента потребуется установить некоторые пакеты LangChain и использовать в качестве демонстрации сервис [Tavily](https://app.tavily.com/sign-in):
+Для работы агента потребуется установить некоторые пакеты GigaChain и использовать в качестве демонстрации сервис [Tavily](https://app.tavily.com/sign-in):
+
+State in LangGraph can be pretty general, but to keep things simpler to start, we'll show off an example where the graph's state is limited to a list of chat messages using the built-in `MessageGraph` class. This is convenient when using LangGraph with LangChain chat models because we can return chat model output directly.
+
+First, install the GigaChain OpenAI integration package:
+
+```python
+pip install gigachain_openai
+```
+
+We also need to export some environment variables:
 
 ```shell
-pip install -U langchain langchain_openai tavily-python
+export OPENAI_API_KEY=sk-...
+```
+
+And now we're ready! The graph below contains a single node called `"oracle"` that executes a chat model, then returns the result:
+
+```python
+from langchain_openai import ChatOpenAI
+from langchain_core.messages import HumanMessage
+from langgraph.graph import END, MessageGraph
+
+model = ChatOpenAI(temperature=0)
+
+graph = MessageGraph()
+
+graph.add_node("oracle", model)
+graph.add_edge("oracle", END)
+
+graph.set_entry_point("oracle")
+
+runnable = graph.compile()
+```
+
+Let's run it!
+
+```python
+runnable.invoke(HumanMessage("What is 1 + 1?"))
+```
+
+```
+[HumanMessage(content='What is 1 + 1?'), AIMessage(content='1 + 1 equals 2.')]
+```
+
+So what did we do here? Let's break it down step by step:
+
+1. First, we initialize our model and a `MessageGraph`.
+2. Next, we add a single node to the graph, called `"oracle"`, which simply calls the model with the given input.
+3. We add an edge from this `"oracle"` node to the special string `END`. This means that execution will end after current node.
+4. We set `"oracle"` as the entrypoint to the graph.
+5. We compile the graph, ensuring that no more modifications to it can be made.
+
+Then, when we execute the graph:
+
+1. LangGraph adds the input message to the internal state, then passes the state to the entrypoint node, `"oracle"`.
+2. The `"oracle"` node executes, invoking the chat model.
+3. The chat model returns an `AIMessage`. LangGraph adds this to the state.
+4. Execution progresses to the special `END` value and outputs the final state.
+
+And as a result, we get a list of two chat messages as output.
+
+### Interaction with LCEL
+
+As an aside for those already familiar with LangChain - `add_node` actually takes any function or runnable as input. In the above example, the model is used "as-is", but we could also have passed in a function:
+
+```python
+def call_oracle(messages: list):
+    return model.invoke(messages)
+
+graph.add_node("oracle", call_oracle)
+```
+
+Just make sure you are mindful of the fact that the input to the runnable is the **entire current state**. So this will fail:
+
+```python
+# This will not work with MessageGraph!
+from langchain_core.prompts import ChatPromptTemplate, MessagesPlaceholder
+
+prompt = ChatPromptTemplate.from_messages([
+    ("system", "You are a helpful assistant named {name} who always speaks in pirate dialect"),
+    MessagesPlaceholder(variable_name="messages"),
+])
+
+chain = prompt | model
+
+# State is a list of messages, but our chain expects a dict input:
+#
+# { "name": some_string, "messages": [] }
+#
+# Therefore, the graph will throw an exception when it executes here.
+graph.add_node("oracle", chain)
+```
+
+## Conditional edges
+
+Now, let's move onto something a little bit less trivial. Because math can be difficult for LLMs, let's allow the LLM to conditionally call a `"multiply"` node using tool calling.
+
+We'll recreate our graph with an additional `"multiply"` that will take the result of the most recent message, if it is a tool call, and calculate the result.
+We'll also [bind](https://api.python.langchain.com/en/latest/chat_models/langchain_openai.chat_models.base.ChatOpenAI.html#langchain_openai.chat_models.base.ChatOpenAI.bind_tools) the calculator to the OpenAI model as a tool to allow the model to optionally use the tool necessary to respond to the current state:
+
+```python
+from langchain_core.tools import tool
+from langgraph.prebuilt import ToolNode
+
+@tool
+def multiply(first_number: int, second_number: int):
+    """Multiplies two numbers together."""
+    return first_number * second_number
+
+model = ChatOpenAI(temperature=0)
+model_with_tools = model.bind_tools([multiply])
+
+graph = MessageGraph()
+
+graph.add_node("oracle", model_with_tools)
+
+tool_node = ToolNode([multiply])
+graph.add_node("multiply", tool_node)
+
+graph.add_edge("multiply", END)
+
+graph.set_entry_point("oracle")
+```
+
+Now let's think - what do we want to have happened?
+
+- If the `"oracle"` node returns a message expecting a tool call, we want to execute the `"multiply"` node
+- If not, we can just end execution
+
+We can achieve this using **conditional edges**, which routes execution to a node based on the current state using a function.
+
+Here's what that looks like:
+
+```python
+def router(state: List[BaseMessage]):
+    tool_calls = state[-1].additional_kwargs.get("tool_calls", [])
+    if len(tool_calls):
+        return "multiply"
+    else:
+        return "end"
+
+graph.add_conditional_edges("oracle", router, {
+    "multiply": "multiply",
+    "end": END,
+})
+```
+
+If the model output contains a tool call, we move to the `"multiply"` node. Otherwise, we end.
+
+Great! Now all that's left is to compile the graph and try it out. Math-related questions are routed to the calculator tool:
+
+```python
+runnable = graph.compile()
+
+runnable.invoke(HumanMessage("What is 123 * 456?"))
+```
+
+```
+
+[HumanMessage(content='What is 123 * 456?'),
+ AIMessage(content='', additional_kwargs={'tool_calls': [{'id': 'call_OPbdlm8Ih1mNOObGf3tMcNgb', 'function': {'arguments': '{"first_number":123,"second_number":456}', 'name': 'multiply'}, 'type': 'function'}]}),
+ ToolMessage(content='56088', tool_call_id='call_OPbdlm8Ih1mNOObGf3tMcNgb')]
+```
+
+While conversational responses are outputted directly:
+
+```python
+runnable.invoke(HumanMessage("What is your name?"))
+```
+
+```
+[HumanMessage(content='What is your name?'),
+ AIMessage(content='My name is Assistant. How can I assist you today?')]
+```
+
+## Cycles
+
+Now, let's go over a more general example with a cycle. We will recreate the `AgentExecutor` class from LangChain. The agent itself will use chat models and function calling.
+This agent will represent all its state as a list of messages.
+
+We will need to install some GigaChain packages, as well as [Tavily](https://app.tavily.com/sign-in) to use as an example tool.
+
+```shell
+pip install -U gigachain gigachain_openai tavily-python
 ```
 
 Также для доступа к OpenAI и Tavily API понадобится задать переменные среды:
 
 ```shell
 export OPENAI_API_KEY=sk-...
 export TAVILY_API_KEY=tvly-...
@@ -102,18 +283,15 @@
 model = ChatOpenAI(temperature=0, streaming=True)
 ```
 
 После подключения убедитесь, что модель знает, какие инструменты доступны ей.
 Для этого преобразуйте инструменты GigaGraph в формат OpenAI-функций и привяжите их к классу модели.
 
 ```python
-from langchain.tools.render import format_tool_to_openai_function
-
-functions = [format_tool_to_openai_function(t) for t in tools]
-model = model.bind_functions(functions)
+model = model.bind_tools(tools)
 ```
 
 ### Определите состояние агента
 
 Основным графом `gigagraph` является `StatefulGraph`.
 Этот граф параметризован объектом состояния, который он передает каждой вершине.
 В свою очередь каждая вершина возвращает операции для обновления состояния.
@@ -122,21 +300,22 @@
 
 В приведенном примере отслеживаемое состояние представлено в виде списка сообщений.
 Поэтому нужно чтобы каждая вершина добавляла сообщения в список.
 
 Для этого используйте `TypedDict` с одним ключом (`messages`) и аннотацией, указывающей на то, что в атрибут `messages` можно только добавлять данные.
 
 ```python
-from typing import TypedDict, Annotated, Sequence
-import operator
-from langchain_core.messages import BaseMessage
+from typing import TypedDict, Annotated
+from langgraph.graph.message import add_messages
 
 
 class AgentState(TypedDict):
-    messages: Annotated[Sequence[BaseMessage], operator.add]
+    # The `add_messages` function within the annotation defines
+    # *how* updates should be merged into the state.
+    messages: Annotated[list, add_messages]
 ```
 
 ### Определите вершины графа
 
 Теперь нужно определить несколько разных вершин графа.
 В `langgraph` вершина может быть представлена в виде функции или [исполняемого интерфейса](https://python.langchain.com/docs/expression_language/).
 Для описываемого примера понадобятся две основных вершины:
@@ -330,100 +509,15 @@
 
 ```
 content='' additional_kwargs={'function_call': {'arguments': '', 'name': 'tavily_search_results_json'}}
 content='' additional_kwargs={'function_call': {'arguments': '{\n', 'name': ''}}
 content='' additional_kwargs={'function_call': {'arguments': ' ', 'name': ''}}
 content='' additional_kwargs={'function_call': {'arguments': ' "', 'name': ''}}
 content='' additional_kwargs={'function_call': {'arguments': 'query', 'name': ''}}
-content='' additional_kwargs={'function_call': {'arguments': '":', 'name': ''}}
-content='' additional_kwargs={'function_call': {'arguments': ' "', 'name': ''}}
-content='' additional_kwargs={'function_call': {'arguments': 'weather', 'name': ''}}
-content='' additional_kwargs={'function_call': {'arguments': ' in', 'name': ''}}
-content='' additional_kwargs={'function_call': {'arguments': ' San', 'name': ''}}
-content='' additional_kwargs={'function_call': {'arguments': ' Francisco', 'name': ''}}
-content='' additional_kwargs={'function_call': {'arguments': '"\n', 'name': ''}}
-content='' additional_kwargs={'function_call': {'arguments': '}', 'name': ''}}
-content=''
-content=''
-content='I'
-content="'m"
-content=' sorry'
-content=','
-content=' but'
-content=' I'
-content=' couldn'
-content="'t"
-content=' find'
-content=' the'
-content=' current'
-content=' weather'
-content=' in'
-content=' San'
-content=' Francisco'
-content='.'
-content=' However'
-content=','
-content=' you'
-content=' can'
-content=' check'
-content=' the'
-content=' historical'
-content=' weather'
-content=' data'
-content=' for'
-content=' January'
-content=' '
-content='202'
-content='4'
-content=' in'
-content=' San'
-content=' Francisco'
-content=' ['
-content='here'
-content=']('
-content='https'
-content='://'
-content='we'
-content='athers'
-content='park'
-content='.com'
-content='/h'
-content='/m'
-content='/'
-content='557'
-content='/'
-content='202'
-content='4'
-content='/'
-content='1'
-content='/H'
-content='istorical'
-content='-'
-content='Weather'
-content='-in'
-content='-Jan'
-content='uary'
-content='-'
-content='202'
-content='4'
-content='-in'
-content='-S'
-content='an'
-content='-F'
-content='r'
-content='anc'
-content='isco'
-content='-Cal'
-content='ifornia'
-content='-'
-content='United'
-content='-'
-content='States'
-content=').'
-content=''
+...
 ```
 
 ## Область применения
 
 Используйте библиотеку если вам нужна поддержка циклов.
 
 Если обычной работы с цепочками для решения ваших задач достаточно, используйте основные возможности [LangChain Expression Language](https://python.langchain.com/docs/expression_language/).
@@ -451,15 +545,15 @@
 
 LangGraph comes with built-in support for human-in-the-loop workflows. This is useful when you want to have a human review the current state before proceeding to a particular node.
 For a walkthrough on how to do that, see [this documentation](https://github.com/langchain-ai/langgraph/blob/main/examples/human-in-the-loop.ipynb)
 
 ### Visualizing the graph
 
 Agents you create with LangGraph can be complex. In order to make it easier to understand what is happening under the hood, we've added methods to print out and visualize the graph.
-This can create both ascii art as well as pngs.
+This can create both ascii art and pngs.
 For a walkthrough on how to do that, see [this documentation](https://github.com/langchain-ai/langgraph/blob/main/examples/visualization.ipynb)
 
 ### "Time Travel"
 
 With "time travel" functionality you can jump to any point in the graph execution, modify the state, and rerun from there.
 This is useful for both debugging workflows, as well as end user-facing workflows to allow them to correct the state.
 For a walkthrough on how to do that, see [this documentation](https://github.com/langchain-ai/langgraph/blob/main/examples/time-travel.ipynb)
```

