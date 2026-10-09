# Survey on LLM Agents and Tool Use

## TL;DR
- LLM agents combine model decisions with external tools and feedback to complete multi-step tasks [16][15][14].
- Dynamic workflows and tool planning organize execution beyond individual API calls [13][2].
- Benchmarks examine task automation, long-horizon planning, and real-world MCP tool use [12][10][9][7].
- Tool descriptions, selection, and stateful feedback are practical targets for improving reliability [8][3][1].

## Background
Agents choose actions and tools dynamically, while fixed workflows follow predetermined steps. Retrieval, memory, and feedback extend the model's ability to act beyond a single response [16]. Surveys of agent skills examine how these capabilities are organized, acquired, and secured [15][14].

## Agent Architectures and Workflows
Architecture research moves from static templates toward runtime graphs that adapt execution to the task [13]. Planning methods such as ToolTree explore search over tool sequences, while skill surveys describe reusable capabilities that support broader agent behavior [2][15][14].

## Learning and Reliable Tool Interfaces
Hard-sample generation targets difficult tool-use cases rather than relying only on straightforward training examples [4]. ToolScope addresses overlapping tools through merging and context-aware filtering; tool-description rewriting addresses ambiguity at the interface. These methods act at different stages of tool selection and execution [8][3]. Gecko supplies stateful feedback for refining tool calls [1].

## Benchmarks and Evaluation
UltraTool examines planning, creation, and use of tools; TaskBench focuses on task automation. PlanBench-XL extends evaluation to long-horizon planning in large tool ecosystems [12][10][9]. MCPAgentBench and MCP-RADAR add real-world MCP tasks and multiple dimensions of tool-use capability [7][6]. These benchmarks evaluate different settings, so their results should not be treated as interchangeable [12][9][7][6].

## Deployment and Reliability
Developer and industry surveys provide deployment perspectives alongside academic benchmarks [11][5]. Agent design also requires explicit checks, useful feedback, and appropriate control over tool execution. Reliable interfaces and stateful environments address practical failure points without replacing end-to-end evaluation [16][3][1].

## Trends and Open Problems
Research increasingly combines reusable skills, adaptive workflows, and longer tool sequences. Generalizing across changing toolsets while keeping execution understandable and affordable remains challenging [15][14][13][9]. Better tool selection and consistent evaluation can support this transition, but improvements need validation across realistic tasks [8][7][6].

## References
[1] Gecko: A Simulation Environment with Stateful Feedback for Refining Agent Tool Calls. hf-search. https://huggingface.co/papers/2602.19218 (2026-02-22)
[2] ToolTree: Efficient LLM Agent Tool Planning via Dual-Feedback Monte Carlo Tree Search and Bidirectional Pruning. hf-search. https://huggingface.co/papers/2603.12740 (2026-03-13)
[3] Learning to Rewrite Tool Descriptions for Reliable LLM-Agent Tool Use. hf-search. https://huggingface.co/papers/2602.20426 (2026-02-23)
[4] From Failure to Mastery: Generating Hard Samples for Tool-use Agents. hf-search. https://huggingface.co/papers/2601.01498 (2026-01-04)
[5] LLM industry survey (Rethink Priorities). web. https://rethinkpriorities.org/wp-content/uploads/2025/07/LLM-industry-survey.pdf (n.d.)
[6] MCP-RADAR: A Multi-Dimensional Benchmark for Evaluating Tool Use Capabilities in Large Language Models. hf-search. https://huggingface.co/papers/2505.16700 (2025-05-22)
[7] MCPAgentBench: A Real-world Task Benchmark for Evaluating LLM Agent MCP Tool Use. hf-search. https://huggingface.co/papers/2512.24565 (2026-01-21)
[8] ToolScope: Enhancing LLM Agent Tool Use through Tool Merging and Context-Aware Filtering. hf-search. https://huggingface.co/papers/2510.20036 (2026-05-08)
[9] PlanBench-XL: Evaluating Long-Horizon Planning of LLM Tool-Use Agents in Large-Scale Tool Ecosystems. hf-search. https://huggingface.co/papers/2606.22388 (2026-06-21)
[10] TaskBench: Benchmarking Large Language Models for Task Automation. web. https://proceedings.neurips.cc/paper_files/paper/2024/file/085185ea97db31ae6dcac7497616fd3e-Paper-Datasets_and_Benchmarks_Track.pdf (n.d.)
[11] AI data 2026 | Stack Overflow Developer Survey. web. https://survey.stackoverflow.co/2026/ai/data (n.d.)
[12] Planning, Creation, Usage: Benchmarking LLMs for Comprehensive Tool Utilization in Real-World Complex Scenarios. arxiv. https://arxiv.org/abs/2401.17167 (2024-06-03)
[13] From Static Templates to Dynamic Runtime Graphs: A Survey of Workflow Optimization for LLM Agents. hf-search. https://huggingface.co/papers/2603.22386 (2026-03-23)
[14] SoK: Agentic Skills -- Beyond Tool Use in LLM Agents. hf-search. https://huggingface.co/papers/2602.20867 (2026-02-24)
[15] Agent Skills for Large Language Models: Architecture, Acquisition, Security, and the Path Forward. hf-search. https://huggingface.co/papers/2602.12430 (2026-02-12)
[16] Building Effective AI Agents - Anthropic. web. https://www.anthropic.com/engineering/building-effective-agents (2024-12-19)
