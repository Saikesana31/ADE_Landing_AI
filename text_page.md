<a id='b2e70e93-0be5-46a9-8303-ee8f0c2925fa'></a>

<::logo: Galileo
Galileo
A red abstract star-like symbol with multiple arms to the left of the wordmark.::>

<a id='d41d32c3-4505-4bc9-b4f6-8a020361b6d6'></a>

v1.01

<a id='d182bff7-3a21-4b84-982d-85cdf3150f4e'></a>

Mastering
Multi-Agent Systems

Real-World Strategies for Multi-Agent Development

<a id='3128e88b-3e92-4e33-b659-9e6094958f8d'></a>

<::An image depicting three people and a dog in a modern, open-concept living space, with elements of a planetary or atomic system superimposed. On the top left is the text "galileo.ai". On the top right, the text reads "Mastering Multi-Agent Systems >) MAS <". The man on the left is laughing, wearing an orange outfit, sitting cross-legged. A woman in the center smiles, holding a large, bright glowing sphere, wearing a white sweater. A second woman on the right smiles, looking towards the center, wearing a light blue outfit. A brown and white dog sits between the man and the central woman. Several smaller glowing spheres, resembling planets or moons, orbit the central sphere, connected by faint white orbital lines. On the right side, percentages are visible: "64%", "88%", "100%", and an obscured value below it. At the bottom right, the text reads "Multi-Agent >*<" followed by an icon and then "▷ Systems". The background shows a modern interior with a stone wall and large windows looking out onto a desert-like landscape with sparse vegetation.
: image::>

<a id='8e6d7830-2113-40fa-a875-57cbb9989399'></a>

Mastering GenAI Series

<a id='dee967cf-9c70-4b65-b153-278ed96bbd7a'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='b4905501-7e34-4d84-abcc-0a13fb58ea4d'></a>

<::logo: Galileo
Galileo
A red abstract star-like symbol with four points is placed to the left of the company name.::>

<a id='34ffab03-6b4b-4c22-b18d-973d0cfac11f'></a>

<::logo: 
Chapter
02
A white square with "Chapter" in black text and "02" in large red text below it::>

<a id='420372f2-bb33-413d-8117-4d2278f2d81b'></a>

# Why Multi-Agent Systems Fail

<a id='2732bc4d-fe87-415a-8fa6-0cfbbe930aa1'></a>

Mastering Multi-Agent Systems

<a id='2d8ac280-263f-410d-bc29-4fb06acfde3c'></a>

-> galileo.ai

<!-- PAGE BREAK -->

<a id='fbacd437-f4c3-47f6-ad6c-9526d93a5b36'></a>

Chapter

<a id='556be300-dcbe-4f30-8e21-6a8594af7ebe'></a>

<::logo: [Unknown] [No readable text] [A red asterisk-like symbol with four curved arms]::>

<a id='1a307e9e-8b94-4521-ad86-cd0c421403dd'></a>

02 Why Multi-Agent Systems Fail

<a id='9d80bb60-f4ea-4c8f-a4e8-51aaad1da4fa'></a>

Multi-agent systems look great on paper. You split complex work across specialized agents, add validation layers to catch errors, and process data in parallel for speed. Everyone sees these benefits and starts building, but many of them abandon their projects in a couple of months.

<a id='72934e47-2328-45f4-a284-b02814f8ad6a'></a>

But the agents themselves aren't the problem, as individual agents work fine. What adds complexity to these systems is the coordination between them. The system becomes difficult to manage and ends up costing more.

<a id='77818b39-7c72-4bbd-807c-1fbe9c65b7fc'></a>

This chapter breaks down the complexities of building a multi-agent
system. You'll see the hidden costs of building them and get a decision
framework to evaluate whether your use case can benefit from it.

<a id='85216d8e-9bfc-4345-b74c-f9184f1a2140'></a>

34

<a id='58dcb4e6-1962-4997-a377-f6a68b80b057'></a>

