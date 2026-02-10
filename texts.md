<a id='0387472f-bbf4-443e-8168-2386e702b3e2'></a>

<::logo: Galileo
Galileo
A red abstract star-like symbol with multiple arms to the left of the wordmark.::>

<a id='b512b204-8b13-4120-a1a3-65459593cc23'></a>

v1.01

<a id='130235b8-18b9-41da-a4b5-f74f4e0cd988'></a>

Mastering
Multi-Agent Systems

Real-World Strategies for Multi-Agent Development

<a id='d5fc0c2e-0b50-4d1a-a5a0-c7bb9cf307f2'></a>

<::An image depicting three people and a dog in a modern, open-concept living space, with elements of a planetary or atomic system superimposed. On the top left is the text "galileo.ai". On the top right, the text reads "Mastering Multi-Agent Systems >) MAS <". The man on the left is laughing, wearing an orange outfit, sitting cross-legged. A woman in the center smiles, holding a large, bright glowing sphere, wearing a white sweater. A second woman on the right smiles, looking towards the center, wearing a light blue outfit. A brown and white dog sits between the man and the central woman. Several smaller glowing spheres, resembling planets or moons, orbit the central sphere, connected by faint white orbital lines. On the right side, percentages are visible: "64%", "88%", "100%", and an obscured value below it. At the bottom right, the text reads "Multi-Agent >*<" followed by an icon and then "▷ Systems". The background shows a modern interior with a stone wall and large windows looking out onto a desert-like landscape with sparse vegetation.
: image::>

<a id='f8e881c6-8667-4226-b332-938471bf4e55'></a>

Mastering GenAI Series

<a id='a95f5332-6977-4a01-a17b-a8290834db62'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='2066c59c-8c22-4b8b-949a-616be1b1a929'></a>

<::logo: Galileo
Galileo
A red abstract star-like symbol with four points is placed to the left of the company name.::>

<a id='8476a678-9cf5-465d-a1fd-f3df99aa8580'></a>

<::logo: 
Chapter
02
A white square with "Chapter" in black text and "02" in large red text below it::>

<a id='b627655e-eedf-4f2a-92ea-47fc48dc4764'></a>

# Why Multi-Agent Systems Fail

<a id='eff25a8e-528a-415a-a5f5-9f1ac46fdafc'></a>

Mastering Multi-Agent Systems

<a id='ceff3498-db27-4626-881f-f7f6254f861b'></a>

-> galileo.ai

<!-- PAGE BREAK -->

<a id='14bfc002-1089-445c-95a2-c844f5ffbd5e'></a>

Chapter

<a id='802b0a15-8a81-4a15-a468-9f1605533f47'></a>

<::logo: [Unknown] [No readable text] [A red asterisk-like symbol with four curved arms]::>

<a id='37614760-c860-4cf2-8a25-71c4bb546a44'></a>

02 Why Multi-Agent Systems Fail

<a id='cd9e1251-9110-4a80-84ed-16d5c3a1d771'></a>

Multi-agent systems look great on paper. You split complex work across specialized agents, add validation layers to catch errors, and process data in parallel for speed. Everyone sees these benefits and starts building, but many of them abandon their projects in a couple of months.

<a id='90d6b2fc-cf2d-4f3f-9260-afb21e13cbd6'></a>

But the agents themselves aren't the problem, as individual agents work fine. What adds complexity to these systems is the coordination between them. The system becomes difficult to manage and ends up costing more.

<a id='d4a6c97a-288e-4b3b-ade6-43d531c90b52'></a>

This chapter breaks down the complexities of building a multi-agent
system. You'll see the hidden costs of building them and get a decision
framework to evaluate whether your use case can benefit from it.

<a id='5eac3b6c-8ffd-46fc-a93b-3d24e8f0a5d5'></a>

34

<a id='9634db33-8f60-4703-aa0a-1d7329a5c27b'></a>