Mastering Multi-Agent Systems )) MAS ((

<a id='7b1a833b-c295-4231-97b7-6c0afe3d70d4'></a>

-> galileo.ai

<!-- PAGE BREAK -->

<a id='81f6e2b1-ab06-4797-830e-ce41823902e1'></a>

Chapter 02

<a id='403b5589-5db2-432c-a3f2-106347038d15'></a>

Why Multi-Agent Systems Fail

<a id='8cbb9aba-f4c7-45a2-8bbc-3bd99a5a65f3'></a>

<::logo: Unknown

A red asterisk-like symbol with four curved arms pointing outwards from a central point::>

<a id='c66524ec-29fb-4664-9249-78e50473c0d0'></a>

Why Coordination Costs Matter

<a id='21da88e2-bceb-460b-98d9-2900eddb9736'></a>

Multi-agent systems struggle when coordination overhead exceeds the value of specialization. Two agents need one communication channel. Three agents need three channels. Four agents need six. Soon, your system becomes harder to manage than it is useful.

<a id='24572a59-0ec2-4dc7-a2a3-eaab214b7ffe'></a>

Consider the last time you worked on a
team project. How much time did you spend
on the actual work versus coordinating
with teammates? Multi-agent systems
face this same challenge, but amplified.

<a id='d8e69e01-357a-4014-b733-31287d5304b9'></a>

Here's how it plays out in practice. Imagine a web development workflow where a multi-agent system builds a dashboard:
→ Agent 1 analyzes requirements and decides on the component structure
→ Agent 2 implements the authentication flow
→ Agent 3 builds the data visualization
→ Agent 4 handles API integration

<a id='e8984a47-53e4-4269-9166-52236ba73b17'></a>

Each agent needs selective knowledge from the others. Agent 2 needs the component structure but not the full requirements analysis. Agent 4 needs auth tokens but not implementation details. This creates cascading memory challenges that single agents don't face.

<a id='54c3dee8-702d-4540-82ba-66da0fb1e167'></a>

35

<a id='28db10c2-e691-46e5-a40d-00c32c31d93a'></a>

OOO Mastering Multi-Agent Systems >> MAS (

<a id='1d55d47e-1d0a-4cf1-b4ef-f481305b0922'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='44c9751e-a5d6-479e-adb0-b6f17f54229d'></a>

Chapter 02

<a id='4ec190c1-cc66-46bc-9dc9-7e8309583b48'></a>

Why Multi-Agent Systems Fail

<a id='d4727aff-5fbe-4d4c-890c-3f6a1526867b'></a>

<::logo: Unknown

A red asterisk-like symbol with six points::>

<a id='345cde6b-067a-4daa-8d64-1677e730213d'></a>

Let's look at three high-impact scenarios that
can break multi-agent systems:

<a id='fefeb2b7-4cb4-4a2e-8576-54ced79c2f97'></a>

1.
Memory fragments across agents
Each agent maintains its own context about the project. When Agent 3 needs to understand Agent 1's component decisions, it either gets too much information (driving up costs) or too little (breaking functionality). There's no clean way to share just the relevant details.

<a id='226c0566-7ca4-45a7-909f-15be169e7551'></a>

2.
Operational costs multiply
A simple task that costs $0.10 for a single agent
might cost $1 for a multi-agent system. The extra
cost is due to all the context sharing, handoffs, and
verification required to keep agents synchronized.

<a id='da140ba0-508f-49f0-a38a-2d7012777e44'></a>

36

<a id='fc3d3905-97de-436e-92eb-b0c8f30aa74c'></a>

OOO Mastering Multi-Agent Systems )) MAS (

<a id='71bdb586-320f-4cc7-8141-ae5afab6e245'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='80665a31-5a2e-4a29-b873-8bf19e9d7eee'></a>

Chapter 02

<a id='bfe84970-d195-4da0-80d2-5bc062d9a706'></a>

Why Multi-Agent Systems Fail

<a id='34ed8967-494f-44bb-ba29-67ec8dcc9a5b'></a>

<::logo: [Unknown] [] [A red asterisk-like symbol with four curved arms]::>

<a id='ff0b1819-1e65-48ed-8c8c-574f13c0b9a1'></a>

3.

Write conflicts cascade

When agents only read data and combine findings, conflicts stay manageable. But when they modify the same system, conflicts multiply (FIGURE 2.1). Agent A creates a user profile structure. Agent B, working independently, creates a different structure. Agent C tries to reconcile both and creates a third. Your system now has three incompatible ways to represent the same user data.

<a id='feec8ecd-33c4-4d2a-a6f8-52b448dec0d1'></a>

Each interaction creates opportunities for context loss, misalignment, or conflicting decisions.

<a id='f49f571c-beed-45a9-9f81-25ee1ad5a2a9'></a>

<::Flowchart: User Profile System - Parallel Write Operations and Conflicts::>
<::Flowchart node: Create user profile system::>

<::Flowchart section: Parallel Write Operations::>
<::Flowchart node: Agent A: Creates profile { id, name, email }::>
<::Flowchart node: Agent C: Reconciliation { profileId, userName, emailAddress }::>
<::Flowchart node: Agent B: Creates profile { userId, fullName, contact }::>
<::Flowchart connection: From Agent A to Agent C, labeled "Unaware of B" (dashed line)::>
<::Flowchart connection: From Agent B to Agent C, labeled "Unaware of A" (dashed line)::>

<::Flowchart section: Cascading conflicts::>
<::Flowchart node: Three incompatible structures (with 'x' icon)::>
<::Flowchart node: Auth expects different fields (with 'x' icon)::>
<::Flowchart node: Database schema mismatched (with 'x' icon)::>
<::Flowchart node: API endpoints broken (with 'x' icon)::>

<::Flowchart node: System failure (with warning icon): Complete rewrite needed::>
<::Flowchart node: Compare to read operations (with checkmark icon):
- Reading is safe
- Can combine findings
- Writing creates conflicts::>

<::Flowchart connection: From 'Create user profile system' to 'Agent A'::>
<::Flowchart connection: From 'Create user profile system' to 'Agent B'::>
<::Flowchart connection: From 'Agent C: Reconciliation' to 'Cascading conflicts' section::>
<::Flowchart connection: From 'Cascading conflicts' section to 'System failure'::>
<::Flowchart connection: From 'System failure' to 'Compare to read operations'::>

<a id='0cd8bd9d-504b-4058-aeb7-7690f5902843'></a>

FIGURE 2.1 How write operations create cascading conflicts in multi-agent systems

<a id='6f463892-bd77-4714-bb98-e8c5c23d94da'></a>

37

<a id='c0e23e43-858d-4d8d-bef6-359b605adf42'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='20fa132e-2e66-4be7-8171-ba894c7b2c72'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='2c0b01ff-39ee-42c4-92f3-e1a7b2b4ba68'></a>

Chapter 02

<a id='19b95a0a-3f85-4d97-abc9-cdccd0ac63d7'></a>

Why Multi-Agent Systems Fail

<a id='45181be7-171c-42db-b26d-776516e77aff'></a>

<::logo: [Unknown] [None] [A red asterisk-like symbol with four thick, curved arms extending outwards from a central point]::>

<a id='9f2be039-e02a-4db6-9745-2c0403154660'></a>

When Multi-Agent Systems Actually Work

<a id='fc288f06-573a-4b1d-9d18-3788aa53e274'></a>

Successful multi-agent implementations share specific characteristics most teams overlook.

<a id='ab34b141-94fe-4290-9674-3dd1a6ed045a'></a>

[Anthropic's research system](https://example.com) is a good starting point. When tasked with analyzing the impacts of climate change, it spawns specialized agents that simultaneously investigate economic effects, environmental data, and policy implications. Each agent processes 50+ sources that a single agent would never have time to handle.

<a id='3620aa80-6e30-4c1e-a915-8ecea136df31'></a>

In this scenario, each agent works
independently, and they don't modify another's
findings. When they finish, an orchestrator
agent (explained in Chapter 3) combines
their findings into a comprehensive report.
There's minimal coordination overhead as
there's no back-and-forth coordination
during the work itself. It's just independent
analysis followed by aggregation.

<a id='1c9f05d6-ee25-4f41-9eea-4f7e98535b75'></a>

Here are three specific patterns that most successful implementations use:

<a id='3cb1f62f-7ce4-4820-83c2-95008af8eef2'></a>

1. Problems that can be parallelized

Multi-agent systems work well when problems can be split into pieces that require no communication during processing.

<a id='2106afbd-f86d-4d25-97db-14963d97e7e2'></a>

Say you have 100 quarterly reports from various companies to analyze
for investment insights. Each agent takes a report and extracts key
metrics: revenue growth, profit margins, debt ratios, and market position.
No agent needs information from another agent's reports. At the end,
you aggregate all findings into a comprehensive market analysis.

<a id='a2acfd34-be69-4bc7-8e9e-ad3778396a31'></a>

38

<a id='8be2e09d-e660-4beb-885d-957e4d811438'></a>

Mastering Multi-Agent Systems )) MAS ((

<a id='0b68ba58-70af-4e21-9151-46029918c5a4'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='256ce688-7785-43aa-84dd-04bbe0516aff'></a>

Chapter 02

<a id='97682433-1366-4aed-bf9b-34d55347f5ad'></a>

Why Multi-Agent Systems Fail

<a id='030c4d90-6cc4-4c05-a3f6-869e0804a6d5'></a>

<::logo: [Unknown] [None] [A red asterisk-like symbol with four thick, curved arms extending outwards from a central point]::>

<a id='a0948280-d82e-497b-a544-ffb3765261eb'></a>

2. Read-heavy, write-light workloads
When agents primarily consume information rather than modify shared state, coordination complexity drops dramatically. Each agent can work independently and combine results at the end.

<a id='0aa337d8-89b5-465c-bd20-eff744fa3188'></a>

Say you're tracking competitor activities across multiple channels. Agent 1 monitors news articles, Agent 2 tracks social media mentions, Agent 3 analyzes patent filings, Agent 4 watches hiring patterns. Each of your agents consumes large amounts of public data and produces intelligence reports. The final analysis combines all reports without agents needing to coordinate during data collection.

<a id='f6b08892-1206-491b-9b08-9ba08e7b66ad'></a>

3.
Explicit coordination rules
Successful implementations use deterministic orchestration with clear handoff points. Anthropic's system doesn't rely on agents figuring out how to work together. It defines exact data formats, interaction protocols, and fallback behaviors through explicit rules.

<a id='4eeca770-e2b7-4c2a-b21a-287a0b66ab2b'></a>

Consider this example from programming and software development. A code change triggers a sequence: Agent 1 runs unit tests and reports pass/fail status, Agent 2 executes integration tests if unit tests pass, Agent 3 performs security scans if integration succeeds, Agent 4 deploys to staging if all checks pass. Each step has clear success criteria, failure protocols, and rollback procedures in place.

<a id='666d390f-a444-4400-94ee-15f210336785'></a>

39

<a id='3147a1e8-d2b9-4e78-b3ac-61622c545aa3'></a>

OOO Mastering Multi-Agent Systems >> MAS (

<a id='c0a358f1-84a5-478f-9aa3-1e3330e99ade'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='710c9889-ffc3-4398-bf1a-588ee1d56491'></a>

Chapter 02

<a id='16811e2d-7a3d-4dfe-995a-4e06438cb26a'></a>

Why Multi-Agent Systems Fail

<a id='1fb24c0a-a70c-400c-953b-a974c572620a'></a>

<::logo: Unknown
No readable text
A red asterisk-like symbol with five arms, each arm consisting of two curved lines that meet at a point, arranged in a circular pattern::>

<a id='ca0bd26e-d46b-47b9-a53b-c070f9c64f4c'></a>

Consider this example from programming and software development. A code change triggers a sequence: Agent 1 runs unit tests and reports pass/fail status, Agent 2 executes integration tests if unit tests pass, Agent 3 performs security scans if integration succeeds, Agent 4 deploys to staging if all checks pass. Each step has clear success criteria, failure protocols, and rollback procedures in place.

<a id='8ef1153f-465f-40a3-8c95-0bb2c9e12785'></a>

Here's a checklist to decide if your use case benefits from a multi-agent setup:

option Can you break down the work into completely independent tasks?: [ ]

option Do agents primarily read and analyze rather than write and modify?: [ ]

option Can results be combined mechanically (concatenation, voting, averaging)?: [ ]

option Is parallel processing speed worth a 2- to 5-fold cost increase?: [ ]

option Can one agent failing be isolated from others?: [ ]

<a id='e251d8e6-7166-412d-bd1d-706c5e9dd1ec'></a>

Use this checklist to help you determine whether your current problem aligns with multi-agent patterns. Before building any multi-agent system, ask: Will this approach still make sense six months from now?

<a id='dd5c0e12-98a7-4b90-877c-5be287037826'></a>

This question matters because you're choosing an architecture that needs to work
as models rapidly improve over time. The history of AI suggests that complex
workarounds often become unnecessary overhead when better models emerge.

<a id='37c55498-792e-4287-b797-69f31db1274f'></a>

40

<a id='2f2481a4-191d-4925-b99f-2c1d47401f57'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='9428e145-db2b-4a2d-bd85-b8805962d50b'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='9a048f2b-73d2-4d9b-ba53-233e1bef53e7'></a>

Chapter 02

<a id='bf7ba7cb-b7d2-4791-9c1e-2fa0fc33e1bd'></a>

Why Multi-Agent Systems Fail

<a id='c664ac68-9f80-4be9-99bc-c176ea7eba64'></a>

<::logo: Unknown

A red asterisk-like symbol with four curved arms pointing outwards from a central point::>

<a id='1eaa44c2-5bf7-4ad3-992a-9c8027181240'></a>

The Model Evolution Challenge

<a id='f373da32-68e3-467d-bf8a-9e49b7b1e7ca'></a>

Rich Sutton's Bitter Lesson teaches us that general methods using more computation ultimately win over specialized structures. This principle now collides with multi-agent system design in ways that should make you pause.

<a id='918f1349-54e5-490f-83d0-0523625de77e'></a>

Consider what you're actually doing with multi-agent systems: adding structure to compensate for current model limitations.

*   Can't get your model to handle complex reasoning in one pass? Split it into specialist agents.
*   Is the context window too small? Distribute the load.
*   Is the tool calling unreliable? Create dedicated tool-use agents

<a id='cac4affd-956f-4711-aa80-29a44687eb63'></a>

What happens when these limitations disappear?

<a id='5b54433d-8cba-4e48-8cda-68d0ee3a4cad'></a>

Think About Your Current Project.

What model limitations are you working around with
your multi-agent architecture? Context windows?
Reasoning capability? Tool use reliability? Write
these down. They're your obsolescence risks.

<a id='21f52294-ce12-4434-af50-ea6516de8a43'></a>

Teams that built complex orchestration layers for GPT-4 found them
unnecessary with GPT-5. Multi-step reasoning chains designed
for Claude 3 became single prompts with Claude 4. The structure
added to work around limitations became the limitation itself.

<a id='58090eec-28f9-474f-af28-1becb0a42213'></a>

41

<a id='1a2755bf-5671-4ab6-8228-6e16db747df1'></a>

(OOO Mastering Multi-Agent Systems >> MAS (

<a id='7a4ac749-790d-49e2-a699-3af89c024e47'></a>

galileo.ai

<!-- PAGE BREAK -->

<a id='6891e189-1ab0-43d1-9f49-59ea81720f91'></a>

Chapter 02

<a id='1e63e421-dd40-47a6-a46b-99b70a9fa13d'></a>

Why Multi-Agent Systems Fail

<a id='e24faeb6-5786-4520-a7e6-d9deed279ed9'></a>

<::logo: [Unknown] [] [A red asterisk-like symbol with four curved arms]::>

<a id='f9d25e87-4095-425c-aac6-f23512f51ec2'></a>

Boris from Anthropic's Claude Code team gets this. Instead of building elaborate multi-agent systems, he focuses on leveraging model improvements directly. The recent success of single-agent systems beating multi-agent baselines validates this philosophy. Our agent leaderboard shows this pattern clearly: newer models consistently outperform older multi-agent systems while being faster and more cost-effective.

<a id='e4b6a38f-b8e5-4fd7-92a8-93e6601e697e'></a>

This pattern repeats across AI development. You might spend months building a complex multi-agent system only to find that a newer model can handle the same work in a single call. The distributed system you worked so hard to build becomes unnecessary overhead.

<a id='05eb091d-cc6c-48cd-87b6-f19adbc1953d'></a>

The smarter approach is to follow Hyung Won Chung's philosophy:

<a id='af0bba73-d5cf-4e0d-80c3-7f8fcd9c0a12'></a>

Add minimal structure:
Instead of building five specialized agents (requirements, authentication,
database, API, frontend), start with two: one for backend logic, one for frontend.
You can always split further if needed, but merging is harder than splitting.

<a id='c7c45523-8d89-4e67-a028-18a88143033c'></a>

Plan for removal

Write your orchestration code in a separate module that you can delete
entirely later. When a better model arrives, you should be able to delete
the orchestration layerfile and call the underlying functions directly.

<a id='a31ad69f-17d0-4c8b-b020-1033850cb7d5'></a>

## Make boundaries collapsible

Structure your agents so their logic can merge into a single prompt. If Agent A does research and Agent B writes summaries, write them so you can combine both into one "research and summarize" agent later.

<a id='110c492d-1a3d-4dad-8841-0976c68a14a4'></a>

Separate orchestration from business logic
Your authentication logic should work the same whether it's called by an orchestrator or directly. Keep the business logic separate from the orchestration.

<a id='bb7abf57-9e59-49f3-a74e-79a76b8ee0a8'></a>

If you're splitting tasks across agents because the model can't
handle complexity, waiting a few months for a better model might be
more effective than building infrastructure you'll have to scrap.

<a id='e61182b1-842d-40dc-9699-1d8ce9afa532'></a>

<::logo: Unknown
42
The numbers "42" are prominently displayed in red, set against a light gray square background.::>

<a id='79fc5086-f93f-4a28-9c18-6ede8fbe11e8'></a>

Abstract logo Mastering Multi-Agent Systems )) MAS (

<a id='4571d9b8-69fb-4c4b-9a82-b0f9b4d39c07'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='9a327a2b-16b9-4f90-86c4-f026bf3c503a'></a>

Chapter 02

<a id='5e280ff7-ff02-4f5c-9668-352a1e6cebf6'></a>

Why Multi-Agent Systems Fail

<a id='b3b4fa2c-6fde-4a50-ace7-9d494417587b'></a>

<::logo: [Unknown] [] [A red asterisk-like symbol with four curved arms]::>

<a id='b7989d73-1843-47ff-8c99-22a1301737a8'></a>

What Frameworks Actually Deliver

<a id='69f0cb08-589a-407a-b00a-61f0cdc4dfb7'></a>

These days, we have many frameworks
for building agents. They tackle the same
core challenge: how do you coordinate
multiple agents without losing critical
context? The approaches vary, but none
solve the fundamental problem.

<a id='4e3c1af5-7504-4326-abe0-c4070c36eac6'></a>

CrewAI provides structured role assignments
and basic handoff protocols. You define agents
with specific responsibilities, and CrewAI
manages the execution flow. However, context
sharing remains a persistent issue. When Agent
A finishes analyzing the requirements and
hands them off to Agent B for implementation,
CrewAI passes along whatever you have
explicitly configured. Miss a crucial detail in
your context template, and Agent B works with
incomplete information.

<a id='0a3d0e75-fe06-46fe-a573-d8ceed8d8d20'></a>

LangGraph gives you complete control over
agent interactions through state machine
design: You can define exactly how agents
communicate, what data they share, and
when handoffs occur. This flexibility comes
with complexity. You're responsible for
designing the state transitions, managing the
context flow, and handling failure scenarios.
LangGraph provides the pipes, but you have
to figure out what flows through them.

<a id='6e1fdfce-a351-49c4-9ae7-4a8988d1bcfc'></a>

The core problem remains unsolved:
efficient context passing between agents.
Current approaches either share everything
(expensive and slow) or share summaries
(losing critical details). No framework has
solved selective, semantic context transfer
that maintains accuracy while minimizing
overhead. Refer to TABLE 2.1 to see a
comparison of different agentic frameworks.

<a id='7aa99270-14e4-49be-a2f6-db8db53a1ae9'></a>

<table id="11-1">
<tr><td id="11-2">Framework</td><td id="11-3">Strength</td><td id="11-4">Limitation</td></tr>
<tr><td id="11-5">CrewAI</td><td id="11-6">Simple role-based setup</td><td id="11-7">Limited context control</td></tr>
<tr><td id="11-8">LangGraph</td><td id="11-9">Full state management</td><td id="11-a">High complexity overhead</td></tr>
<tr><td id="11-b">Swarm</td><td id="11-c">Lightweight coordination</td><td id="11-d">Manual context passing</td></tr>
</table>

<a id='2c7100bb-3397-414a-a0f1-b8aa863bff62'></a>

TABLE 2.1 Comparison of different agentic frameworks

<a id='78deaabb-e5f4-4948-a72d-5f11ba18743a'></a>

43

<a id='6ce9bd37-2e51-4f29-acca-977ece1bcf23'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='a22fd242-c80b-4a83-90b1-2c7f11c7c3cb'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='6d0400a7-bf63-44b0-ad3a-e09f79aaeb74'></a>

Chapter 02

<a id='865f92d0-b02a-4ba6-afda-532a4f0044df'></a>

Why Multi-Agent Systems Fail

<a id='85d1db7c-0f34-485f-90d9-037bc66712af'></a>

<::logo: [Unknown] [None] [A red asterisk-like symbol with four thick, curved arms extending outwards from a central point]::>

<a id='f6a12984-b9bd-48a4-9d7e-77255138adee'></a>

Consider this workflow: Agent A analyzes a 50-page requirements document
and identifies 12 key components. Agent B needs to implement authentication
based on those requirements. How much context does Agent B actually need?

<a id='075a8f76-516e-4c82-9504-b4075b75bf81'></a>

**Option 1: Share everything:**
Agent B gets the full 50-page analysis plus Agent A's complete reasoning chain. This works but costs 10x more in API calls and processing time.

<a id='23f9032c-be80-4019-a2e9-dca4a71f6c32'></a>

Option 2: Share summaries:

Agent B gets a condensed version of the key authentication
requirements. This costs less but risks losing the
nuanced decisions that affect implementation.

<a id='c2679134-a720-449a-8957-32f7df0cc463'></a>

Option 3: Selective sharing:
Agent B gets precisely the authentication-relevant
context with enough surrounding detail to make informed
decisions. No framework handles this automatically.

<a id='23291c67-e3d3-4bb5-bc74-7d882de09b44'></a>

While frameworks can't solve the context efficiency problem, they do handle the mechanics that would otherwise require significant custom development. However, they can't solve the fundamental coordination economics that make most multi-agent systems too expensive to run.

<a id='40cef57a-e395-4535-a6f5-73a21aeff691'></a>

44

<a id='58583c26-062b-4661-8d5c-f8d6f33f1080'></a>

Mastering Multi-Agent Systems )) MAS ((

<a id='2cda4c83-0f33-48aa-8dfd-b757e32621dd'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='b5b57f17-3f37-4e2f-a292-577da7417669'></a>

Chapter 02

<a id='39d79039-14c3-4e59-b065-948a697f046f'></a>

Why Multi-Agent Systems Fail

<a id='9af2e46b-6a7b-4d90-a99f-4b2043f3bc15'></a>

<::logo: [Unknown] [No readable text] [A red, star-like symbol with curved arms]::>

<a id='ff289da7-29b7-42a5-b531-200748e1ecd9'></a>

The Decision Framework

<a id='b6aa2a21-0812-4f5e-8ad2-53393f7049d8'></a>

Before you build a multi-agent system,
walk through these questions in order:

<a id='3585e05d-ff57-43e5-822a-a2279ccc2d86'></a>

1.
Can better prompt engineering solve this?
In 80% of cases, a well-crafted single agent with good context management beats a multi-agent system. Don't split up complexity unless you haven't tried to simplify it.

<a id='b808b47d-32ea-494b-9b76-e404a472a029'></a>

Say you want code review automation. One agent with a comprehensive prompt handles syntax checking, logic review, and security scanning faster than three separate agents. The single agent maintains context about the entire codebase while reviewing. Multiple agents would need to share that context repeatedly, which would slow down the process and increase costs without improving quality.

<a id='cdf3cf7f-9484-49e4-8aca-9208188db844'></a>

2.

Are your subtasks genuinely independent?
Real independence means zero shared state during processing. If Agent B needs Agent A's output to function, you have sequential tasks with extra overhead.

<a id='328de17a-a62a-4b2e-91bd-5cd4d9da9f4e'></a>

Say you're analyzing 100 quarterly earnings reports. Each agent
processes one company's financials independently. Company A's
analysis doesn't affect Company B's. At the end, you combine findings.
This works because subtasks are genuinely independent.

<a id='7c7da826-32ca-4cca-9370-358bb5ab68fd'></a>

But if you're writing a report where Section 2 analyzes trends from Section 1, and Section 3 builds recommendations from Section 2, you've created dependencies. You're running sequential tasks with coordination overhead, not parallel work.

<a id='9a650d1b-d435-4b36-bdc7-5f66897665e5'></a>

45

<a id='80639e02-65f1-4946-a6d1-f36553926c52'></a>

OOO Mastering Multi-Agent Systems >> MAS (

<a id='57d12fa3-0360-4254-bdb0-25192b7b5f1e'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='b1a85f1a-2818-4034-935a-7fc5ae9aa14e'></a>

Chapter 02

<a id='aaa93c98-c00c-499e-a9a3-b3429ce803f5'></a>

Why Multi-Agent Systems Fail

<a id='e5b8c9ea-2f9c-4226-91b1-a290c61f31eb'></a>

<::logo: [Unknown] [No readable text] A red asterisk-like symbol with four curved arms pointing outwards from a central point.::>

<a id='10e04934-e7cf-42b6-aad6-1e83d5280c3d'></a>

3. Can you afford the cost increase?
Between coordination overhead, duplicate context, and retry logic, expect to pay 2-5x more than single agents.

<a id='70ee3bba-bb98-4482-9004-c37910d29e8a'></a>

The extra cost comes from agents needing overlapping context to work together. Each handoff requires reconstructing relevant information, and verification steps multiply as agents check each other's work.

<a id='cfc8e651-7ac4-4b94-b1a6-2c81d1d85a2d'></a>

4. Is your latency tolerance measured in seconds?
Each agent handoff adds 100-500ms. Five agents can add 2+ seconds to response time.

<a id='0ea0dbae-4f46-42e8-8275-27c002e43661'></a>

If you're building real-time trading systems, you need responses under
100ms. If you're handling live chat, users expect replies within 1-2
seconds. The extra latency makes multi-agent systems unusable here.

<a id='bec3b4f2-bb8d-4daf-9e51-d3e0baba1c27'></a>

5. Do you have debugging infrastructure?
When multi-agent systems break, you need to trace through multiple
execution paths, shared state changes, and inter-agent communication logs.

<a id='4c590577-79a2-41df-8929-1a2aa0d6b914'></a>

When your single agent fails on a database query, you check one error log. When the same failure occurs in a multi-agent system, you may need to investigate the query agent, validation agent, retry logic, and coordinator by piecing together logs from four different components.

<a id='71753f84-37dc-4f83-87da-a0bd3d78f80b'></a>

Debugging becomes exponentially more complex in production
because failures can originate from any agent, any interaction between
agents, or timing issues in the coordination layer. Without specialized
tooling, you'll spend more time debugging than building features.

<a id='e8d76f4d-2747-4cf2-9495-c59167fba603'></a>

46

<a id='8dbe21ef-a0fe-4ad6-a709-c92c50331dbc'></a>

OOO Mastering Multi-Agent Systems >> MAS (

<a id='21e354a0-3de3-4af5-b7e2-2ac0a2d012a8'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='56526ab2-b072-4fc4-a9cb-c77440a778d8'></a>

Chapter 02

<a id='59ca42d9-f279-4532-8098-d5e6488ac53e'></a>

Why Multi-Agent Systems Fail

<a id='f781ff61-3d9f-427c-8fc8-f6587b5ddc7f'></a>

<::logo: [Unknown] [] [A red asterisk-like symbol with four curved arms]::>

<a id='3b0980e1-5b7d-4186-8665-1a41358fc8b5'></a>

<table id="15-1">
<tr><td id="15-2">Aspect</td><td id="15-3">Single Agent</td><td id="15-4">Multi-Agent</td></tr>
<tr><td id="15-5">Context management</td><td id="15-6">Continuous, unified context maintained throughout</td><td id="15-7">Context fragmented across agents, requires synchronization</td></tr>
<tr><td id="15-8">Error propagation</td><td id="15-9">Errors contained, can self-correct</td><td id="15-a">Errors compound: 90% accuracy per agent -&gt; 59% for 5 agents</td></tr>
<tr><td id="15-b">Operational cost</td><td id="15-c">Baseline cost (1x)</td><td id="15-d">5-10x higher due to coordination and context sharing</td></tr>
<tr><td id="15-e">Latency</td><td id="15-f">Single processing chain</td><td id="15-g">Multiple handoffs add 50-200ms per agent interaction</td></tr>
<tr><td id="15-h">Best use cases</td><td id="15-i">Code generation, content writing, complex reasoning</td><td id="15-j">Parallel research, independent analysis, monitoring</td></tr>
<tr><td id="15-k">Debugging complexity</td><td id="15-l">Linear trace through single chain</td><td id="15-m">Exponential complexity with agent interactions</td></tr>
<tr><td id="15-n">Token efficiency</td><td id="15-o">Optimal - single context window</td><td id="15-p">Wasteful - redundant context across agents</td></tr>
<tr><td id="15-q">Scalability</td><td id="15-r">Vertical (better models)</td><td id="15-s">Horizontal (more agents) but with diminishing returns</td></tr>
</table>

<a id='9b812ba6-5f30-4130-bd94-9011f161b70e'></a>

FIGURE 2.2 Single vs Multi-agent systems across different dimensions

<a id='f40641b9-4e9e-468c-91a4-b2719fe907e3'></a>

You can see the pattern in FIGURE 2.2. Read-heavy tasks work better than write-heavy tasks when you're using multi-agent systems. When your agents can work independently and combine findings, multi-agent approaches work well. When your agents need to build something together, coordination costs usually outweigh benefits.

<a id='006fe300-e551-40cc-8362-b42561463594'></a>

Let's look at a concrete example to see how these costs play out in practice.

<a id='f5d40ea6-3ab3-4964-a5fb-bcbbcfdd8059'></a>

47

<a id='eef708e1-cb9b-4e30-b217-bfb63c04d950'></a>

Mastering Multi-Agent Systems >> MAS (

<a id='d5a015c2-591f-40c8-a30c-9f2bac7782ee'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='b9b23d82-e9df-4dca-926a-dacdae38d6b7'></a>

Chapter 02

<a id='8ed793a0-70d6-4844-b046-c370f302cc5d'></a>

Why Multi-Agent Systems Fail

<a id='285ee7cc-143c-4988-92a4-9fa2cc239fe0'></a>

<::logo: Unknown

A red asterisk-like symbol with curved arms, radiating from a central point, on a white background.::>

<a id='6860953e-77a0-4103-b5e2-48689fb5b622'></a>

The Cost Reality Check
Consider a customer support system and how the economics work out:

<a id='11089e19-614c-423f-b810-0534ea7024f2'></a>

# Single-Agent Approach

-> One agent reads the ticket, searches documentation, checks account status, and crafts a response
-> Time: 2 seconds
-> Cost: $0.05
-> Debugging: Straightforward trace through one decision path

<a id='e6342a9f-87bd-4853-8658-4e128cab2f57'></a>

Multi-Agent Approach

*   Triage agent categorizes (0.5s, $0.08)
*   Research agent searches documentation (1s, $0.10)
*   Account agent checks status (0.8s, $0.08)
*   Response agent crafts reply (1s, $0.10)
*   Orchestrator combines everything (0.5s, $0.04)
*   Time: 3.8 seconds
*   Cost: $0.40
*   Debugging: Five different failure points, 10 potential interaction bugs

<a id='39fb4244-401d-42dc-8ce6-539e86be6b33'></a>

The multi-agent system costs 8x more, takes nearly twice as long, and creates exponentially more ways to fail. The coordination overhead consumes more resources than the actual work. Unless you're handling millions of tickets where parallelization provides massive scale benefits, the single agent wins.

<a id='511cc688-2642-4c58-bfc0-4b5e44c8891e'></a>

48

<a id='4fa5bb4b-93c6-4c7b-92c5-cb5d34623a6e'></a>

OOO Mastering Multi-Agent Systems >> MAS (

<a id='03a484e4-8cd3-448f-a40f-783af762e4d2'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='b0569756-04ed-4a99-84a6-c11c5cb5cbe0'></a>

Chapter 02

<a id='a1582a56-1b74-41cc-954b-78262a918c9a'></a>

Why Multi-Agent Systems Fail

<a id='eb1b37a1-d44f-4a47-9109-e22e45fd1520'></a>

<::logo: [Unknown] [] [A red star-like symbol with four points, each point resembling a stylized arrow or 'V' shape, is centrally positioned against a white background.]::>

<a id='d0f599b8-81e2-4b9f-b29a-ee9514cac312'></a>

This pattern holds across domains. Unless you're processing at a massive scale where parallelization provides exponential benefits, a single agent typically wins on cost, speed, and reliability. Most problems that seem like they need multiple agents actually need better prompt engineering and context management for a single agent.

<a id='a532db43-fc7d-4ba1-815f-6209b5f1c917'></a>

EXERCISE

Think about a current AI workflow in your organization that's not performing well. Map it through the decision framework above:

1. Write down the specific problem: What exactly isn't working?
2. Apply the 5-question framework: Can prompt engineering fix this? Are subtasks independent? Can you afford a 2-5x cost increase? Is latency tolerance in seconds? Do you have debugging infrastructure?
3. Calculate the economics: If your current solution costs $X, are you willing to pay $2-5X for potential improvements?
4. Identify your constraints: What matters most - cost, speed, accuracy, or reliability?

See if your "multi-agent problem" is actually a single-agent optimization problem you can tackle easily.

<a id='bfd4cadc-94d0-4aff-b58d-2e9c43737c07'></a>

<::logo: Undetermined
49
The number "49" is displayed in a prominent red font, suggesting a possible brand or product identifier::>

<a id='60494f73-aec0-4ff5-96a4-81d08fde527c'></a>

Mastering Multi-Agent Systems )) MAS ((

<a id='e10ed6cd-e4de-421f-bdd5-266d82f423da'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='8d2657eb-7c94-4817-8e56-555f9fbce7f1'></a>

Chapter 02

<a id='b3636a82-b498-4740-a2ae-49d198df8dfb'></a>

Why Multi-Agent Systems Fail

<a id='277b24cf-ae6c-4641-9418-0361d638b101'></a>

<::logo: [Unknown] [] [A red asterisk-like symbol with four curved arms]::>

<a id='542c98f2-3463-4ed5-912a-dfb2fee3aab6'></a>

Building Visibility Into Your System

<a id='fff66ab1-daea-42e4-8faa-d3122878b76b'></a>

Even after you've identified a legitimate
use case for multi-agent systems, you
might face another challenge: a lack
of visibility into agent failures.

<a id='5eb3b87d-00be-40b4-8314-0acdfd4763e0'></a>

Traditional LLM evaluation is not effective for
debugging agents as they can take completely
different paths to reach the same goal. Your
research agent might retrieve papers in
different orders, make varying numbers of

<a id='f1818fff-cdf2-4f16-a79d-b7c63cd7910e'></a>

tool calls, or explore alternative approaches
while still producing the same quality output.

<a id='e5619914-ad19-4f1f-896b-c37df079740f'></a>

This makes measurement more complex than checking if the final answer matches your expected output. You need to understand what happened at each decision point, why the agent chose specific tools, and how context influenced those choices. Without this visibility, you're optimizing in the dark.

<a id='29f83f37-0909-4bdf-9196-42737acc4a37'></a>

Galileo addresses this by tracking three distinct levels:

<a id='cd68d159-ac48-426c-bf5b-b1ff7c730747'></a>

# 1.

**Session Level:**
Did it complete
the task?

-> [Action Completion](link_to_completion)
tracks whether all user
goals were met

-> [Action Advancement](link_to_advancement)
measures progress
toward at least one goal

<a id='97f79cfb-4b67-4549-9aa9-d1a65f804ef5'></a>

2.

Step Level:
Were individual
decisions correct?

→ Tool Selection Quality
measures whether the right
tools were chosen with
the correct parameters

→ Context Adherence
checks if responses
used provided context
instead of hallucinating.

<a id='058fd27e-cd55-4aee-9737-43547972352a'></a>

3.

System Level:
What patterns exist across sessions?

-> Tracks the number of errors
-> Identifies the latency of API calls
-> Monitors token consumption patterns and costs
-> Detects agents stuck in repetitive loops due to coordination issues

<a id='dd699e9a-c323-4588-9a36-0ab1d61122a6'></a>

50

<a id='9c2a9800-ab97-49b2-85f1-8588d59c32dc'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='22fbc4ba-6070-4a26-8e02-2f76c2c5fb26'></a>

-> galileo.ai

<!-- PAGE BREAK -->

<a id='74913534-ce90-4663-9e39-58c5bb1517cf'></a>

Chapter 02

<a id='dac7eecd-4ce3-4c7f-9b0f-331565b78572'></a>

Why Multi-Agent Systems Fail

<a id='25977f8c-0501-4aeb-b832-d3df72d280d1'></a>

<::logo: Brand: Unknown
Visuals: A red asterisk-like symbol with four stylized, curved arms pointing outwards from a central point.::>

<a id='e916afdb-09e8-4bb6-a2a2-f555fc61ec4a'></a>

## Process for Continuous Improvement

Reliable multi-agent systems aren't built in one pass. They're refined through systematic observation and targeted fixes. This four-step process helps you identify exactly where coordination breaks down and validate each improvement.

<a id='78f599b0-d238-421f-9581-bedb3e139ae0'></a>

1. Establish a Measurement Framework

<::
chart: A visual representation of a banking conversation and task completion status.

**Sample banking conversation**

[Chat bubble - User]: I need to dispute a fraudulent $87.32 charge, transfer $4,000, set up text alerts over $20, schedule $750 monthly rent for Jake, order a new debit card shipped express, and pull a 45-day statement.

[Chat bubble - Agent]: Certainly! To get started I'll need:
• last 4 digits of the affected card
• your shipping address for the replacement card
• which account to move the $4,000 from
• Jake's account details.
Once I have those, I can process everything.

[Chat bubble - User]: Card ending 4321, ship to 123 Maple St, Boston 02118. Move the funds from High-Yield Savings to Main Checking. Jake's routing 111000025, account 987654321.

[Chat bubble - Agent]: Great - I've disputed the charge, transferred $4,000, and generated your 45-day statement (sent to your email).
I've submitted a ticket for the replacement card; you'll see shipping details soon.

[Chat bubble - User]: Thanks! Can you confirm the dispute is filed and the transfer shows in checking? Also, please set those text alerts and the monthly rent transfer before I travel.

[Chat bubble - Agent]: Confirmed: the dispute is filed and the $4,000 is now in Checking.
Unfortunately card-replacement express shipping is still pending.
At the moment, text alerts and scheduled payments must be set up through phone support - I can't configure them here, sorry!

**Task Completion**
option Process $4,000 transfer: [x]
option File dispute for $87.32: [x]
option Generate 45-day statement: [x]
option Set text alerts > $20: [ ]
option Order express replacement card: [ ]
option Schedule automatic $750 rent transfer: [ ]

**Action Completion Score**
0%
Because any missing action sets the score to 0%,
the agent's failure to configure text alerts,
order the card with express shipping, and schedule
the rent transfer results in a total Action Completion
score of 0%.
::>

<a id='f04d42fa-59a5-426b-87d5-f031f7f58c7c'></a>

FIGURE 2.3 Action Completion Scoring

<a id='bc99b66b-3df9-48bb-a5c9-c26b980322ca'></a>

As part of session-level analysis, use Action Completion (FIGURE 2.3)
and Action Advancement to measure overall goal achievement. The
Trace View lets you replay entire sessions to see how your agents
work together to accomplish user objectives. Each trace shows the
complete execution path and agent interactions at every step.

<a id='10f606bd-44b3-4583-9a7a-2b0481204e3d'></a>

51

<a id='6a86b9b3-8729-4c48-8021-e98a0330deda'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='20455275-6df4-49b2-a6cc-bd601718df3c'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='3092b026-f57e-436c-a065-7f76b090f861'></a>

Chapter 02

<a id='793a7d04-3418-4fd6-9a53-fccbe0b85c82'></a>

Why Multi-Agent Systems Fail

<a id='da743444-6c4d-4d72-98af-d356f6cd8847'></a>

<::logo: Unknown
No readable text
A red asterisk-like symbol with five arms, each arm consisting of two curved lines that meet at a point, arranged in a circular pattern::>

<a id='6a2a6649-6ae2-4b28-81fa-f0d4e37017f4'></a>

<::Evaluating AI Agents
: flowchart
User Input
-> LLM Planner
LLM Planner
-> Develops plans

From Develops plans, a dotted arrow points up to the question: "Were the correct tools and arguments selected?"

Develops plans forks into three paths, represented by wavy dotted lines, leading to:
- Tool A
- Tool B
- Tool C

From Tools A, B, C, a dotted arrow points up to the question: "Did the tool encounter errors?"

The paths from Tools A, B, C converge and lead to Final Action.

From Final Action, a dotted arrow points up to the question: "Did the tool selection meet user goals with right parameter values?"

A dotted line from the right side of the Final Action box goes down and then left, connecting to a block labeled "Tool response sent to planner".

Below the main flow, there is text: "Repeat until final action".

"Tool response sent to planner" has a dotted arrow that loops back to the LLM Planner.
::>

<a id='e9d021f0-8164-42e0-995d-121d3c06d2b8'></a>

FIGURE 2.4 Tool Selection Scoring

<a id='556084d4-7674-4544-a5de-436f64cf7e54'></a>

As part of step-level analysis, apply Tool Selection Quality (FIGURE 2.4)
and Context Adherence to evaluate individual agent decisions. The
Graph View reveals coordination patterns, showing where agents fail to
communicate properly or choose the wrong approach. Click any node to
see the exact information available to that agent at that decision point.

<a id='f876fe71-3430-475d-a044-f0a7bcf53b18'></a>

You can use Log Stream Insights for real-time monitoring. It provides instant visibility into multi-agent performance with intelligent pattern detection.
Set up custom filters to monitor specific coordination events, such as when agents fail to share information or when handoffs break down.

<a id='20b89051-7b55-4adb-b274-28eb4bed2ae6'></a>

52

<a id='a1852ede-fa7e-4641-bdb4-19d1a16abb8e'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='931af53f-1b4d-413b-b39e-028108acf642'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='618de128-cec8-4d0b-95cc-0cdeb5d2e21b'></a>

Chapter 02

<a id='385aeebc-5a70-4ae3-a37e-af6c04435827'></a>

Why Multi-Agent Systems Fail

<a id='ab14032b-bbf8-486c-96d1-d93626f222f4'></a>

<::logo: [Unknown] [None] [A red asterisk-like symbol with four thick, curved arms extending outwards from a central point]::>

<a id='af2c4608-2588-485e-bd9d-1b8ec677f757'></a>

2. Implement an Iterative Improvement Process
Once you've established baseline metrics, use
them to spot problems and test solutions.

<a id='097cad33-46bc-4fd4-9a6d-d005e7b7f952'></a>

Identify patterns: Monitor metrics over time using the Latency Chart to spot performance degradation as your system scales. Correlate latency spikes with specific agent interactions or coordination bottlenecks. Galileo's automated insights highlight which agent handoffs consistently cause failures or slowdowns.

<a id='95caa76c-2666-42ff-9a63-28c266ff0707'></a>

Visualize agent behavior: Compare different execution paths for the same task using Graph View. See how agent coordination strategies lead to different routes and identify which approaches work most efficiently. Export these visualizations for team reviews and documentation.

<a id='f7af7fc6-1688-4046-881e-6ad47ddd0964'></a>

Test variations: Create different versions of your
agent coordination strategies and use A/B testing to
compare performance. The Trace View allows side-by-
side comparison of different multi-agent approaches,
showing exactly where behaviors diverge.

<a id='34a5cd7c-3ea7-4d18-8d16-62e9c66e107e'></a>

Benchmark against baselines: Compare your multi-agent system against Galileo's evaluation datasets and industry benchmarks. The platform provides pre-built test suites for common agent coordination patterns like parallel processing, sequential workflows, and hierarchical delegation.

<a id='6b080035-c0e1-49ba-b253-f854cae5bd85'></a>

53

<a id='df001fde-93e2-4288-92b7-66c59ba9d73d'></a>

Logo Mastering Multi-Agent Systems )) MAS (

<a id='fbbdfa2b-fe4c-4b97-83c2-2948974d4075'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='4fe3fc61-ece6-4b34-8f54-157e91a718c8'></a>

Chapter 02

<a id='bd04e3c9-e789-4eb4-a027-5802e5250502'></a>

Why Multi-Agent Systems Fail

<a id='1550d485-d4e9-4200-bde1-b9363b0b9389'></a>

<::logo: [Unknown] [None] [A red star-like symbol with curved points, resembling an asterisk or a stylized flower]::>

<a id='ff3bad48-a70f-4e5a-9513-5fd63baaecff'></a>

3. Apply Specific Optimization Strategies

<a id='97fada76-9031-4967-a43e-5a1caf0f7915'></a>

Multi-Agent Telecom Chatbot / Log Stream: prod / Session: Telecom Agent - 2025-09-25 16:
Share
<::A tab bar with three options: Messages, Latency, and Trace graph. Messages is selected.:tab_bar::>
Session 2 of 6 Configure Metrics

option Condense steps: [ ]
Type: All Q
Tool Selection Quality Supervisor
Input
JSON
Metrics Parameters Insights
Telecom Agent - 2025-09-25 16:24:37
Agent Quality
<::A tree-like structure showing the flow of agent interactions with associated percentages:
Trace 80%
Supervisor 33%
transfer_to_plan-advisor-agent
Plan Advisor Agent 67%
pinecone_retrieval
pinecone_retrieval
Plan Advisor Agent 100%
"content": "
You are a supervisor managing a team of specialized telecom
service agents at ConnectTel.

Route customer queries to the appropriate agent based on their
needs:
  - Billing Account Agent: Bill inquiries, payment issues, usage
    tracking, account balance, charges, credit card information, credit score,
    etc.
  - Technical Support Agent: Device troubleshooting, connectivity
    issues, configuration help, resets
  - Plan Advisor Agent: Plan recommendations, upgrades, comparing
    plans, finding savings

Guidelines:
  - Route queries to the most appropriate specialist agent
  - For complex issues spanning multiple areas, coordinate between
    agents
  - Be helpful and empathetic to customer concerns
  - If unsure, ask clarifying questions before routing
  - For general greetings, respond warmly before asking how you
    can help
  - If a query doesn't fit any agent's expertise, politely explain
    our service limitations.
",
"role": "system"
pinecone_retrieval
pinecone_retrieval
Plan Advisor Agent 100%
Supervisor 100%
Trace 100%
Supervisor 100%
{ "content": "check my usage and suggest me how to select the plan", "role": "user" }
:agent_interaction_flow::>
Action Completion Pending...
Tool Selection Quality 33%
Generated Reasoning
The user's query has two parts: 'check my usage'
(which pertains to billing/account information) and
'suggest me how to select the plan' (which is for
the plan advisor). The bot chose to transfer the
conversation to the plan-advisor-agent. However,
the user's query also concerns billing/account
usage, which falls under the billing-account-
Auto-improve Metric
System Metrics
Cost $0.0007
Latency 1.48 sec
Num Input Tokens 279
Num Output Tokens 14
Num Total Tokens 293

<a id='a08b8ba2-37ae-4772-8e67-40fc197c9f68'></a>

FIGURE 2.5 Trace View

<a id='fee619a8-2325-4005-a214-937d8926af3c'></a>

Use the Trace View's collapsible interface (FIGURE 2.5)
to navigate through nested agent calls and interactions.
Each trace shows the complete execution path at that
point, which makes it easy to identify where agents fail to
communicate properly or where coordination breaks down.

<a id='8d96d13d-a01c-4850-b0f6-994cb99ff076'></a>

54

<a id='c9fb5a57-169e-445b-871a-bab269fdcc30'></a>

Abstract logo Mastering Multi-Agent Systems )) MAS (

<a id='37523887-98bc-43f8-8536-1e96c8f4ba39'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='26c5f2bb-38cd-4309-94d2-22ab70bde0ec'></a>

Chapter 02

<a id='2699681c-5a14-482f-bc67-a64edde13896'></a>

Why Multi-Agent Systems Fail

<a id='bd8e77fe-a790-4ce1-878c-44ef3f0a425c'></a>

<::logo: [Unknown] [None] [A red abstract symbol resembling a star or asterisk, with eight curved arms pointing outwards from a central point.]::>

<a id='9df4a404-e381-473b-a786-520676e6271d'></a>

Multi-Agent Telecom Chatbot / Log Stream: prod ⌄ / Session: Telecom Agent - 2025-09-25 20:...
← /
option Messages: [ ]
option Latency: [x]
option Trace graph: [ ]
<::Latency chart displaying activities over time:

Time axis (top): 0m, 1m

Activities (left column):
- call_model
- Prompt
- Supervisor
- should_continue
- transfer_to_billing_account ag...
- call_agent
- Billing Account Agent
- billing_account
- transfer_to_technical-support-...
- Technical Support Agent
- transfer_to_plan-advisor-agent
- Plan Advisor Agent
- pinecone_retrieval

The chart shows various colored bars and dots distributed across the timeline for each activity, indicating their occurrences and durations.
: chart::>

<a id='d4f1a41c-5ea6-4b4a-a6db-b1767b8c776b'></a>

FIGURE 2.6 Timeline View

<a id='ad77f7aa-bd72-4fef-b3be-a6f9f413537e'></a>

The Timeline View (FIGURE 2.6) breaks down time spent in each phase for
performance optimization:

→ Agent communication latency (identifying slow handoffs between agents)
→ Processing latency (showing when coordination
overhead impacts performance)
→ Generation latency (revealing when response assembly affects speed)

<a id='bf6268cd-9f33-4865-a6dc-cf56ba55d73e'></a>

Use these insights to identify which agent interactions create bottlenecks and where you can optimize handoffs.

<a id='bdb403f4-169d-4b34-9e82-95b0dc8dc151'></a>

55

<a id='d2ca88ab-af77-4a84-810c-073a869a4a9e'></a>

Mastering Multi-Agent Systems )) MAS ((

<a id='efb4ddb0-a18e-4cb5-824c-76440a1c984c'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='0fc99e68-7229-49c2-b6d0-8c492cecf7bf'></a>

Chapter 02

<a id='41bb25fd-137b-4abc-9604-e28491ac7e36'></a>

Why Multi-Agent Systems Fail

<a id='b267d483-85af-47ad-a81c-0a186598d1e7'></a>

<::logo: Unknown
A red abstract starburst or pinwheel shape is centered in the image.::>

<a id='9610b54d-b9c6-42d6-b628-b09b977afc96'></a>

← Table view Trends option Agent graph: [x]
12H 1D 1W 1M 6M 1Y Log Stream Insights Alerts Configure Metrics
<::A flowchart titled "Agent Graph" displays a series of interconnected rectangular nodes representing different agents and processes. The graph is divided into two main sections.

The upper section shows:
- "connect-supervisor-agent" connected to "billing-account-agent" and "technical-support-agent" via dashed lines.
- "billing-account-agent" connected to "plan-advisor-agent" via a dashed line.
- "technical-support-agent" connected to "set_agent" via a dashed line.
- "plan-advisor-agent" connected to "set_agent" via a dashed line.
- "set_agent" connected to a larger section labeled "agent" below.

The lower section, enclosed within a large box labeled "agent", contains:
- "self_model" as a separate node.
- A "RunnableSequence" block which contains:
  - "Prompt"
  - "Technical Support Agent" connected to "Supervisor"
  - "Supervisor" connected to "Plan Advice Agent"
  - "Plan Advice Agent" connected to "Billing Account Agent"
  - "Billing Account Agent"
- A solid line connects the bottom of the "agent" box to a node labeled "should_continue".

Navigation controls for the graph are visible above the main graph area, including zoom in/out, fit to view, and fullscreen options.
: flowchart::>
Aggregate Agent Graph
This graph shows the structure of your agent as inferred from the set of filtered traces. If the structure of your agent changed during this interval, the graph will attempt to unify all versions. Click on a node or an edge to view details.
General Select one to filter
Sessions 4
Traces 27

<a id='370f8300-7f5c-493c-9594-fd95a2d73523'></a>

FIGURE 2.7 Graph View

<a id='15444364-5153-47cc-903b-8b529e16c855'></a>

Leverage Log Stream Insights for
production debugging:

* Real-time error detection
  with stack traces
* Automatic correlation of related
  events across distributed agents
* Pattern matching to identify
  recurring coordination issues
* Export capabilities for
  offline analysis

<a id='3135ac1f-d968-4ce4-9d3b-90ceb683a122'></a>

Use Graph View (FIGURE 2.7) for
architectural decisions:

- Identify redundant agent interactions
  that could be optimized
- Spot opportunities to
  parallelize agent work
- Visualize multi-agent coordination
  and information flow
- Export graphs for architecture
  documentation

<a id='04cd5318-87e6-489c-94cc-c1f3fc0ce3ff'></a>

56

<a id='8e653eac-dd2b-442f-b1fe-a29ca51e4937'></a>

OOO Mastering Multi-Agent Systems » MAS (

<a id='7c015240-b6a5-414e-8100-89f269631957'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='a147842b-5e32-439d-b63a-48ca8d43bb12'></a>

Chapter 02

<a id='9b87f598-cdfe-4e3b-9585-70cbf12c9ad3'></a>

Why Multi-Agent Systems Fail

<a id='9f66c6cf-4491-4d00-a00b-845f33e5d386'></a>

<::logo: [Unknown] [None] [A red asterisk-like symbol with four thick, curved arms extending outwards from a central point]::>

<a id='66e4b698-e5a8-4576-818f-f6fc527d408a'></a>

4. Configure Continuous Monitoring and Alerting

Set up alerts based on patterns detected in the Log Stream to catch issues early. Configure thresholds in the Timeline View to notify you when agent coordination exceeds acceptable limits.

<a id='1822ab16-e4d6-4ea2-87ce-290eb3e09091'></a>

**Intelligent Alerting**: Anomaly detection that learns your system's patterns and flags deviations

<a id='a4c1776d-39fd-4e9f-a980-1955db258d00'></a>

Custom Dashboards: Combine Trace, Graph, and
Timeline views into unified monitoring screens

<a id='5fd11db3-2381-4d75-a259-8419cacfa21b'></a>

Integrations: Native connectors for LangGraph,
CrewAI, and other frameworks

<a id='076ba849-ba66-4c5c-8add-92cf5d008517'></a>

API Access: Programmatic access to all metrics for custom analysis

<a id='3b669f35-d725-4fcb-8719-fe5507423dcc'></a>

Treat these visualization and monitoring tools as a continuous
feedback loop:

-> Trace View shows what happened
-> Graph View shows why it happened
-> Timeline View shows how fast it happened

<a id='6b41fbdc-5eed-4b11-874e-f48586164118'></a>

57

<a id='e2ce6c5e-8a44-4230-b1e9-425ce01c8946'></a>

Mastering Multi-Agent Systems )) MAS ((

<a id='19a099d2-3eb6-4a75-95bf-d8c70f4b0319'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='ba90839e-53c5-498c-b2b3-e10ca3275fb2'></a>

Chapter 02

<a id='56800380-3f9e-4b2c-b800-809e7b010764'></a>

Why Multi-Agent Systems Fail

<a id='9a1f2fda-0c7a-4729-b634-70fb8ade3070'></a>

<::logo: [Unknown] [None] [A red asterisk-like symbol with four thick, curved arms extending outwards from a central point]::>

<a id='bc65b116-34c1-4d10-a85d-7d4818b9fcb7'></a>

Your Path To Reliability

<a id='12c6a79f-d74e-4f5e-9543-e003d309301f'></a>

Multi-agent systems aren't inherently bad.
The excitement around them stems from
an intuitive but flawed assumption: if one
smart agent is good, many must be better.

<a id='f0fbf614-375d-44c3-ae93-ab34aae4f65e'></a>

The most successful approach follows a simple progression:

1. Start with single agents and master prompt engineering and context management
2. Understand your task's true dependencies through careful analysis, not assumptions
3. Measure actual parallelization potential with real data, not theoretical benefits
4. Only consider distribution when you hit genuine single-agent limitations

<a id='589d2871-a4de-44b5-9786-0f2c23b5e849'></a>

Remember that models are improving
quickly. Don't over-engineer a distributed
solution today for a problem that a
simpler system will solve tomorrow.

<a id='cd01ad0f-3732-407a-9369-d8a702f4dfd3'></a>

The core challenges that cause multi-agent failures, such as context loss, coordination overhead, and debugging complexity, have solutions, as shown in FIGURE 2.8. Galileo addresses these through semantic context compression, standardized agent protocols, and comprehensive observability tools.

<a id='b8d7b5ee-c834-4c31-8c30-c267c9310e13'></a>

But the fundamental question remains: does your use case justify the complexity?

<a id='e803824e-5a21-4135-834f-ddf28dbb7f2c'></a>

<table id="26-1">
<tr><td id="26-2">Today&#x27;s reality</td><td id="26-3">Context loss Critical nuance lost in every handoff between agents (checkbox icon)</td><td id="26-4">No coordination Agents work in isolation without shared understanding (alert icon)</td><td id="26-5">Black box Impossible to trace failures across agent boundaries (box icon)</td></tr>
<tr><td id="26-6">Three strategic pillars of change</td><td id="26-7">1. Context compression Semantic-aware compression 10x token reduction Preserve decision rationale Maintain confidence levels (up/down arrow icon)</td><td id="26-8">2. Agent protocols Intent communication Confidence signaling Context boundaries Shared language (list icon)</td><td id="26-9">3. Deep observability Cross-agent tracing Failure pattern analysis Component visibility Causality tracking (magnifying glass icon)</td></tr>
</table>
Galileo's solution
Graph engine
Trace complex agent paths and
interactions
Insights engine
Identify failure modes
and patterns
Scalable metrics
Customizable performance
tracking

<a id='f745a88b-d716-4e23-8a7a-57cd32b356fc'></a>

FIGURE 2.8 Galileo's approach to solving multi-agent system challenges

<a id='873eec8d-dbbf-4caa-8a00-96114ffd0acb'></a>

58

<a id='43004968-2df9-4214-9ce4-19631875dd3f'></a>

Mastering Multi-Agent Systems )) MAS ((

<a id='ed7e9a38-3b63-4b7a-a6bc-f1ddc4da1830'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='7194f165-a967-4e06-9953-0bf54b03f6d3'></a>

Chapter 02

<a id='e8b8a26e-3f75-4451-b638-f1f116884a41'></a>

Why Multi-Agent Systems Fail

<a id='ab9aa836-b550-41fa-ae81-e0fd93cd2e34'></a>

<::logo: [Unknown] [No readable text] [A red, star-like symbol with four curved arms pointing outwards]::>

<a id='0c3d90c7-1fbe-41c9-8510-c3396cc8736a'></a>

What You've Learned

<a id='0c78f465-b8c4-4db6-804a-73d358327140'></a>

You learned why coordination costs often destroy the benefits of specialization and gained a practical framework for deciding whether your use case actually needs multiple agents.

<a id='75332ef3-8cf3-423d-9458-8d88909664aa'></a>

<table id="27-1">
<tr><td id="27-2">Factor</td><td id="27-3">Multi-Agent</td><td id="27-4">Single Agent</td></tr>
<tr><td id="27-5">Task Structure</td><td id="27-6">Tasks can run independently in parallel</td><td id="27-7">Tasks must happen one after another</td></tr>
<tr><td id="27-8">Data Processing</td><td id="27-9">Agents read and analyze separately</td><td id="27-a">Agents need to modify the same data</td></tr>
<tr><td id="27-b">Cost Tolerance</td><td id="27-c">Can afford 2-5x increase for reliability</td><td id="27-d">Need to minimize costs</td></tr>
<tr><td id="27-e">Speed Requirements</td><td id="27-f">2-5 seconds is acceptable</td><td id="27-g">Need sub-second responses</td></tr>
<tr><td id="27-h">Scale Demands</td><td id="27-i">High-volume parallel processing</td><td id="27-j">Small-scale simple tasks</td></tr>
<tr><td id="27-k">Failure Tolerance</td><td id="27-l">System must stay partially operational</td><td id="27-m">Complete failure is acceptable temporarily</td></tr>
<tr><td id="27-n">Model Evolution</td><td id="27-o">Requires distinct expertise areas like legal, medical, technical</td><td id="27-p">Single domain and the model just needs improvement</td></tr>
</table>

<a id='1ba8c16c-3b41-4955-8105-a5297e080a76'></a>

TABLE 2.2
Multi-Agent Systems: Where they work and where they may not

<a id='794ad344-22cb-4641-99db-b53d4204524d'></a>

59

<a id='383f132e-40dc-4190-b9b8-bcb1c89ff4a5'></a>

Mastering Multi-Agent Systems » MAS (

<a id='0340a755-438d-4b53-aa99-0c74e291eeef'></a>

-> galileo.ai

<!-- PAGE BREAK -->

<a id='11b27e25-f578-47a8-8645-2537c743ddf1'></a>

Chapter 02

<a id='aed77e90-6155-4b1c-8e7d-f7c9e8ae3a10'></a>

Why Multi-Agent Systems Fail

<a id='da756814-0d90-4e97-bc37-5e12538e78c5'></a>

<::logo: [Unknown] [No readable text] [A red abstract symbol with four curved elements pointing inwards, forming a star-like shape]::>

<a id='68222864-2960-4fd8-be1e-b79abb55ced7'></a>

TABLE 2.2 summarizes the key decision factors from this chapter. Multi-agent systems are effective when you require parallel processing for scalability, validation layers for accuracy, and flexible routing for cost optimization. They struggle when you need sub-second response times, minimal operational complexity, and have tight budget constraints.

<a id='0f3a5e4e-7bd7-4ff1-a825-67120783ff85'></a>

The pressing question is, which specific problems in your stack
would benefit most from specialized agent teams?

<a id='c64be947-8063-4704-9944-ec5f99bdb297'></a>

Understanding when multi-agent systems fail is only half the battle. When you do decide that coordination costs are worth the benefits, you face another challenge: how do you actually build these systems? The architecture you choose determines not just performance, but which problems become solvable at all.

<a id='f4320edb-a019-429a-9cad-59e867076bf8'></a>

In Chapter 3, we'll explore the four primary architectures for multi-agent systems and how each one creates different capabilities and constraints. You'll learn when centralized orchestration works better than peer-to-peer coordination, how hierarchical systems handle complex workflows, and which frameworks actually deliver on their promises versus which ones add unnecessary complexity.

<a id='1710938b-dd1d-4d91-84d8-c49655ea5c6e'></a>

60

<a id='5af46638-1abc-444b-ae72-c614a51a52d2'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='23988884-4050-4418-a96a-4856b2689d2c'></a>

→ galileo.ai

<a id='048bde63-01c6-4fc8-8fcb-9f6a6107cf1e'></a>

<::logo: [Unknown] [None] [A red outline of a U-turn arrow pointing right]::>

<!-- PAGE BREAK -->

<a id='8af57cd9-c8af-49a3-99c6-f63670c0a2f2'></a>

<::logo: Galileo
Galileo
A red, abstract star-like shape is to the left of the text "Galileo"::>

<a id='785b0724-3aea-4a1e-b02f-0e1a2798bc3d'></a>

<::logo: [N/A]
Chapter
03
Black text "Chapter" above red text "03" on a white background with a subtle textured pattern.::>

<a id='1b0c7f5e-8ddb-4125-8830-f4f2d01c74fd'></a>

Architectures
for Multi-Agent
Systems

<a id='33d9a9ee-f2d7-438b-a257-f498f6105bbc'></a>

Mastering Multi-Agent Systems

<a id='1e7abf51-c2cb-494e-add5-660daf454d00'></a>

-> galileo.ai