Mastering Multi-Agent Systems )) MAS ((

<a id='9611fc69-5222-4c74-ad98-edad0f935af5'></a>

-> galileo.ai

<!-- PAGE BREAK -->

<a id='f16880af-8ec3-4827-930e-1d8409af93bf'></a>

Chapter 02

<a id='92243f7e-3d20-4d71-bdf7-af90a06454e1'></a>

Why Multi-Agent Systems Fail

<a id='16f8c406-2519-48c6-a5c0-cf1c9a60787e'></a>

<::logo: Unknown

A red asterisk-like symbol with four curved arms pointing outwards from a central point::>

<a id='d2536686-8c13-4524-9b26-067ec9b8e2e4'></a>

Why Coordination Costs Matter

<a id='fb7be29d-67dc-40c9-a06c-c0df502b4bbf'></a>

Multi-agent systems struggle when coordination overhead exceeds the value of specialization. Two agents need one communication channel. Three agents need three channels. Four agents need six. Soon, your system becomes harder to manage than it is useful.

<a id='28089531-0066-470f-bb3c-60c1b8ff5f1e'></a>

Consider the last time you worked on a
team project. How much time did you spend
on the actual work versus coordinating
with teammates? Multi-agent systems
face this same challenge, but amplified.

<a id='dc59fe5b-95cd-4337-b937-62defc988711'></a>

Here's how it plays out in practice. Imagine a web development workflow where a multi-agent system builds a dashboard:
→ Agent 1 analyzes requirements and decides on the component structure
→ Agent 2 implements the authentication flow
→ Agent 3 builds the data visualization
→ Agent 4 handles API integration

<a id='a92cd872-b623-4425-98f6-150a1908e42e'></a>

Each agent needs selective knowledge from the others. Agent 2 needs the component structure but not the full requirements analysis. Agent 4 needs auth tokens but not implementation details. This creates cascading memory challenges that single agents don't face.

<a id='54e1fd9a-32c9-462b-bc57-f8c9e4bc7835'></a>

35

<a id='b30218cd-86fc-4b45-949c-897523c5e486'></a>

OOO Mastering Multi-Agent Systems >> MAS (

<a id='890d79ba-b3c7-4e6d-a168-30816d5a1f14'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='2fc28181-d6ad-46c7-8855-20b5744ac2d6'></a>

Chapter 02

<a id='4ef10816-afd1-4950-908a-db7114a8e440'></a>

Why Multi-Agent Systems Fail

<a id='a1331dd6-7214-49c0-bd4f-0098f22741fe'></a>

<::logo: Unknown

A red asterisk-like symbol with six points::>

<a id='35175ad9-ca81-4d7e-a8d9-5f0ca94e4cb2'></a>

Let's look at three high-impact scenarios that
can break multi-agent systems:

<a id='742a793a-0046-4426-99a4-dca07db1e7df'></a>

1.
Memory fragments across agents
Each agent maintains its own context about the project. When Agent 3 needs to understand Agent 1's component decisions, it either gets too much information (driving up costs) or too little (breaking functionality). There's no clean way to share just the relevant details.

<a id='d2116203-d56c-4111-a069-bf386d7c39ad'></a>

2.
Operational costs multiply
A simple task that costs $0.10 for a single agent
might cost $1 for a multi-agent system. The extra
cost is due to all the context sharing, handoffs, and
verification required to keep agents synchronized.

<a id='06df88f0-def6-4c75-a93b-d1167a7831a8'></a>

36

<a id='fd5ac906-50e7-446d-873b-e4a6942fd076'></a>

OOO Mastering Multi-Agent Systems )) MAS (

<a id='b7d9f765-e1e8-47ac-8692-40e5616f90b6'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='1bb10f87-bc18-487c-89a4-49a16b342a0f'></a>

Chapter 02

<a id='1b1bf142-224d-4ea3-8dca-4c5ab2c785e6'></a>

Why Multi-Agent Systems Fail

<a id='f61b43ae-e676-42c4-ab79-71ce9f845c16'></a>

<::logo: [Unknown] [] [A red asterisk-like symbol with four curved arms]::>

<a id='a4d9e938-f3ca-4a86-855a-59e80c401db8'></a>

3.

Write conflicts cascade

When agents only read data and combine findings, conflicts stay manageable. But when they modify the same system, conflicts multiply (FIGURE 2.1). Agent A creates a user profile structure. Agent B, working independently, creates a different structure. Agent C tries to reconcile both and creates a third. Your system now has three incompatible ways to represent the same user data.

<a id='48b77647-229a-4824-ab6c-754e846efedd'></a>

Each interaction creates opportunities for context loss, misalignment, or conflicting decisions.

<a id='10f170c9-4412-4383-b28f-b3d0c7f51021'></a>

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

<a id='a11f2454-e766-4b6b-80a1-b851dad461b2'></a>

FIGURE 2.1 How write operations create cascading conflicts in multi-agent systems

<a id='f2c79dbc-4dcb-446e-9427-b8008f542626'></a>

37

<a id='7bf82c3b-efc6-431d-b899-88ba8a064d0b'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='c3923bba-f2e2-4897-bbe6-091c5f58b3f3'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='44bd9847-8314-43d3-8ae5-7cfde0dbf4e4'></a>

Chapter 02

<a id='fa976e84-d492-4192-8366-0b2d398ab835'></a>

Why Multi-Agent Systems Fail

<a id='610ab8ed-41b7-4512-a7aa-08c242d18a53'></a>

<::logo: [Unknown] [None] [A red asterisk-like symbol with four thick, curved arms extending outwards from a central point]::>

<a id='ed67bb91-411c-4720-a846-fdb295200345'></a>

When Multi-Agent Systems Actually Work

<a id='1736ab03-e19b-4899-a925-930523cea5a3'></a>

Successful multi-agent implementations share specific characteristics most teams overlook.

<a id='ec450578-32a8-4379-a79a-d313528f6c8c'></a>

[Anthropic's research system](https://example.com) is a good starting point. When tasked with analyzing the impacts of climate change, it spawns specialized agents that simultaneously investigate economic effects, environmental data, and policy implications. Each agent processes 50+ sources that a single agent would never have time to handle.

<a id='4f5a7822-f1f0-41a3-893e-e2c12fee7957'></a>

In this scenario, each agent works
independently, and they don't modify another's
findings. When they finish, an orchestrator
agent (explained in Chapter 3) combines
their findings into a comprehensive report.
There's minimal coordination overhead as
there's no back-and-forth coordination
during the work itself. It's just independent
analysis followed by aggregation.

<a id='8acd6479-341c-492a-a5c7-34e9e2668246'></a>

Here are three specific patterns that most successful implementations use:

<a id='b93ad488-15d8-4496-b671-51a71b33548a'></a>

1. Problems that can be parallelized

Multi-agent systems work well when problems can be split into pieces that require no communication during processing.

<a id='08c09525-56d8-4cb6-98c2-8eb400ce4bb1'></a>

Say you have 100 quarterly reports from various companies to analyze
for investment insights. Each agent takes a report and extracts key
metrics: revenue growth, profit margins, debt ratios, and market position.
No agent needs information from another agent's reports. At the end,
you aggregate all findings into a comprehensive market analysis.

<a id='c98d9f26-c321-48c9-9e88-298bec5a5c9b'></a>

38

<a id='ea9edf26-d772-46f6-ae8b-2ba0008adf5f'></a>

Mastering Multi-Agent Systems )) MAS ((

<a id='283ead31-f2a7-49ce-b851-43b6374e632a'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='2e392ac5-29f6-4046-83e2-7bd47fb39248'></a>

Chapter 02

<a id='5cd921b8-b64b-4301-9dad-75a86f1e128b'></a>

Why Multi-Agent Systems Fail

<a id='6bd5e03d-88ad-43d3-9c76-fc9d7f07ef38'></a>

<::logo: [Unknown] [None] [A red asterisk-like symbol with four thick, curved arms extending outwards from a central point]::>

<a id='4d0b2270-7198-47ca-a41f-1f4b3dc1ad33'></a>

2. Read-heavy, write-light workloads
When agents primarily consume information rather than modify shared state, coordination complexity drops dramatically. Each agent can work independently and combine results at the end.

<a id='3ceccba9-111a-4cfb-90c1-4060450fe731'></a>

Say you're tracking competitor activities across multiple channels. Agent 1 monitors news articles, Agent 2 tracks social media mentions, Agent 3 analyzes patent filings, Agent 4 watches hiring patterns. Each of your agents consumes large amounts of public data and produces intelligence reports. The final analysis combines all reports without agents needing to coordinate during data collection.

<a id='6b7a45a8-be9a-4672-9ccf-f3d5e7c6548a'></a>

3.
Explicit coordination rules
Successful implementations use deterministic orchestration with clear handoff points. Anthropic's system doesn't rely on agents figuring out how to work together. It defines exact data formats, interaction protocols, and fallback behaviors through explicit rules.

<a id='18729e4a-5f3f-4798-a224-9f7b5c1b26a4'></a>

Consider this example from programming and software development. A code change triggers a sequence: Agent 1 runs unit tests and reports pass/fail status, Agent 2 executes integration tests if unit tests pass, Agent 3 performs security scans if integration succeeds, Agent 4 deploys to staging if all checks pass. Each step has clear success criteria, failure protocols, and rollback procedures in place.

<a id='62b3d2e0-7d04-4477-9bd5-4bd0f3080bf4'></a>

39

<a id='84e1352e-8b4b-4ba7-aba9-14515aa5d10c'></a>

OOO Mastering Multi-Agent Systems >> MAS (

<a id='a33e916a-92af-463f-8921-1d791faa5a67'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='7f1a87ed-4c0f-477e-98d0-649b658a8ede'></a>

Chapter 02

<a id='8f8e30b1-913f-4cfe-8ce6-fae36c761e45'></a>

Why Multi-Agent Systems Fail

<a id='981f7654-26a3-4702-a9af-9d4f413c1b92'></a>

<::logo: Unknown
No readable text
A red asterisk-like symbol with five arms, each arm consisting of two curved lines that meet at a point, arranged in a circular pattern::>

<a id='3d58f520-1161-4927-b861-5db0eb1dd051'></a>

Consider this example from programming and software development. A code change triggers a sequence: Agent 1 runs unit tests and reports pass/fail status, Agent 2 executes integration tests if unit tests pass, Agent 3 performs security scans if integration succeeds, Agent 4 deploys to staging if all checks pass. Each step has clear success criteria, failure protocols, and rollback procedures in place.

<a id='7657cf74-142c-465b-9bdf-d65f95cd0f52'></a>

Here's a checklist to decide if your use case benefits from a multi-agent setup:

option Can you break down the work into completely independent tasks?: [ ]

option Do agents primarily read and analyze rather than write and modify?: [ ]

option Can results be combined mechanically (concatenation, voting, averaging)?: [ ]

option Is parallel processing speed worth a 2- to 5-fold cost increase?: [ ]

option Can one agent failing be isolated from others?: [ ]

<a id='fdf957f4-99fa-4d05-97d2-095a9e6a3a20'></a>

Use this checklist to help you determine whether your current problem aligns with multi-agent patterns. Before building any multi-agent system, ask: Will this approach still make sense six months from now?

<a id='a0ce48e6-c9f1-419f-b083-789b8ee101a6'></a>

This question matters because you're choosing an architecture that needs to work
as models rapidly improve over time. The history of AI suggests that complex
workarounds often become unnecessary overhead when better models emerge.

<a id='14f7496f-d55a-4e6f-b2c8-fe586f84a193'></a>

40

<a id='501beb04-d1be-4ff8-be5f-edba52db17f0'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='5a31a3e9-d7d0-4216-aed0-7f9b6fd37115'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='e4f0e0d6-2fdb-4474-a2c9-02d22310aa39'></a>

Chapter 02

<a id='6e14541a-0008-4318-8a27-0d8090a7c07b'></a>

Why Multi-Agent Systems Fail

<a id='e6070b24-44f6-4e24-8138-59eaf3c3e4a4'></a>

<::logo: Unknown

A red asterisk-like symbol with four curved arms pointing outwards from a central point::>

<a id='c2baf53c-8a60-4a8a-a2d4-d86b716e2fe1'></a>

The Model Evolution Challenge

<a id='b5200ef5-c188-4c83-a138-bbc0bbb2d778'></a>

Rich Sutton's Bitter Lesson teaches us that general methods using more computation ultimately win over specialized structures. This principle now collides with multi-agent system design in ways that should make you pause.

<a id='a76226d1-3dad-41a7-9df8-56c468f45d99'></a>

Consider what you're actually doing with multi-agent systems: adding structure to compensate for current model limitations.

*   Can't get your model to handle complex reasoning in one pass? Split it into specialist agents.
*   Is the context window too small? Distribute the load.
*   Is the tool calling unreliable? Create dedicated tool-use agents

<a id='9a244b36-a60d-45ce-94e1-bd299864fc37'></a>

What happens when these limitations disappear?

<a id='9b128de0-68b6-40ca-a460-7259c88a630f'></a>

Think About Your Current Project.

What model limitations are you working around with
your multi-agent architecture? Context windows?
Reasoning capability? Tool use reliability? Write
these down. They're your obsolescence risks.

<a id='e062daa4-7093-42bf-80a3-f9dee3f2d818'></a>

Teams that built complex orchestration layers for GPT-4 found them
unnecessary with GPT-5. Multi-step reasoning chains designed
for Claude 3 became single prompts with Claude 4. The structure
added to work around limitations became the limitation itself.

<a id='903b44af-8cb1-430a-8285-60487b911f3a'></a>

41

<a id='2ef434e3-4585-43cd-a260-67d27882c520'></a>

(OOO Mastering Multi-Agent Systems >> MAS (

<a id='58a5f06e-016f-4142-9348-8c7e3abead25'></a>

galileo.ai

<!-- PAGE BREAK -->

<a id='84b9df75-56da-4c02-ae9d-a90efa82c312'></a>

Chapter 02

<a id='19dcd584-f8d8-4520-b76d-98ce4e8b0ad9'></a>

Why Multi-Agent Systems Fail

<a id='1ea85e77-5d02-4f64-868b-53e49e3140aa'></a>

<::logo: [Unknown] [] [A red asterisk-like symbol with four curved arms]::>

<a id='e28b2971-6f9d-423e-b7cd-9cb71b506504'></a>

Boris from Anthropic's Claude Code team gets this. Instead of building elaborate multi-agent systems, he focuses on leveraging model improvements directly. The recent success of single-agent systems beating multi-agent baselines validates this philosophy. Our agent leaderboard shows this pattern clearly: newer models consistently outperform older multi-agent systems while being faster and more cost-effective.

<a id='e7445dc9-6855-40c6-b28c-1311e0c28905'></a>

This pattern repeats across AI development. You might spend months building a complex multi-agent system only to find that a newer model can handle the same work in a single call. The distributed system you worked so hard to build becomes unnecessary overhead.

<a id='cf5f9a37-c47f-472a-8cfe-8fa15522ccc7'></a>

The smarter approach is to follow Hyung Won Chung's philosophy:

<a id='170f5a93-f64a-43fd-b489-29de73f43642'></a>

Add minimal structure:
Instead of building five specialized agents (requirements, authentication,
database, API, frontend), start with two: one for backend logic, one for frontend.
You can always split further if needed, but merging is harder than splitting.

<a id='f0cc97cf-8e52-4129-988c-1f8da26b2db4'></a>

Plan for removal

Write your orchestration code in a separate module that you can delete
entirely later. When a better model arrives, you should be able to delete
the orchestration layerfile and call the underlying functions directly.

<a id='3341e26b-752d-4975-8ae7-da1a47b9b381'></a>

## Make boundaries collapsible

Structure your agents so their logic can merge into a single prompt. If Agent A does research and Agent B writes summaries, write them so you can combine both into one "research and summarize" agent later.

<a id='87278ec2-51b3-419c-847b-c58a054bd4d8'></a>

Separate orchestration from business logic
Your authentication logic should work the same whether it's called by an orchestrator or directly. Keep the business logic separate from the orchestration.

<a id='c0feb66a-45ca-4902-b71d-6895f151b328'></a>

If you're splitting tasks across agents because the model can't
handle complexity, waiting a few months for a better model might be
more effective than building infrastructure you'll have to scrap.

<a id='ded80ff7-329f-4819-aa12-8759d8d30e09'></a>

<::logo: Unknown
42
The numbers "42" are prominently displayed in red, set against a light gray square background.::>

<a id='9791ec2d-d0c3-41c5-af3d-43704ea3e6db'></a>

Abstract logo Mastering Multi-Agent Systems )) MAS (

<a id='ae66b5c2-48f8-4155-ad4c-87d56aab279c'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='66726218-c1e9-4efe-9c3c-4d869fef856d'></a>

Chapter 02

<a id='edaab05a-e675-4895-813d-bedf8703f78a'></a>

Why Multi-Agent Systems Fail

<a id='344a4680-1443-4a8a-a32f-25bb2e19d454'></a>

<::logo: [Unknown] [] [A red asterisk-like symbol with four curved arms]::>

<a id='ea5d1ac2-15be-49da-bde4-2dede878f2c2'></a>

What Frameworks Actually Deliver

<a id='13549e56-4b6b-42eb-b666-90afae9a1cb4'></a>

These days, we have many frameworks
for building agents. They tackle the same
core challenge: how do you coordinate
multiple agents without losing critical
context? The approaches vary, but none
solve the fundamental problem.

<a id='e0ab87ea-628a-47be-be98-c9e675753736'></a>

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

<a id='c7963b11-c9cb-4a47-9383-0f3f79389d6f'></a>

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

<a id='faa55847-2e37-4bb5-a135-c38b9be4a117'></a>

The core problem remains unsolved:
efficient context passing between agents.
Current approaches either share everything
(expensive and slow) or share summaries
(losing critical details). No framework has
solved selective, semantic context transfer
that maintains accuracy while minimizing
overhead. Refer to TABLE 2.1 to see a
comparison of different agentic frameworks.

<a id='231b4274-9d2e-4a53-945e-922f6c9405f1'></a>

<table id="11-1">
<tr><td id="11-2">Framework</td><td id="11-3">Strength</td><td id="11-4">Limitation</td></tr>
<tr><td id="11-5">CrewAI</td><td id="11-6">Simple role-based setup</td><td id="11-7">Limited context control</td></tr>
<tr><td id="11-8">LangGraph</td><td id="11-9">Full state management</td><td id="11-a">High complexity overhead</td></tr>
<tr><td id="11-b">Swarm</td><td id="11-c">Lightweight coordination</td><td id="11-d">Manual context passing</td></tr>
</table>

<a id='442d1e92-8988-4a91-9cf9-c1e88196de89'></a>

TABLE 2.1 Comparison of different agentic frameworks

<a id='868aa684-3dcc-4bb5-aa5f-fb23d39d663e'></a>

43

<a id='5cc293dc-b246-4d1a-b068-fa9717eeb72c'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='c54251f6-acb8-4a94-af1f-57486b4d5944'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='5fb15e12-3ab2-4932-bf0a-e9b32ed7df87'></a>

Chapter 02

<a id='1f764585-d3bf-438f-ad71-c9670e9dcbcc'></a>

Why Multi-Agent Systems Fail

<a id='e8536a69-a93b-4217-8c70-b80b39f46adc'></a>

<::logo: [Unknown] [None] [A red asterisk-like symbol with four thick, curved arms extending outwards from a central point]::>

<a id='cda5dc8b-bb5b-415b-82c2-afe1aaa01b04'></a>

Consider this workflow: Agent A analyzes a 50-page requirements document
and identifies 12 key components. Agent B needs to implement authentication
based on those requirements. How much context does Agent B actually need?

<a id='a32962ea-e9df-42cd-b974-aec925ea80a9'></a>

**Option 1: Share everything:**
Agent B gets the full 50-page analysis plus Agent A's complete reasoning chain. This works but costs 10x more in API calls and processing time.

<a id='d3dcf543-d4ff-4bb8-a658-a8ca8a678d6b'></a>

Option 2: Share summaries:

Agent B gets a condensed version of the key authentication
requirements. This costs less but risks losing the
nuanced decisions that affect implementation.

<a id='87e947d7-ec24-40ca-9809-d27afaf0e7e5'></a>

Option 3: Selective sharing:
Agent B gets precisely the authentication-relevant
context with enough surrounding detail to make informed
decisions. No framework handles this automatically.

<a id='4f6b42ec-ef7b-4626-bac1-f651ea71fdb2'></a>

While frameworks can't solve the context efficiency problem, they do handle the mechanics that would otherwise require significant custom development. However, they can't solve the fundamental coordination economics that make most multi-agent systems too expensive to run.

<a id='57fe8343-0548-43ea-8a4a-39d291ab493a'></a>

44

<a id='b97d38b5-6b04-4440-a696-8d583f8a79d8'></a>

Mastering Multi-Agent Systems )) MAS ((

<a id='d9e74bcd-7b1b-4459-891f-32c4ef61dc3e'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='6c29a790-8919-4cf4-afd8-77cc37a589be'></a>

Chapter 02

<a id='d85dacc1-f0c9-438c-b076-28fea05fcb23'></a>

Why Multi-Agent Systems Fail

<a id='3ff059fc-088a-40cd-bfc4-994fc8c5b99c'></a>

<::logo: [Unknown] [No readable text] [A red, star-like symbol with curved arms]::>

<a id='5dcc2e70-28d2-4d1c-a0f9-cd26888cbb25'></a>

The Decision Framework

<a id='0180b0fd-fe78-4a63-bb83-cf963d6a460d'></a>

Before you build a multi-agent system,
walk through these questions in order:

<a id='967599d9-bf87-4747-bb43-f21ff012ddb6'></a>

1.
Can better prompt engineering solve this?
In 80% of cases, a well-crafted single agent with good context management beats a multi-agent system. Don't split up complexity unless you haven't tried to simplify it.

<a id='cdd3d1d4-ea53-4557-b2fb-c0ce0c79118d'></a>

Say you want code review automation. One agent with a comprehensive prompt handles syntax checking, logic review, and security scanning faster than three separate agents. The single agent maintains context about the entire codebase while reviewing. Multiple agents would need to share that context repeatedly, which would slow down the process and increase costs without improving quality.

<a id='47409012-89f5-4ef9-907f-0a9c912f825a'></a>

2.

Are your subtasks genuinely independent?
Real independence means zero shared state during processing. If Agent B needs Agent A's output to function, you have sequential tasks with extra overhead.

<a id='f2211934-5da0-4516-ba3a-defe5cfc7b54'></a>

Say you're analyzing 100 quarterly earnings reports. Each agent
processes one company's financials independently. Company A's
analysis doesn't affect Company B's. At the end, you combine findings.
This works because subtasks are genuinely independent.

<a id='90ce9289-982e-43e3-a904-69737ca90ae2'></a>

But if you're writing a report where Section 2 analyzes trends from Section 1, and Section 3 builds recommendations from Section 2, you've created dependencies. You're running sequential tasks with coordination overhead, not parallel work.

<a id='bcd97c76-f838-45b9-958d-5fbfdafdc741'></a>

45

<a id='45b3f551-47d1-4025-8119-49e5ef081b3f'></a>

OOO Mastering Multi-Agent Systems >> MAS (

<a id='7fed64f0-4924-457d-901f-1b3684b663eb'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='e3549eb7-e07a-4c45-85a7-084a7b814b88'></a>

Chapter 02

<a id='08431cf8-2e6f-4dd4-b24d-8d666a4c649c'></a>

Why Multi-Agent Systems Fail

<a id='d5d3a3ff-c96c-49cb-850f-422103b2ecfd'></a>

<::logo: Unknown

A red asterisk-like symbol with curved arms, radiating from a central point, on a white background.::>

<a id='e20df4fa-ea20-4280-aaad-a81e9ef157be'></a>

3. Can you afford the cost increase?
Between coordination overhead, duplicate context, and retry logic, expect to pay 2-5x more than single agents.

<a id='38744846-8894-4ca4-82fe-622af4981570'></a>

The extra cost comes from agents needing overlapping context to work together. Each handoff requires reconstructing relevant information, and verification steps multiply as agents check each other's work.

<a id='aa3d7a58-f155-4758-806d-3ea65600eaca'></a>

4. Is your latency tolerance measured in seconds?
Each agent handoff adds 100-500ms. Five agents can add 2+ seconds to response time.

<a id='c7673c05-47c5-45f0-b99e-31ff809e40e8'></a>

If you're building real-time trading systems, you need responses under
100ms. If you're handling live chat, users expect replies within 1-2
seconds. The extra latency makes multi-agent systems unusable here.

<a id='1d3a22e4-5a80-4972-931f-01c337ff5829'></a>

5. Do you have debugging infrastructure?
When multi-agent systems break, you need to trace through multiple
execution paths, shared state changes, and inter-agent communication logs.

<a id='ffb66bc2-9f1c-49ff-b4bd-77c74bac9283'></a>

When your single agent fails on a database query, you check one error log. When the same failure occurs in a multi-agent system, you may need to investigate the query agent, validation agent, retry logic, and coordinator by piecing together logs from four different components.

<a id='bea914a2-6064-48b5-b715-b473a9f9abce'></a>

Debugging becomes exponentially more complex in production
because failures can originate from any agent, any interaction between
agents, or timing issues in the coordination layer. Without specialized
tooling, you'll spend more time debugging than building features.

<a id='f5a77b09-4e0d-4df4-ae3f-2c3b3fc8d446'></a>

46

<a id='f8d4db21-7b62-4777-b5ea-c14f2b1e027b'></a>

OOO Mastering Multi-Agent Systems >> MAS (

<a id='fe39b63d-61f8-4187-8a2a-4896e97cb375'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='e9e35ce1-5475-4341-aeb5-cb73039f6ce3'></a>

Chapter 02

<a id='5b00114c-4b70-48af-b956-20affbdaa50f'></a>

Why Multi-Agent Systems Fail

<a id='0cf9c3cb-afee-4acf-b7f8-2cb96286d622'></a>

<::logo: [Unknown] [] [A red asterisk-like symbol with four curved arms]::>

<a id='a9227800-0079-410f-9d2a-832508595851'></a>

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

<a id='b28f85f2-05b5-4da6-8c21-ba9f35a8e46b'></a>

FIGURE 2.2 Single vs Multi-agent systems across different dimensions

<a id='161b7a8d-e729-4b67-acfd-69d3e071ded3'></a>

You can see the pattern in FIGURE 2.2. Read-heavy tasks work better than write-heavy tasks when you're using multi-agent systems. When your agents can work independently and combine findings, multi-agent approaches work well. When your agents need to build something together, coordination costs usually outweigh benefits.

<a id='7858a9f1-f363-42c7-bd8f-f75f0f4fb953'></a>

Let's look at a concrete example to see how these costs play out in practice.

<a id='0397fe54-6e78-4909-8aab-92b67ef3aeba'></a>

47

<a id='a12c9d02-51b0-4112-b577-5e4b34c4de79'></a>

Mastering Multi-Agent Systems >> MAS (

<a id='cfa5deb7-e6b9-4671-b8df-7efdc584bd4d'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='64a0c42b-5179-45e0-91c6-d4a3c118b37e'></a>

Chapter 02

<a id='fb795cfb-dc4f-4275-a027-6c194d651d26'></a>

Why Multi-Agent Systems Fail

<a id='fa193783-94c1-4a8c-86f9-0f94ffd26420'></a>

<::logo: Unknown

A red asterisk-like symbol with curved arms, radiating from a central point, on a white background.::>

<a id='d257cc8d-8fd4-4128-ba7d-6a38af2b70db'></a>

The Cost Reality Check
Consider a customer support system and how the economics work out:

<a id='5443c3b1-17d8-45eb-821e-d00b4d153610'></a>

# Single-Agent Approach

-> One agent reads the ticket, searches documentation, checks account status, and crafts a response
-> Time: 2 seconds
-> Cost: $0.05
-> Debugging: Straightforward trace through one decision path

<a id='cf2058ff-a1c5-4849-8249-cd1e452dc503'></a>

Multi-Agent Approach

*   Triage agent categorizes (0.5s, $0.08)
*   Research agent searches documentation (1s, $0.10)
*   Account agent checks status (0.8s, $0.08)
*   Response agent crafts reply (1s, $0.10)
*   Orchestrator combines everything (0.5s, $0.04)
*   Time: 3.8 seconds
*   Cost: $0.40
*   Debugging: Five different failure points, 10 potential interaction bugs

<a id='4a48220f-3c00-4fd4-99ab-5a63580bba80'></a>

The multi-agent system costs 8x more, takes nearly twice as long, and creates exponentially more ways to fail. The coordination overhead consumes more resources than the actual work. Unless you're handling millions of tickets where parallelization provides massive scale benefits, the single agent wins.

<a id='d88faab1-1346-478f-9d40-bb1cb19dd2df'></a>

48

<a id='edd3a35f-4666-4197-9628-b898748bef58'></a>

OOO Mastering Multi-Agent Systems >> MAS (

<a id='e3c6dd4e-70d4-4795-9c51-71dec74fa716'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='0b098417-a7b0-4743-adbc-e7cb706803c7'></a>

Chapter 02

<a id='b59a664a-325a-43f5-a627-b3f2391b3235'></a>

Why Multi-Agent Systems Fail

<a id='cfa88b94-71af-487d-b063-09e2369cad05'></a>

<::logo: [Unknown] [] [A red star-like symbol with four points, each point resembling a stylized arrow or 'V' shape, is centrally positioned against a white background.]::>

<a id='7c8217b4-ce0b-4c8c-98fa-4e3248d017de'></a>

This pattern holds across domains. Unless you're processing at a massive scale where parallelization provides exponential benefits, a single agent typically wins on cost, speed, and reliability. Most problems that seem like they need multiple agents actually need better prompt engineering and context management for a single agent.

<a id='f758ca42-470d-422f-bc20-2cc505f5a391'></a>

EXERCISE

Think about a current AI workflow in your organization that's not performing well. Map it through the decision framework above:

1. Write down the specific problem: What exactly isn't working?
2. Apply the 5-question framework: Can prompt engineering fix this? Are subtasks independent? Can you afford a 2-5x cost increase? Is latency tolerance in seconds? Do you have debugging infrastructure?
3. Calculate the economics: If your current solution costs $X, are you willing to pay $2-5X for potential improvements?
4. Identify your constraints: What matters most - cost, speed, accuracy, or reliability?

See if your "multi-agent problem" is actually a single-agent optimization problem you can tackle easily.

<a id='6cd0da7c-afb1-4f95-af4b-673fae633b76'></a>

<::logo: Undetermined
49
The number "49" is displayed in a prominent red font, suggesting a possible brand or product identifier::>

<a id='4da5873a-84e3-4ff4-a55e-f2a4015d2202'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='519b0f5c-8aa2-42d4-86f8-63cee96fbfd2'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='72d6345c-520f-4a56-8a29-3da9bc68667b'></a>

Chapter 02

<a id='b4f0b7c7-194e-412b-8eb5-ecd5470884fd'></a>

Why Multi-Agent Systems Fail

<a id='efe83d8d-7da8-4c0c-a31e-4d44596af0d7'></a>

<::logo: [Unknown] [] [A red asterisk-like symbol with four curved arms]::>

<a id='8553afdb-5ee2-4ade-9b97-16e6e57e2261'></a>

Building Visibility Into Your System

<a id='eea53051-3038-4ac6-81b0-dcbba857b956'></a>

Even after you've identified a legitimate
use case for multi-agent systems, you
might face another challenge: a lack
of visibility into agent failures.

<a id='35f16b43-2129-4ed5-ad50-f371ee54df44'></a>

Traditional LLM evaluation is not effective for
debugging agents as they can take completely
different paths to reach the same goal. Your
research agent might retrieve papers in
different orders, make varying numbers of

<a id='0988c532-0c49-4598-8413-b2b734bb6156'></a>

tool calls, or explore alternative approaches
while still producing the same quality output.

<a id='66d6e189-0b1a-4aaf-b0a8-50a55a429b04'></a>

This makes measurement more complex than checking if the final answer matches your expected output. You need to understand what happened at each decision point, why the agent chose specific tools, and how context influenced those choices. Without this visibility, you're optimizing in the dark.

<a id='dc8f32a2-e5a3-408d-b593-267372f3bcda'></a>

Galileo addresses this by tracking three distinct levels:

<a id='ffb59a78-2967-4888-b0f7-830ee6f758f4'></a>

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

<a id='bbd971de-c39d-4fb4-b23f-4611c045351b'></a>

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

<a id='618c35ed-19d2-4bd3-86c6-241c79438644'></a>

3.

System Level:
What patterns exist across sessions?

-> Tracks the number of errors
-> Identifies the latency of API calls
-> Monitors token consumption patterns and costs
-> Detects agents stuck in repetitive loops due to coordination issues

<a id='54a88dbd-0c30-4c93-a064-2d5f8b9eded7'></a>

50

<a id='9c320768-36ae-4ea0-a10c-78743cbb1cc1'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='7f09a39c-95a0-4666-91da-d921a123c1c1'></a>

-> galileo.ai

<!-- PAGE BREAK -->

<a id='72bee6e9-89e3-4286-9db9-c400b05243d2'></a>

Chapter 02

<a id='66ea8dd1-f30b-4173-b7e1-ba8f5657b8a9'></a>

Why Multi-Agent Systems Fail

<a id='d87c676a-b685-491b-9c69-93a09805b23a'></a>

<::logo: [Unknown] [None] [A red star-like symbol with curved points, resembling an asterisk or a stylized flower]::>

<a id='2395df5f-be2b-4b36-81e0-a914fe9d1ed9'></a>

## Process for Continuous Improvement

Reliable multi-agent systems aren't built in one pass. They're refined through systematic observation and targeted fixes. This four-step process helps you identify exactly where coordination breaks down and validate each improvement.

<a id='78f6926a-aecd-44f8-b3c8-dbdbc122a4de'></a>

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

<a id='60c0bbed-6db0-41a0-a705-8a184b92e0af'></a>

FIGURE 2.3 Action Completion Scoring

<a id='92761e26-52af-4f85-b78f-c07000492a15'></a>

As part of session-level analysis, use Action Completion (FIGURE 2.3)
and Action Advancement to measure overall goal achievement. The
Trace View lets you replay entire sessions to see how your agents
work together to accomplish user objectives. Each trace shows the
complete execution path and agent interactions at every step.

<a id='ca250ea0-1506-4422-bbb9-9d6862c93477'></a>

51

<a id='bace254c-c681-4b6a-83d8-7f042cc15a36'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='7f71e18a-24bd-4ece-a50b-e407c3e36a38'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='2612e63d-f0d0-4b3a-892a-7d0592206cdb'></a>

Chapter 02

<a id='d46209e2-bafb-4caa-aee5-ab5838ff9189'></a>

Why Multi-Agent Systems Fail

<a id='093e78f7-c4d7-4b39-917e-78c9c8f64a13'></a>

<::logo: Unknown
No readable text
A red asterisk-like symbol with five arms, each arm consisting of two curved lines that meet at a point, arranged in a circular pattern::>

<a id='a0388d47-ff32-420b-8ac2-1fb88bbe9a03'></a>

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

<a id='3e40d079-f0bb-4940-abdb-b2a756c5e31e'></a>

FIGURE 2.4 Tool Selection Scoring

<a id='227d99fc-c8d9-4d58-803b-6b339bc34c66'></a>

As part of step-level analysis, apply Tool Selection Quality (FIGURE 2.4)
and Context Adherence to evaluate individual agent decisions. The
Graph View reveals coordination patterns, showing where agents fail to
communicate properly or choose the wrong approach. Click any node to
see the exact information available to that agent at that decision point.

<a id='219c3776-15e6-4c56-bd6d-eeb6d869c901'></a>

You can use Log Stream Insights for real-time monitoring. It provides instant visibility into multi-agent performance with intelligent pattern detection.
Set up custom filters to monitor specific coordination events, such as when agents fail to share information or when handoffs break down.

<a id='2bb3b60a-68a7-47fc-afca-d750abd9ecd5'></a>

52

<a id='57476eab-4119-4cfd-befb-6cfc476a70dd'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='470de810-975d-4812-84b6-6324360cb433'></a>

->galileo.ai

<!-- PAGE BREAK -->

<a id='8274473d-1e30-405d-b733-62de990cfa90'></a>

Chapter 02

<a id='8d10a5c0-09eb-4fd0-9366-6684c8e3d214'></a>

Why Multi-Agent Systems Fail

<a id='de3897ab-3ad7-4cbc-bd18-d9271523fa2e'></a>

<::logo: [Unknown] [None] [A red asterisk-like symbol with four thick, curved arms extending outwards from a central point]::>

<a id='a6c9eeb8-1a10-4655-bcf8-c9a8d1a331a1'></a>

2. Implement an Iterative Improvement Process
Once you've established baseline metrics, use
them to spot problems and test solutions.

<a id='40ac5641-dfe3-4ba6-a8ed-9a0ae5c8f532'></a>

Identify patterns: Monitor metrics over time using the Latency Chart to spot performance degradation as your system scales. Correlate latency spikes with specific agent interactions or coordination bottlenecks. Galileo's automated insights highlight which agent handoffs consistently cause failures or slowdowns.

<a id='fdc80f65-7d40-4be2-9372-5cc1074a6cb7'></a>

Visualize agent behavior: Compare different execution paths for the same task using Graph View. See how agent coordination strategies lead to different routes and identify which approaches work most efficiently. Export these visualizations for team reviews and documentation.

<a id='05f74bbe-c74a-43c9-8694-d98051cea479'></a>

Test variations: Create different versions of your
agent coordination strategies and use A/B testing to
compare performance. The Trace View allows side-by-
side comparison of different multi-agent approaches,
showing exactly where behaviors diverge.

<a id='13d3ad77-e223-44ae-8833-c604c7d62e9a'></a>

Benchmark against baselines: Compare your multi-agent system against Galileo's evaluation datasets and industry benchmarks. The platform provides pre-built test suites for common agent coordination patterns like parallel processing, sequential workflows, and hierarchical delegation.

<a id='30649328-06fa-4a92-a4c7-31fc14617104'></a>

53

<a id='943a0267-b90f-46a1-a030-5165a87f2c86'></a>

Logo Mastering Multi-Agent Systems )) MAS (

<a id='40768ba6-1fed-4114-85f7-884cd4084bb0'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='948936bb-496f-449a-9fd6-878e07e481ce'></a>

Chapter 02

<a id='bc14acf2-ae3f-4168-bd74-f344046eb34d'></a>

Why Multi-Agent Systems Fail

<a id='b4e138e1-134e-4394-a4ad-879df01caca7'></a>

<::logo: [Unknown] [None] [A red star-like symbol with curved points, resembling an asterisk or a stylized flower]::>

<a id='8917f680-a515-48fc-85be-0b217f50bd89'></a>

3. Apply Specific Optimization Strategies

<a id='82e3d7a1-c6c5-4ba7-ad97-962e171f03e1'></a>

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

<a id='cd2fc891-9793-4f09-becf-fb66a8887fcd'></a>

FIGURE 2.5 Trace View

<a id='cb439f31-185a-4092-8197-487276e11616'></a>

Use the Trace View's collapsible interface (FIGURE 2.5)
to navigate through nested agent calls and interactions.
Each trace shows the complete execution path at that
point, which makes it easy to identify where agents fail to
communicate properly or where coordination breaks down.

<a id='b28ab1b2-e461-411a-b18e-f89ef232cbf6'></a>

54

<a id='72203aee-0566-480c-a5f2-ff0f6341361a'></a>

Abstract logo Mastering Multi-Agent Systems )) MAS (

<a id='88c374c4-5e26-4dc0-ac68-19e047e6e61d'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='40c4c666-a785-4485-986a-4140363ca300'></a>

Chapter 02

<a id='3eab1314-2105-4543-ae61-fe7791a3c273'></a>

Why Multi-Agent Systems Fail

<a id='56b90d5f-8914-4507-8b93-c8c4fa73f47f'></a>

<::logo: [Unknown] [None] [A red abstract symbol resembling a star or asterisk, with eight curved arms pointing outwards from a central point.]::>

<a id='9f2ebf69-9580-4538-903a-0de5c4aacd56'></a>

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

<a id='d4e704c1-6f2c-41fa-a8e3-a796a680b5c1'></a>

FIGURE 2.6 Timeline View

<a id='cba6dd13-7647-4899-851c-6b334c7716ad'></a>

The Timeline View (FIGURE 2.6) breaks down time spent in each phase for
performance optimization:

→ Agent communication latency (identifying slow handoffs between agents)
→ Processing latency (showing when coordination
overhead impacts performance)
→ Generation latency (revealing when response assembly affects speed)

<a id='f8da49eb-cb59-495d-9b3d-c554cb0c6904'></a>

Use these insights to identify which agent interactions create bottlenecks and where you can optimize handoffs.

<a id='70600e05-1c40-4c75-a303-d9245efd7916'></a>

55

<a id='6c945535-1ec8-40e6-90eb-98ffefd986e2'></a>

Mastering Multi-Agent Systems )) MAS ((

<a id='0ade9785-768d-41c9-8aa7-9e9ec763d7fe'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='c5318482-c7cf-40fb-bebb-20c47bc5bcac'></a>

Chapter 02

<a id='c15400e4-7c77-4944-990d-6fb1b6cf83c1'></a>

Why Multi-Agent Systems Fail

<a id='8c4bc55b-8b30-4410-ad15-4d13dc4a5f1d'></a>

<::logo: Unknown
A red abstract starburst or pinwheel shape is centered in the image.::>

<a id='c35b301a-0e95-407b-845c-7321c6dff88b'></a>

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

<a id='e95014d0-37d7-4234-8564-f48039d01842'></a>

FIGURE 2.7 Graph View

<a id='d572239e-67d1-4fa2-96b7-e67362940fef'></a>

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

<a id='cd0dc80a-af56-4231-87b9-f5b35be7e0ca'></a>

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

<a id='eff3034b-037b-4fb2-887f-1aa93a20434f'></a>

56

<a id='126af4d7-074b-49d5-8de7-dece583cb576'></a>

OOO Mastering Multi-Agent Systems » MAS (

<a id='9b3313a8-9280-4c8a-b4a3-7955936ee6ac'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='c49e6c2a-46f1-4ce9-b241-705f93d1dbe0'></a>

Chapter 02

<a id='697a5097-9e1c-45dd-9236-b3c6fd694d71'></a>

Why Multi-Agent Systems Fail

<a id='6e6f5193-92f7-4287-b42e-d2900d43b360'></a>

<::logo: [Unknown] [None] [A red asterisk-like symbol with four thick, curved arms extending outwards from a central point]::>

<a id='11639e4a-9845-413d-8117-6af3caebb9c4'></a>

4. Configure Continuous Monitoring and Alerting

Set up alerts based on patterns detected in the Log Stream to catch issues early. Configure thresholds in the Timeline View to notify you when agent coordination exceeds acceptable limits.

<a id='b1b2eeff-70b2-483e-be24-1e1d1111fab6'></a>

**Intelligent Alerting**: Anomaly detection that learns your system's patterns and flags deviations

<a id='8bb31961-f5a2-4657-a056-32c99f2bf72b'></a>

Custom Dashboards: Combine Trace, Graph, and
Timeline views into unified monitoring screens

<a id='d2239d18-7583-480c-953e-5a1cfd92ec4b'></a>

Integrations: Native connectors for LangGraph,
CrewAI, and other frameworks

<a id='00cf03f1-a61c-4b48-bfc3-fe49f884488f'></a>

API Access: Programmatic access to all metrics for custom analysis

<a id='789b0e6c-f5ba-4ebf-a4a4-58306a8d1c2e'></a>

Treat these visualization and monitoring tools as a continuous
feedback loop:

-> Trace View shows what happened
-> Graph View shows why it happened
-> Timeline View shows how fast it happened

<a id='84dc5a38-d556-4e1a-a4b2-0e646b2ce2be'></a>

57

<a id='3c0303b5-4005-4a5c-b8db-630a8c7ee70f'></a>

Mastering Multi-Agent Systems )) MAS ((

<a id='dbf0c92e-20e3-4c10-b976-06a892d8ca4b'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='860bc7ef-65e9-4b2d-8c20-c7f8d1d00e0d'></a>

Chapter 02

<a id='432f0a01-9488-43f5-a633-a54e7b175c54'></a>

Why Multi-Agent Systems Fail

<a id='aafac8f3-e7de-4529-99fb-0182ee7f9128'></a>

<::logo: [Unknown] [None] [A red asterisk-like symbol with four thick, curved arms extending outwards from a central point]::>

<a id='f2f692b8-5f7f-4818-b3c5-7d61fbb29874'></a>

Your Path To Reliability

<a id='3cf681e6-4ea5-4d7d-b9b9-1e6d9bd9234f'></a>

Multi-agent systems aren't inherently bad.
The excitement around them stems from
an intuitive but flawed assumption: if one
smart agent is good, many must be better.

<a id='9939ea9e-694b-4d99-94db-d58039710b4f'></a>

The most successful approach follows a simple progression:

1. Start with single agents and master prompt engineering and context management
2. Understand your task's true dependencies through careful analysis, not assumptions
3. Measure actual parallelization potential with real data, not theoretical benefits
4. Only consider distribution when you hit genuine single-agent limitations

<a id='dc910024-d592-4b89-83f8-b481482de733'></a>

Remember that models are improving
quickly. Don't over-engineer a distributed
solution today for a problem that a
simpler system will solve tomorrow.

<a id='e25d8f98-f689-4bad-8fc4-32eead323089'></a>

The core challenges that cause multi-agent failures, such as context loss, coordination overhead, and debugging complexity, have solutions, as shown in FIGURE 2.8. Galileo addresses these through semantic context compression, standardized agent protocols, and comprehensive observability tools.

<a id='f1e18316-d258-4b01-82b0-948ce2ea0327'></a>

But the fundamental question remains: does your use case justify the complexity?

<a id='1ff92c96-1a06-4884-9ec2-430d7f2b26e6'></a>

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

<a id='c4f15023-c5a6-4dbd-afee-a19d962853f8'></a>

FIGURE 2.8 Galileo's approach to solving multi-agent system challenges

<a id='a8796d40-c4fd-4d45-a49f-9e345592bcf2'></a>

58

<a id='9035055c-dac4-4be7-94c5-a5f9e3e2b3bc'></a>

Mastering Multi-Agent Systems )) MAS ((

<a id='0fa93019-22a0-4d53-8d55-888e503a5505'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='88c11507-70cf-4eb8-8e71-d3ed3d10972f'></a>

Chapter 02

<a id='7b64bd0c-9b07-48bd-a67d-32d1fd2a8153'></a>

Why Multi-Agent Systems Fail

<a id='240740a7-3c42-4174-9060-7158fc9cd8ba'></a>

<::logo: [Unknown] [No readable text] [A red, star-like symbol with four curved arms pointing outwards]::>

<a id='75a71148-c78f-48b1-b02a-c2aa79b80071'></a>

What You've Learned

<a id='c7ae4d44-7c2d-43dd-af89-a14aa67a4404'></a>

You learned why coordination costs often destroy the benefits of specialization and gained a practical framework for deciding whether your use case actually needs multiple agents.

<a id='1786fb68-d6de-4025-9f18-a2fbcff2db97'></a>

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

<a id='96ed5684-45b0-4140-9dc6-ad144de3add4'></a>

TABLE 2.2
Multi-Agent Systems: Where they work and where they may not

<a id='56cde33e-854b-414b-82c6-32247ffd7297'></a>

59

<a id='083efd61-a4a3-4984-a423-bf56d63c7c9c'></a>

Mastering Multi-Agent Systems » MAS (

<a id='50fbc089-c94e-4412-8b06-60f1d24c58f0'></a>

-> galileo.ai

<!-- PAGE BREAK -->

<a id='56be4b7d-6384-497e-88d3-57dad667b5d0'></a>

Chapter 02

<a id='635d7115-81bf-4b05-8e8b-b4dbf9f82555'></a>

Why Multi-Agent Systems Fail

<a id='94754eb2-5f56-49e9-b09d-e3ee890a141b'></a>

<::logo: [Unknown] [No readable text] [A red abstract symbol with four curved elements pointing inwards, forming a star-like shape]::>

<a id='77cdcc48-35ef-4466-83b4-d9c581e1a780'></a>

TABLE 2.2 summarizes the key decision factors from this chapter. Multi-agent systems are effective when you require parallel processing for scalability, validation layers for accuracy, and flexible routing for cost optimization. They struggle when you need sub-second response times, minimal operational complexity, and have tight budget constraints.

<a id='4a2a55b0-82e8-4398-bb36-73e0249fd7c2'></a>

The pressing question is, which specific problems in your stack
would benefit most from specialized agent teams?

<a id='6bd02e13-f1b9-4581-9d17-56fb85f11e80'></a>

Understanding when multi-agent systems fail is only half the battle. When you do decide that coordination costs are worth the benefits, you face another challenge: how do you actually build these systems? The architecture you choose determines not just performance, but which problems become solvable at all.

<a id='53794163-4105-4124-8fd4-8096d3cb3982'></a>

In Chapter 3, we'll explore the four primary architectures for multi-agent systems and how each one creates different capabilities and constraints. You'll learn when centralized orchestration works better than peer-to-peer coordination, how hierarchical systems handle complex workflows, and which frameworks actually deliver on their promises versus which ones add unnecessary complexity.

<a id='1b3c74aa-f774-4cb4-89aa-2d64b3afec17'></a>

60

<a id='0cf7297a-4499-4f6e-97ca-fbea3c85a016'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='7c338e39-6769-4c9a-becd-d7301d11c75b'></a>

→ galileo.ai

<a id='1aa5cff7-120a-4b36-9667-e4e1baf0e83a'></a>

<::logo: [Unknown] [None] [A red outline of a U-turn arrow pointing right]::>

<!-- PAGE BREAK -->

<a id='dea0add1-b224-4c06-aafd-85505545e54a'></a>

<::logo: Galileo
Galileo
A red, abstract star-like shape is to the left of the text "Galileo"::>

<a id='b6803096-435e-4289-81fd-34a4a33e8e46'></a>

<::logo: [N/A]
Chapter
03
Black text "Chapter" above red text "03" on a white background with a subtle textured pattern.::>

<a id='88bea59b-0dbc-4750-9e21-8dcd02f513c5'></a>

Architectures
for Multi-Agent
Systems

<a id='6396286c-496e-4af1-ab83-706bdca89393'></a>

Mastering Multi-Agent Systems

<a id='77643442-98e3-4b64-9659-db4767145dd3'></a>

-> galileo.ai