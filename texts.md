<a id='87f2a1aa-f226-4a1e-a73a-997c7b1b0825'></a>

<::logo: Galileo
Galileo
A red abstract star-like symbol with multiple arms to the left of the wordmark.::>

<a id='3c4a19c4-892a-4909-845b-7bec225f972d'></a>

v1.01

<a id='c9b1fcae-f3b9-4179-8048-0a3c1a67145e'></a>

Mastering
Multi-Agent Systems

Real-World Strategies for Multi-Agent Development

<a id='5a0627f7-11de-4019-97ce-cfcd3384dd57'></a>

<::An illustration depicting three people and a dog in a modern, light-filled room. A man on the left, wearing an orange tracksuit and glasses, laughs while sitting cross-legged. A brown and white dog sits in front of him. A woman in a light-colored sweatshirt and pants sits in the middle, holding a large glowing white sphere. Another woman with curly hair, wearing a light blue tracksuit, sits on the right, looking towards the center. All three individuals appear to be smiling and engaged. Surrounding them are several smaller glowing white spheres and white orbital lines, creating a visual metaphor for a multi-agent system. In the background, there are elements of a rocky, natural landscape visible through a large window. Overlaid on the image are text elements:

Top left: "galileo.ai"
Top right: "Mastering Multi-Agent Systems >) MAS (" followed by what appears to be a logo or symbol.
Right side: "64%", "88%", "100%"
Bottom right: "Multi-Agent" followed by symbols, and then "Systems" with symbols.
: illustration::>

<a id='e29f5c2f-cc14-4c46-8f94-697f21ea04a9'></a>

Mastering GenAI Series

<a id='52c97be9-1e2f-4e3f-985c-a1c6f6791e95'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='94ab4d0b-5d13-4b4b-9ca0-c49f7aadcfde'></a>

<::logo: Galileo
Galileo
A red abstract star-like symbol with four points is placed to the left of the company name.::>

<a id='74204f95-04d6-4837-8972-37c992c4e572'></a>

<::logo: 
Chapter
02
A white square with "Chapter" in black text and "02" in large red text below it::>

<a id='2c18bd20-347b-44ae-9fc6-9c2017193b56'></a>

# Why Multi-Agent Systems Fail

<a id='c73dcbe4-b80a-42fb-83b5-c6aea95d43f1'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='6fd2cd69-5c5c-4b56-86e7-a3372eb7109c'></a>

-> galileo.ai

<!-- PAGE BREAK -->

<a id='2e2e72b2-e5ea-40e9-9719-fbb3a7010c09'></a>

Chapter

<a id='8a0673c2-357a-4cf8-912c-ff3aaad716bb'></a>

<::logo: [Unknown] [No readable text] [A red asterisk-like symbol with four curved arms]::>

<a id='a7d9ff50-7d23-4eff-a399-d147a46fa5e1'></a>

02 Why Multi-Agent Systems Fail

<a id='d0d90810-c0b3-4734-99fe-1d72aaee4361'></a>

Multi-agent systems look great on paper. You split complex work across specialized agents, add validation layers to catch errors, and process data in parallel for speed. Everyone sees these benefits and starts building, but many of them abandon their projects in a couple of months.

<a id='6fb4c2c2-333b-4a70-a5e2-95b9d7164acf'></a>

But the agents themselves aren't the problem, as individual agents work fine. What adds complexity to these systems is the coordination between them. The system becomes difficult to manage and ends up costing more.

<a id='b61460fc-51d2-47f6-943c-2f7a1099d5c3'></a>

This chapter breaks down the complexities of building a multi-agent
system. You'll see the hidden costs of building them and get a decision
framework to evaluate whether your use case can benefit from it.

<a id='29cebbd4-ebf5-4fd9-a05d-2f86c086aa4e'></a>

34

<a id='fc18c167-2d53-4c16-a76e-2cd40a38f666'></a>

Mastering Multi-Agent Systems )) MAS ((

<a id='8d482f90-303a-47bb-a1ee-72b2c850978e'></a>

-> galileo.ai

<!-- PAGE BREAK -->

<a id='c8fbf30b-880e-4391-ba38-74959d8022ac'></a>

Chapter 02

<a id='304ecc2d-213a-44f6-959e-23d23812e6f1'></a>

Why Multi-Agent Systems Fail

<a id='6a6783db-a823-4628-86db-7f577cfb547d'></a>

<::logo: Unknown

A red asterisk-like symbol with four curved arms pointing outwards from a central point::>

<a id='a991991c-d6c7-4a78-8b61-a3e28ec9d2f2'></a>

Why Coordination Costs Matter

<a id='f35fec3f-6cc8-466e-91e7-247bd60de0ca'></a>

Multi-agent systems struggle when coordination overhead exceeds the value of specialization. Two agents need one communication channel. Three agents need three channels. Four agents need six. Soon, your system becomes harder to manage than it is useful.

<a id='1b53ea90-935e-42d4-8dce-612fb64ebae1'></a>

Consider the last time you worked on a
team project. How much time did you spend
on the actual work versus coordinating
with teammates? Multi-agent systems
face this same challenge, but amplified.

<a id='70346c1d-7d19-47af-a548-8592650b895b'></a>

Here's how it plays out in practice. Imagine a web development workflow where a multi-agent system builds a dashboard:
→ Agent 1 analyzes requirements and decides on the component structure
→ Agent 2 implements the authentication flow
→ Agent 3 builds the data visualization
→ Agent 4 handles API integration

<a id='79e4a4c4-1407-4ba7-b8b8-f11035b9f37f'></a>

Each agent needs selective knowledge from the others. Agent 2 needs the component structure but not the full requirements analysis. Agent 4 needs auth tokens but not implementation details. This creates cascading memory challenges that single agents don't face.

<a id='85605ecf-a3e7-4a91-8025-f8aeaa5d5df9'></a>

35

<a id='aa6e5950-327a-4e3b-8210-34acaaa120a5'></a>

OOO Mastering Multi-Agent Systems >> MAS (

<a id='d9b4da4b-dd33-4ce5-982e-e81705e00f98'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='0e394a5f-ec73-4e08-a915-59b9c3d4c780'></a>

Chapter 02

<a id='9ccb1247-44e8-4f1a-a411-cdbd12f23f23'></a>

Why Multi-Agent Systems Fail

<a id='c7ba1197-90ab-4637-8a91-644b8198aff6'></a>

<::logo: Unknown

A red asterisk-like symbol with six points::>

<a id='e791175d-7d74-439c-be88-049ff9b90650'></a>

Let's look at three high-impact scenarios that
can break multi-agent systems:

<a id='5c40d288-a80a-4d56-9ff5-89e503d711c1'></a>

1.
Memory fragments across agents
Each agent maintains its own context about the project. When Agent 3 needs to understand Agent 1's component decisions, it either gets too much information (driving up costs) or too little (breaking functionality). There's no clean way to share just the relevant details.

<a id='c00e6abe-3b6e-4cec-94a9-68760cc24057'></a>

2.
Operational costs multiply
A simple task that costs $0.10 for a single agent
might cost $1 for a multi-agent system. The extra
cost is due to all the context sharing, handoffs, and
verification required to keep agents synchronized.

<a id='e5597c61-3834-45bd-9b6d-e9895af51ba6'></a>

36

<a id='1a40048f-bbbc-4d5d-b2ea-49eb20aaafea'></a>

OOO Mastering Multi-Agent Systems )) MAS (

<a id='b8384b3d-5d75-4213-9fbc-04bcefdf2257'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='b60d6d4d-7a78-4bfa-b2d4-a6a631602487'></a>

Chapter 02

<a id='00cd07e4-721d-4449-b77b-e09e9852099f'></a>

Why Multi-Agent Systems Fail

<a id='9131bf47-4176-4295-af77-a9190611decd'></a>

<::logo: [Unknown] [] [A red asterisk-like symbol with four curved arms]::>

<a id='fbf4312d-ec74-405c-9bac-6836f841acb2'></a>

3.

Write conflicts cascade

When agents only read data and combine findings, conflicts stay manageable. But when they modify the same system, conflicts multiply (FIGURE 2.1). Agent A creates a user profile structure. Agent B, working independently, creates a different structure. Agent C tries to reconcile both and creates a third. Your system now has three incompatible ways to represent the same user data.

<a id='1e5a7990-6f4c-41c0-8fd7-176aa23d46e9'></a>

Each interaction creates opportunities for context loss, misalignment, or conflicting decisions.

<a id='64acf02d-2c0c-4936-9f3b-93c6da2a8587'></a>

<::Flowchart illustrating parallel write operations, cascading conflicts, and outcomes:

1.  **Create user profile system** (rectangular box) branches into two parallel operations:
    a.  **Agent A:** (blue rectangular box) Creates profile { id, name, email }
    b.  **Agent B:** (blue rectangular box) Creates profile { userld, fullName, contact }

2.  Both Agent A and Agent B feed into **Agent C: Reconciliation** (orange rectangular box) with { profileId, userName, emailAddress }.
    *   A dashed arrow from Agent A to Agent C is labeled "Unaware of B".
    *   A dashed arrow from Agent B to Agent C is labeled "Unaware of A".

3.  Agent C leads to a section titled **Cascading conflicts** (pink background area) which contains four red rectangular boxes, each with an 'x' icon, indicating issues:
    *   option Three incompatible structures: [x]
    *   option Auth expects different fields: [x]
    *   option Database schema mismatched: [x]
    *   option API endpoints broken: [x]

4.  The Cascading conflicts section leads to **System failure** (red rectangular box with a warning icon) with the description: Complete rewrite needed.

5.  System failure leads to **Compare to read operations** (green rectangular box with a checkmark icon), which lists:
    *   Reading is safe
    *   Can combine findings
    *   Writing creates conflicts
:flowchart::>

<a id='e363349d-5699-460e-8678-d5a70cc9bcfc'></a>

FIGURE 2.1 How write operations create cascading conflicts in multi-agent systems

<a id='357da2ee-01ea-472b-8f79-721c1a393c3d'></a>

37

<a id='e26dc3e0-b764-45e1-88e8-4706523ad140'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='c121465c-bac9-411b-844f-690d79324828'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='9d5eb448-37b7-4eed-88ff-9070f30f02ed'></a>

Chapter 02

<a id='dee9cb47-7e4a-41f8-bec0-42abca298998'></a>

Why Multi-Agent Systems Fail

<a id='9be07531-0ce1-4785-9828-a97984aa5024'></a>

<::logo: [Unknown] [None] [A red asterisk-like symbol with four thick, curved arms extending outwards from a central point]::>

<a id='09f82693-2061-4857-a9bf-353907d23ebc'></a>

When Multi-Agent Systems Actually Work

<a id='584919bf-bfcf-4377-b426-8f5e9b2e2950'></a>

Successful multi-agent implementations share specific characteristics most teams overlook.

<a id='3ba45140-101a-49db-9223-1939d214072b'></a>

[Anthropic's research system](https://example.com) is a good starting point. When tasked with analyzing the impacts of climate change, it spawns specialized agents that simultaneously investigate economic effects, environmental data, and policy implications. Each agent processes 50+ sources that a single agent would never have time to handle.

<a id='9461466b-c2be-4745-a909-824382dbffa0'></a>

In this scenario, each agent works
independently, and they don't modify another's
findings. When they finish, an orchestrator
agent (explained in Chapter 3) combines
their findings into a comprehensive report.
There's minimal coordination overhead as
there's no back-and-forth coordination
during the work itself. It's just independent
analysis followed by aggregation.

<a id='7b30b2c0-6c1e-45de-a3a0-863234d446ab'></a>

Here are three specific patterns that most successful implementations use:

<a id='91af8af8-3a41-4494-b10d-e97c41393cb3'></a>

1. Problems that can be parallelized

Multi-agent systems work well when problems can be split into pieces that require no communication during processing.

<a id='c623f423-9683-429e-905f-067272784a82'></a>

Say you have 100 quarterly reports from various companies to analyze
for investment insights. Each agent takes a report and extracts key
metrics: revenue growth, profit margins, debt ratios, and market position.
No agent needs information from another agent's reports. At the end,
you aggregate all findings into a comprehensive market analysis.

<a id='70fe2010-5a00-4e95-910a-d48a4c9d7256'></a>

38

<a id='390364f8-062d-4b95-ab49-b8c676ee3606'></a>

Mastering Multi-Agent Systems )) MAS ((

<a id='def237fa-c1cd-4439-8192-5dc69b62b1c3'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='e36d0817-d89f-4e0c-b425-7baa5091adae'></a>

Chapter 02

<a id='d486d783-80a3-417b-b55f-1245cbe8438b'></a>

Why Multi-Agent Systems Fail

<a id='aeaf5a29-f107-40be-a9ae-6ac7359f43b2'></a>

<::logo: [Unknown] [None] [A red asterisk-like symbol with four thick, curved arms extending outwards from a central point]::>

<a id='9447427c-b71c-4c45-b2af-ea900325befe'></a>

2. Read-heavy, write-light workloads
When agents primarily consume information rather than modify shared state, coordination complexity drops dramatically. Each agent can work independently and combine results at the end.

<a id='36a4843e-bdc3-4019-97df-8a89388c32b2'></a>

Say you're tracking competitor activities across multiple channels. Agent 1 monitors news articles, Agent 2 tracks social media mentions, Agent 3 analyzes patent filings, Agent 4 watches hiring patterns. Each of your agents consumes large amounts of public data and produces intelligence reports. The final analysis combines all reports without agents needing to coordinate during data collection.

<a id='0addc453-2d00-476d-9ffe-99c04d434197'></a>

3.
Explicit coordination rules
Successful implementations use deterministic orchestration with clear handoff points. Anthropic's system doesn't rely on agents figuring out how to work together. It defines exact data formats, interaction protocols, and fallback behaviors through explicit rules.

<a id='fada6357-6bfd-47b9-b981-8893f014878f'></a>

Consider this example from programming and software development. A code change triggers a sequence: Agent 1 runs unit tests and reports pass/fail status, Agent 2 executes integration tests if unit tests pass, Agent 3 performs security scans if integration succeeds, Agent 4 deploys to staging if all checks pass. Each step has clear success criteria, failure protocols, and rollback procedures in place.

<a id='c25b17ca-45a2-417b-875a-b3b85c3ba740'></a>

39

<a id='2e52ff02-129c-4aee-bbda-84ffdf63e6e4'></a>

OOO Mastering Multi-Agent Systems >> MAS (

<a id='7c8b3d77-878c-4313-8933-0272a2262df6'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='59a6741d-45e6-47dd-970a-f6f99f230e86'></a>

Chapter 02

<a id='af547a2d-d989-47f4-9849-188eb5d853ac'></a>

Why Multi-Agent Systems Fail

<a id='bbbf7837-69ac-4353-b5fb-eadb00607e88'></a>

<::logo: Unknown
No readable text
A red asterisk-like symbol with five arms, each arm consisting of two curved lines that meet at a point, arranged in a circular pattern::>

<a id='c08964da-85b9-498f-b00f-33ba3420438e'></a>

Consider this example from programming and software development. A code change triggers a sequence: Agent 1 runs unit tests and reports pass/fail status, Agent 2 executes integration tests if unit tests pass, Agent 3 performs security scans if integration succeeds, Agent 4 deploys to staging if all checks pass. Each step has clear success criteria, failure protocols, and rollback procedures in place.

<a id='656ce5fe-bd17-4d91-8dda-f1bf15c346b1'></a>

Here's a checklist to decide if your use case benefits from a multi-agent setup:

option Can you break down the work into completely independent tasks?: [ ]

option Do agents primarily read and analyze rather than write and modify?: [ ]

option Can results be combined mechanically (concatenation, voting, averaging)?: [ ]

option Is parallel processing speed worth a 2- to 5-fold cost increase?: [ ]

option Can one agent failing be isolated from others?: [ ]

<a id='ef0f2212-c98f-4d03-9be8-f27233018a6c'></a>

Use this checklist to help you determine whether your current problem aligns with multi-agent patterns. Before building any multi-agent system, ask: Will this approach still make sense six months from now?

<a id='2f97b3f9-4566-4c9a-bb0d-8ca9e66f92dd'></a>

This question matters because you're choosing an architecture that needs to work
as models rapidly improve over time. The history of AI suggests that complex
workarounds often become unnecessary overhead when better models emerge.

<a id='85053482-a6c9-4d65-b987-86ba419c0bd4'></a>

40

<a id='5499e5ba-a213-469a-81c6-977c4dae58c8'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='9639e53b-7423-43cf-a090-95b6170c2a5d'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='16057f62-dae3-43b2-931b-48da102d4488'></a>

Chapter 02

<a id='419ea5fd-b48e-4203-8b87-5393d9dc64e1'></a>

Why Multi-Agent Systems Fail

<a id='475b0ba4-443a-4bf7-bb73-1ebcaaa687ed'></a>

<::logo: [Unknown]
A red star-like symbol with four arms, each splitting into two points, is depicted.::>

<a id='5efd281d-95fa-403d-8f64-f35c1a72b3f6'></a>

The Model Evolution Challenge

<a id='32e11663-bb8c-4365-8e0d-3efbba4f6667'></a>

Rich Sutton's Bitter Lesson teaches us that general methods using more computation ultimately win over specialized structures. This principle now collides with multi-agent system design in ways that should make you pause.

<a id='a07ab31f-9588-457c-af87-34c3586b5bf1'></a>

Consider what you're actually doing with multi-agent systems: adding structure to compensate for current model limitations.

*   Can't get your model to handle complex reasoning in one pass? Split it into specialist agents.
*   Is the context window too small? Distribute the load.
*   Is the tool calling unreliable? Create dedicated tool-use agents

<a id='dcc04512-3e1e-4692-bbbd-04c5b6f01ac3'></a>

What happens when these limitations disappear?

<a id='18de1fa4-7af4-4806-ad3f-f6a510e5c4dd'></a>

Think About Your Current Project.

What model limitations are you working around with
your multi-agent architecture? Context windows?
Reasoning capability? Tool use reliability? Write
these down. They're your obsolescence risks.

<a id='804338c8-bf7b-4685-9f86-7fbc77d8561e'></a>

Teams that built complex orchestration layers for GPT-4 found them
unnecessary with GPT-5. Multi-step reasoning chains designed
for Claude 3 became single prompts with Claude 4. The structure
added to work around limitations became the limitation itself.

<a id='4b5a34e8-8df3-4b22-87d3-c703cfe90b1e'></a>

41

<a id='5a17ea44-5dc4-4387-9384-a053e1577d17'></a>

(OOO Mastering Multi-Agent Systems >> MAS (

<a id='c33e18e4-f436-4691-92a0-b6b35379b6f3'></a>

galileo.ai

<!-- PAGE BREAK -->

<a id='00dc17f8-c284-47cc-b55d-050ea59c8c4f'></a>

Chapter 02

<a id='ac3499a8-6700-40e7-b425-635801884e6b'></a>

Why Multi-Agent Systems Fail

<a id='3da3a81d-7cdc-462e-84ac-b6cf320d7280'></a>

<::logo: [Unknown] [] [A red asterisk-like symbol with four curved arms]::>

<a id='3bf9899a-18ce-47e5-b612-a978dfdf60a8'></a>

Boris from Anthropic's Claude Code team gets this. Instead of building elaborate multi-agent systems, he focuses on leveraging model improvements directly. The recent success of single-agent systems beating multi-agent baselines validates this philosophy. Our agent leaderboard shows this pattern clearly: newer models consistently outperform older multi-agent systems while being faster and more cost-effective.

<a id='01c0c907-f744-4f36-b131-cd8cdbfc2793'></a>

This pattern repeats across AI development. You might spend months building a complex multi-agent system only to find that a newer model can handle the same work in a single call. The distributed system you worked so hard to build becomes unnecessary overhead.

<a id='05a307d0-0268-4dd9-b84c-d6b51f79540c'></a>

The smarter approach is to follow Hyung Won Chung's philosophy:

<a id='30fa85be-025f-4035-903d-92d4b752af20'></a>

Add minimal structure:
Instead of building five specialized agents (requirements, authentication,
database, API, frontend), start with two: one for backend logic, one for frontend.
You can always split further if needed, but merging is harder than splitting.

<a id='6de67623-e4a9-41bb-8393-7600e07b1712'></a>

Plan for removal

Write your orchestration code in a separate module that you can delete
entirely later. When a better model arrives, you should be able to delete
the orchestration layerfile and call the underlying functions directly.

<a id='3a17b0fc-0133-4f0a-9dff-2127c5ff0ba1'></a>

## Make boundaries collapsible

Structure your agents so their logic can merge into a single prompt. If Agent A does research and Agent B writes summaries, write them so you can combine both into one "research and summarize" agent later.

<a id='6358ff54-333e-4bfd-b47a-9bc0fc7cf50e'></a>

Separate orchestration from business logic
Your authentication logic should work the same whether it's called by an orchestrator or directly. Keep the business logic separate from the orchestration.

<a id='479e418b-6867-4130-b2f0-132935104cab'></a>

If you're splitting tasks across agents because the model can't
handle complexity, waiting a few months for a better model might be
more effective than building infrastructure you'll have to scrap.

<a id='85504563-ba59-4507-80e3-b93beae47b44'></a>

<::logo: Unknown
42
The numbers "42" are prominently displayed in red, set against a light gray square background.::>

<a id='e8e1b0fc-08da-43b1-8af9-9232ddce56d4'></a>

Abstract logo Mastering Multi-Agent Systems )) MAS (

<a id='5ef88cc0-d88c-4f00-aa64-265bb2205e93'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='7d5c529a-73fd-461b-a42b-29a19e17ed5d'></a>

Chapter 02

<a id='c4e42808-9753-44e2-b24e-a3bc2b3c027e'></a>

Why Multi-Agent Systems Fail

<a id='6cdf4c62-4f65-49c5-8216-5c0fd678a258'></a>

<::logo: [Unknown] [] [A red asterisk-like symbol with four curved arms]::>

<a id='200ce1c8-2e2b-4d9a-b43c-da3cc444b057'></a>

What Frameworks Actually Deliver

<a id='dd568c14-a37a-4335-99dd-ef45ef52a37c'></a>

These days, we have many frameworks
for building agents. They tackle the same
core challenge: how do you coordinate
multiple agents without losing critical
context? The approaches vary, but none
solve the fundamental problem.

<a id='cbc15bed-ba80-4682-b962-01a242fe3811'></a>

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

<a id='87fbc7fe-314b-43bf-99c1-91d9d94033a2'></a>

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

<a id='0418ed9d-1b4d-43ba-8ce4-6b11b930f6e2'></a>

The core problem remains unsolved:
efficient context passing between agents.
Current approaches either share everything
(expensive and slow) or share summaries
(losing critical details). No framework has
solved selective, semantic context transfer
that maintains accuracy while minimizing
overhead. Refer to TABLE 2.1 to see a
comparison of different agentic frameworks.

<a id='42fe40c8-6e44-4d3d-8389-c0c6f2da1b17'></a>

<table id="11-1">
<tr><td id="11-2">Framework</td><td id="11-3">Strength</td><td id="11-4">Limitation</td></tr>
<tr><td id="11-5">CrewAI</td><td id="11-6">Simple role-based setup</td><td id="11-7">Limited context control</td></tr>
<tr><td id="11-8">LangGraph</td><td id="11-9">Full state management</td><td id="11-a">High complexity overhead</td></tr>
<tr><td id="11-b">Swarm</td><td id="11-c">Lightweight coordination</td><td id="11-d">Manual context passing</td></tr>
</table>

<a id='6ba3d717-94e7-486b-9458-d320b633bd42'></a>

TABLE 2.1 Comparison of different agentic frameworks

<a id='49be1279-cc82-465a-8359-0fea0d72974d'></a>

43

<a id='0a082936-80f6-4de5-a28a-b4e54440fdee'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='78d39287-5531-4c22-89a6-ed0f292c9791'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='6eba7d06-e455-4b1c-890a-ee54456ead4f'></a>

Chapter 02

<a id='1900f300-b4e7-4c77-bc33-a60d39b1c8e8'></a>

Why Multi-Agent Systems Fail

<a id='c89e22dc-90e1-4e39-989e-b503bf1e016f'></a>

<::logo: [Unknown] [None] [A red asterisk-like symbol with four thick, curved arms extending outwards from a central point]::>

<a id='1ddbca74-952b-4067-a6e7-85305566ca39'></a>

Consider this workflow: Agent A analyzes a 50-page requirements document
and identifies 12 key components. Agent B needs to implement authentication
based on those requirements. How much context does Agent B actually need?

<a id='1e5ca67a-4938-404e-a2a1-7c697e46011f'></a>

**Option 1: Share everything:**
Agent B gets the full 50-page analysis plus Agent A's complete reasoning chain. This works but costs 10x more in API calls and processing time.

<a id='87e7d60f-e723-4909-9ced-4b6763f5606e'></a>

Option 2: Share summaries:

Agent B gets a condensed version of the key authentication
requirements. This costs less but risks losing the
nuanced decisions that affect implementation.

<a id='80f69bb2-af5f-4a4c-b295-6978cf696577'></a>

Option 3: Selective sharing:
Agent B gets precisely the authentication-relevant
context with enough surrounding detail to make informed
decisions. No framework handles this automatically.

<a id='51cb50ee-fc65-4236-9d28-8cf1ff18149b'></a>

While frameworks can't solve the context efficiency problem, they do handle the mechanics that would otherwise require significant custom development. However, they can't solve the fundamental coordination economics that make most multi-agent systems too expensive to run.

<a id='5bba0423-194e-41a2-803f-cd2806b398a0'></a>

44

<a id='45048318-b213-4627-a114-ebdf62827153'></a>

Mastering Multi-Agent Systems )) MAS ((

<a id='c820d9c1-1af0-487c-bc6d-5b1d79cb661f'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='f36aa6c0-64da-473f-9fb5-a161b4d1e71e'></a>

Chapter 02

<a id='9f7ed3b0-e029-4ae5-bfdc-4cd0984fb5fb'></a>

Why Multi-Agent Systems Fail

<a id='7f39cedd-7c7a-4c2b-b087-d4064cda0dd0'></a>

<::logo: [Unknown] [No readable text] [A red, star-like symbol with curved arms]::>

<a id='6959afd0-9122-459e-be33-4079c7f4e925'></a>

The Decision Framework

<a id='40e629e8-18c6-4bfd-a42d-4a81e7d0b348'></a>

Before you build a multi-agent system,
walk through these questions in order:

<a id='055febcf-ea94-4e2f-a4c2-193ba5f0acab'></a>

1.
Can better prompt engineering solve this?
In 80% of cases, a well-crafted single agent with good context management beats a multi-agent system. Don't split up complexity unless you haven't tried to simplify it.

<a id='f6b3ab50-9f90-4d82-9c50-f7fa9358755d'></a>

Say you want code review automation. One agent with a comprehensive prompt handles syntax checking, logic review, and security scanning faster than three separate agents. The single agent maintains context about the entire codebase while reviewing. Multiple agents would need to share that context repeatedly, which would slow down the process and increase costs without improving quality.

<a id='293ecebe-fbe1-4a36-b886-1feeafce2d34'></a>

2.

Are your subtasks genuinely independent?
Real independence means zero shared state during processing. If Agent B needs Agent A's output to function, you have sequential tasks with extra overhead.

<a id='ab53fc32-08b1-44a8-a5a2-444175793bc7'></a>

Say you're analyzing 100 quarterly earnings reports. Each agent
processes one company's financials independently. Company A's
analysis doesn't affect Company B's. At the end, you combine findings.
This works because subtasks are genuinely independent.

<a id='739d0dd3-1004-4fd1-a246-782ba223a4be'></a>

But if you're writing a report where Section 2 analyzes trends from Section 1, and Section 3 builds recommendations from Section 2, you've created dependencies. You're running sequential tasks with coordination overhead, not parallel work.

<a id='cf69e2e4-7c97-499a-9b31-8d61d384e04b'></a>

45

<a id='51158f42-acbb-4ad5-a696-fb8db411fe11'></a>

OOO Mastering Multi-Agent Systems >> MAS (

<a id='f704665f-545c-4d71-a79a-9be4c9da3e2b'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='9e32db83-0748-423a-b4d4-f53222ad8951'></a>

Chapter 02

<a id='be844b10-a3e7-4844-b6d0-af2cb460ba76'></a>

Why Multi-Agent Systems Fail

<a id='ffc15e66-50db-4360-83a7-06b74afdc0f4'></a>

<::logo: Unknown

A red asterisk-like symbol with curved arms, radiating from a central point, on a white background.::>

<a id='5b84c063-34de-4901-b772-6e6af52eaab6'></a>

3. Can you afford the cost increase?
Between coordination overhead, duplicate context, and retry logic, expect to pay 2-5x more than single agents.

<a id='d8e0853c-e21c-431b-827e-c1e834d51eec'></a>

The extra cost comes from agents needing overlapping context to work together. Each handoff requires reconstructing relevant information, and verification steps multiply as agents check each other's work.

<a id='361243ad-dfd4-448b-a2aa-7d3ef047c909'></a>

4. Is your latency tolerance measured in seconds?
Each agent handoff adds 100-500ms. Five agents can add 2+ seconds to response time.

<a id='2fca6332-7c78-4f17-810f-a21bca6d1f5a'></a>

If you're building real-time trading systems, you need responses under
100ms. If you're handling live chat, users expect replies within 1-2
seconds. The extra latency makes multi-agent systems unusable here.

<a id='ce7abcdc-9753-4e0a-9bc6-b25a746fb9dd'></a>

5. Do you have debugging infrastructure?
When multi-agent systems break, you need to trace through multiple
execution paths, shared state changes, and inter-agent communication logs.

<a id='808ad448-9d1d-4f41-bfdd-55b8445ee454'></a>

When your single agent fails on a database query, you check one error log. When the same failure occurs in a multi-agent system, you may need to investigate the query agent, validation agent, retry logic, and coordinator by piecing together logs from four different components.

<a id='92d04078-e294-4602-8a56-65918c57a13d'></a>

Debugging becomes exponentially more complex in production
because failures can originate from any agent, any interaction between
agents, or timing issues in the coordination layer. Without specialized
tooling, you'll spend more time debugging than building features.

<a id='b6a746c7-2006-448f-acc2-248ec41ffab1'></a>

46

<a id='a028d38c-5699-4aed-9116-e0f5c8ed2745'></a>

OOO Mastering Multi-Agent Systems >> MAS (

<a id='c5b6cd31-5f30-4a94-b309-57a9595a1f5d'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='793704a8-e88a-43b0-9967-9a4b5c0d30f4'></a>

Chapter 02

<a id='f7389f13-9dea-4703-b1e1-18b7d414e246'></a>

Why Multi-Agent Systems Fail

<a id='fac1f803-16c7-4d15-9da3-a7250de8c59e'></a>

<::logo: [Unknown] [] [A red asterisk-like symbol with four curved arms]::>

<a id='8c26f2a6-40d5-49e9-86d2-c475cba0b0e2'></a>

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

<a id='1862f99d-1f8b-400d-b1e4-10e13f7b004e'></a>

FIGURE 2.2 Single vs Multi-agent systems across different dimensions

<a id='c9a76a09-9687-4495-ba43-5ebfde14d579'></a>

You can see the pattern in FIGURE 2.2. Read-heavy tasks work better than write-heavy tasks when you're using multi-agent systems. When your agents can work independently and combine findings, multi-agent approaches work well. When your agents need to build something together, coordination costs usually outweigh benefits.

<a id='2dd3a170-4f9b-4111-968a-8923d46965e1'></a>

Let's look at a concrete example to see how these costs play out in practice.

<a id='25708453-81dc-4afa-aa25-d060c4fcc359'></a>

47

<a id='fab00250-2bfa-466f-9c56-98c7b7482fd2'></a>

Mastering Multi-Agent Systems >> MAS (

<a id='863420c9-bd38-45cc-92ce-3f7810322f81'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='d0c62f59-ad96-462d-9c34-f2b6d8951c01'></a>

Chapter 02

<a id='f0beb292-8b77-41fa-968f-fd4d576c7630'></a>

Why Multi-Agent Systems Fail

<a id='4b57c8b8-837c-41d0-a445-c8e0a08cc81b'></a>

<::logo: Unknown

A red asterisk-like symbol with curved arms, radiating from a central point, on a white background.::>

<a id='496045e5-be0e-4beb-b5eb-462951500616'></a>

The Cost Reality Check
Consider a customer support system and how the economics work out:

<a id='2fa403d4-d524-48f3-9654-414052a1e4af'></a>

# Single-Agent Approach

-> One agent reads the ticket, searches documentation, checks account status, and crafts a response
-> Time: 2 seconds
-> Cost: $0.05
-> Debugging: Straightforward trace through one decision path

<a id='2d75f708-6ec2-4825-be11-4c75e446a223'></a>

Multi-Agent Approach

*   Triage agent categorizes (0.5s, $0.08)
*   Research agent searches documentation (1s, $0.10)
*   Account agent checks status (0.8s, $0.08)
*   Response agent crafts reply (1s, $0.10)
*   Orchestrator combines everything (0.5s, $0.04)
*   Time: 3.8 seconds
*   Cost: $0.40
*   Debugging: Five different failure points, 10 potential interaction bugs

<a id='58b68cb8-87ac-4990-af7f-a8a6b436b745'></a>

The multi-agent system costs 8x more, takes nearly twice as long, and creates exponentially more ways to fail. The coordination overhead consumes more resources than the actual work. Unless you're handling millions of tickets where parallelization provides massive scale benefits, the single agent wins.

<a id='579ccf54-ea8a-4cc8-91f7-002ee27ec2d6'></a>

48

<a id='9b9449c2-f49b-428c-9e93-a1351937e249'></a>

OOO Mastering Multi-Agent Systems >> MAS (

<a id='63443843-0835-4fd5-8ffe-0122b656d1f6'></a>

-> galileo.ai

<!-- PAGE BREAK -->

<a id='0b74c06b-2ef4-43db-87e2-3b197a975d6d'></a>

Chapter 02

<a id='aa63cdcb-6c56-42f0-996d-41c769e77b18'></a>

Why Multi-Agent Systems Fail

<a id='3bee89c1-6cc6-4c7d-ad4d-a37867121a0a'></a>

<::logo: [Unknown] [] [A red star-like symbol with four points, each point resembling a stylized arrow or 'V' shape, is centrally positioned against a white background.]::>

<a id='640657e5-5420-4a98-b973-46211e36ee66'></a>

This pattern holds across domains. Unless you're processing at a massive scale where parallelization provides exponential benefits, a single agent typically wins on cost, speed, and reliability. Most problems that seem like they need multiple agents actually need better prompt engineering and context management for a single agent.

<a id='3a2cd659-c0c1-4a27-8dcb-dc356d697a75'></a>

EXERCISE

Think about a current AI workflow in your organization that's not performing well. Map it through the decision framework above:

1. Write down the specific problem: What exactly isn't working?
2. Apply the 5-question framework: Can prompt engineering fix this? Are subtasks independent? Can you afford a 2-5x cost increase? Is latency tolerance in seconds? Do you have debugging infrastructure?
3. Calculate the economics: If your current solution costs $X, are you willing to pay $2-5X for potential improvements?
4. Identify your constraints: What matters most - cost, speed, accuracy, or reliability?

See if your "multi-agent problem" is actually a single-agent optimization problem you can tackle easily.

<a id='94c8a70a-a996-4297-a843-df34bd834fab'></a>

<::logo: Undetermined
49
The number "49" is displayed in a prominent red font, suggesting a possible brand or product identifier::>

<a id='60a66d6e-8caa-4580-8e06-204f3ebc3cea'></a>

Mastering Multi-Agent Systems )) MAS ((

<a id='bfc1e5c2-2484-4507-adcc-07293554d2f4'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='10d121f7-e982-497a-be70-88ee4c30792f'></a>

Chapter 02

<a id='30c520c2-a879-4eea-b9c3-8bfb4d35dc28'></a>

Why Multi-Agent Systems Fail

<a id='5a4f8afe-8c09-4de9-8317-026b9daffe99'></a>

<::logo: [Unknown] [] [A red asterisk-like symbol with four curved arms]::>

<a id='a1fd0844-e6bb-4c57-ab53-3485054f1399'></a>

Building Visibility Into Your System

<a id='936f2009-64fd-4b8a-b3f4-f3097a175bf2'></a>

Even after you've identified a legitimate
use case for multi-agent systems, you
might face another challenge: a lack
of visibility into agent failures.

<a id='128158df-7b1b-4cd4-8f78-7f6320719eca'></a>

Traditional LLM evaluation is not effective for
debugging agents as they can take completely
different paths to reach the same goal. Your
research agent might retrieve papers in
different orders, make varying numbers of

<a id='d6dd03d4-ae6f-472c-acd7-fe941f88a2a4'></a>

tool calls, or explore alternative approaches
while still producing the same quality output.

<a id='fb902772-d461-471a-b82a-b1663bdb9f91'></a>

This makes measurement more complex than checking if the final answer matches your expected output. You need to understand what happened at each decision point, why the agent chose specific tools, and how context influenced those choices. Without this visibility, you're optimizing in the dark.

<a id='20176386-29a2-419e-be3b-324f925acad3'></a>

Galileo addresses this by tracking three distinct levels:

<a id='f48af505-1b13-47b9-9678-f68898b42230'></a>

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

<a id='b2e87723-e03f-4e1c-b4a5-4522f18e49c8'></a>

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

<a id='6f2dfb3b-c5b3-4676-81b4-658fe701584d'></a>

3.

System Level:
What patterns exist across sessions?

-> Tracks the number of errors
-> Identifies the latency of API calls
-> Monitors token consumption patterns and costs
-> Detects agents stuck in repetitive loops due to coordination issues

<a id='a5e921f1-0234-4114-b838-a6eaf8b65b61'></a>

50

<a id='84781156-7862-44e2-9687-23cb732593a7'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='9fd5551f-d8cd-4177-8da3-27cdd0c7bb90'></a>

-> galileo.ai

<!-- PAGE BREAK -->

<a id='7eaea1c7-288a-4faf-8758-3908f1a923a1'></a>

Chapter 02

<a id='1596c1da-45dd-44c1-a02a-3747c9913cb8'></a>

Why Multi-Agent Systems Fail

<a id='670ede3f-3845-4e71-9151-a0b1f58b054f'></a>

<::logo: [Unknown] [None] [A red star-like symbol with curved points, resembling an asterisk or a stylized flower]::>

<a id='0b92142b-830a-41b0-9887-6b5f6c4308da'></a>

## Process for Continuous Improvement

Reliable multi-agent systems aren't built in one pass. They're refined through systematic observation and targeted fixes. This four-step process helps you identify exactly where coordination breaks down and validate each improvement.

<a id='95b8d233-4ea0-43f0-b1e3-a23cb1d64e6f'></a>

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

<a id='cf390066-c3ae-47a8-98eb-78aa86dcbe7b'></a>

FIGURE 2.3 Action Completion Scoring

<a id='b1a60140-c4aa-4011-9e59-4df8f53fd1b7'></a>

As part of session-level analysis, use Action Completion (FIGURE 2.3)
and Action Advancement to measure overall goal achievement. The
Trace View lets you replay entire sessions to see how your agents
work together to accomplish user objectives. Each trace shows the
complete execution path and agent interactions at every step.

<a id='a7e58bd3-52ec-49c9-ad79-9df4f43ce063'></a>

51

<a id='3332f3ca-4e9f-4b78-8148-2d215fbad848'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='5a7fcbac-7deb-499a-bafd-441241411dd0'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='d2ae0003-c6b6-428f-b3c3-10f0d6e68284'></a>

Chapter 02

<a id='67e614e6-8ffa-43c2-b92f-d1813df28493'></a>

Why Multi-Agent Systems Fail

<a id='64b9338b-1f7a-44f1-94aa-ad8b25357ebf'></a>

<::logo: Unknown
No readable text
A red asterisk-like symbol with five arms, each arm consisting of two curved lines that meet at a point, arranged in a circular pattern::>

<a id='71f0a214-6a69-4de4-80cc-0b642cecea59'></a>

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

<a id='9eb63353-694b-4204-acc3-741ff723ca09'></a>

FIGURE 2.4 Tool Selection Scoring

<a id='8eae5f9f-6d7a-4783-856f-8ebc873e80a6'></a>

As part of step-level analysis, apply Tool Selection Quality (FIGURE 2.4)
and Context Adherence to evaluate individual agent decisions. The
Graph View reveals coordination patterns, showing where agents fail to
communicate properly or choose the wrong approach. Click any node to
see the exact information available to that agent at that decision point.

<a id='0a9b5e8c-698f-40ad-ae76-1ef0996315f4'></a>

You can use Log Stream Insights for real-time monitoring. It provides instant visibility into multi-agent performance with intelligent pattern detection.
Set up custom filters to monitor specific coordination events, such as when agents fail to share information or when handoffs break down.

<a id='6854d8a4-bd62-4812-8278-234660e5b1af'></a>

52

<a id='ce1d52a7-1d53-4a5f-9297-2f2953bc7eae'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='21931324-8e65-406c-a820-1a5e4f111054'></a>

galileo.ai

<!-- PAGE BREAK -->

<a id='a6961e82-81e7-4a50-97cd-f4a757ba365a'></a>

Chapter 02

<a id='fbd5a1f7-04ea-455c-b050-9960f54f676f'></a>

Why Multi-Agent Systems Fail

<a id='d383f2a2-a86b-49ba-b1af-963f37a1945c'></a>

<::logo: [Unknown] [None] [A red asterisk-like symbol with four thick, curved arms extending outwards from a central point]::>

<a id='d5569ed0-0910-439f-a7cc-48aa5f20f44e'></a>

2. Implement an Iterative Improvement Process
Once you've established baseline metrics, use
them to spot problems and test solutions.

<a id='89e3c6a3-a40f-4dfe-a4e9-abf51a9f0d12'></a>

Identify patterns: Monitor metrics over time using the Latency Chart to spot performance degradation as your system scales. Correlate latency spikes with specific agent interactions or coordination bottlenecks. Galileo's automated insights highlight which agent handoffs consistently cause failures or slowdowns.

<a id='b1c240bb-614f-43d1-b057-0aa9fa556dbb'></a>

Visualize agent behavior: Compare different execution paths for the same task using Graph View. See how agent coordination strategies lead to different routes and identify which approaches work most efficiently. Export these visualizations for team reviews and documentation.

<a id='98fe80f8-f8d4-492c-829b-3a92e3f43211'></a>

Test variations: Create different versions of your
agent coordination strategies and use A/B testing to
compare performance. The Trace View allows side-by-
side comparison of different multi-agent approaches,
showing exactly where behaviors diverge.

<a id='e3e13d27-51cd-4af0-a96a-3a4e22ceab92'></a>

Benchmark against baselines: Compare your multi-agent system against Galileo's evaluation datasets and industry benchmarks. The platform provides pre-built test suites for common agent coordination patterns like parallel processing, sequential workflows, and hierarchical delegation.

<a id='69f14e48-65b9-4452-97ce-af479e53a713'></a>

53

<a id='397d934c-db1d-4765-aea7-a8cba98ff943'></a>

Logo Mastering Multi-Agent Systems )) MAS (

<a id='bf64f1c0-1095-4c85-a911-f3492c41ffbb'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='da95e8f0-3792-4a99-87c5-199579468f30'></a>

Chapter 02

<a id='b16efaeb-eedc-4ebf-b46b-d2c5e16a4c0f'></a>

Why Multi-Agent Systems Fail

<a id='ba556ff8-b1fc-4c48-a2ec-5b6a16873a53'></a>

<::logo: [Unknown] [None] [A red star-like symbol with curved points, resembling an asterisk or a stylized flower]::>

<a id='64638f3b-536d-4f2b-ad3a-3c5a58f1b33b'></a>

3. Apply Specific Optimization Strategies

<a id='d5b98511-0201-4f9c-b92b-316496c2b58f'></a>

Multi-Agent Telecom Chatbot / Log Stream: prod
Session: Telecom Agent-2025-09-25 16:

Share

option Messages: [x]
option Latency: [ ]
option Trace graph: [ ]

Condense steps

Session 2 of 6
Configure Metrics

## Supervisor

Type: All
Tool Selection Quality
Q

## Input

JSON

Telecom Agent - 2025-09-25 16:24:37

Trace 80%

Supervisor 33%

transfer_to_plan-advisor-agent

Plan Advisor Agent 67%

pinecone_retrieval

pinecone_retrieval

Plan Advisor Agent 100%

pinecone_retrieval

pinecone_retrieval

Plan Advisor Agent 100%

Trace 100%

Supervisor 100%

```json
{
  "content": "You are a supervisor managing a team of specialized telecom service agents at ConnectTel.",
  "Route customer queries to the appropriate agent based on their needs:
    "needs": [
      "Billing Account Agent: Bill inquiries, payment issues, usage tracking, account balance, charges, credit card information, credit score, etc.",
      "Technical Support Agent: Device troubleshooting, connectivity issues, configuration help, resets",
      "Plan Advisor Agent: Plan recommendations, upgrades, comparing plans, finding savings"
    ],
  "Guidelines:
    "guidelines": [
      "Route queries to the most appropriate specialist agent",
      "For complex issues spanning multiple areas, coordinate between agents",
      "Be helpful and empathetic to customer concerns",
      "If unsure, ask clarifying questions before routing",
      "For general greetings, respond warmly before asking how you can help",
      "If a query doesn't fit any agent's expertise, politely explain our service limitations."
    ]
}
```

```json
{
  "role": "system",
  "content": "check my usage and suggest me how to select the plan",
  "role": "user"
}
```

## Metrics

## Parameters

## Insights

## Agent Quality

Action Completion: Pending...

Tool Selection Quality: 33%

Generated Reasoning
The user's query has two parts: 'check my usage' (which pertains to billing/account information) and 'suggest me how to select the plan' (which is for the plan advisor). The bot chose to transfer the conversation to the plan-advisor-agent. However, the user's query also concerns billing/account usage, which falls under the billing-account--

Auto-improve Metric

## System Metrics

Cost: $0.0007

Latency: 1.48 sec

Num Input Tokens: 279

Num Output Tokens: 14

Num Total Tokens: 293

<a id='d08fed4f-aa01-483d-a1f5-0c0dd979f4ae'></a>

FIGURE 2.5 Trace View

<a id='3bcf394b-ff0d-47ed-9b16-2d56044df47f'></a>

Use the Trace View's collapsible interface (FIGURE 2.5)
to navigate through nested agent calls and interactions.
Each trace shows the complete execution path at that
point, which makes it easy to identify where agents fail to
communicate properly or where coordination breaks down.

<a id='9ddb6e14-02c2-4516-93e2-b8a8d2d2d230'></a>

54

<a id='fd2a1b09-e640-4c52-8f6c-72decce74ca3'></a>

Abstract logo Mastering Multi-Agent Systems )) MAS (

<a id='71249ade-60d5-47f9-b483-da6bc2cb6d76'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='db57623f-ddb0-4ee8-98c3-b0cbd378ffa1'></a>

Chapter 02

<a id='7f5b9639-f2a3-427e-b3e6-27746410fdd2'></a>

Why Multi-Agent Systems Fail

<a id='b1da502a-b89b-4c21-83d2-16190aa66ca0'></a>

<::logo: [Unknown] [None] [A red abstract symbol resembling a star or asterisk, with eight curved arms pointing outwards from a central point.]::>

<a id='636df66d-90ec-4e39-a989-84c82b4d9417'></a>

Multi-Agent Telecom Chatbot / Log Stream: prod ⌄ / Session: Telecom Agent - 2025-09-25 20:...
← /
option Messages: [ ]
option Latency: [x]
option Trace graph: [ ]
<::A timeline chart displaying latency for various processes.
Time axis labels: 0m, 1m.
Processes (Y-axis):
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
The chart shows colored dots and bars representing activity and duration for each process along the timeline.
: timeline chart::>

<a id='d4a80d96-8cc9-4bc4-806b-c54df594e83e'></a>

FIGURE 2.6 Timeline View

<a id='3fb5afca-47a8-47cb-89e9-85a2514f2c6b'></a>

The Timeline View (FIGURE 2.6) breaks down time spent in each phase for
performance optimization:

→ Agent communication latency (identifying slow handoffs between agents)
→ Processing latency (showing when coordination
overhead impacts performance)
→ Generation latency (revealing when response assembly affects speed)

<a id='96196aaa-1aad-4892-9cea-f0dab4356beb'></a>

Use these insights to identify which agent interactions create bottlenecks and where you can optimize handoffs.

<a id='68ccee8d-510f-4306-80c1-90abb8cf9010'></a>

55

<a id='c37bef9a-5129-46f1-988f-208ef5f00fde'></a>

Mastering Multi-Agent Systems )) MAS ((

<a id='d209e91a-1d17-499a-bea4-84e59522f495'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='d51a9d07-1709-48ed-82bb-103fe59d0edb'></a>

Chapter 02

<a id='5e93db7f-f3de-478b-bd5e-bc2b9959e501'></a>

Why Multi-Agent Systems Fail

<a id='83bdfeb2-9066-42dc-b091-d3d29eedf6b3'></a>

<::logo: Unknown
A red abstract starburst or pinwheel shape is centered in the image.::>

<a id='8155c169-c5cb-41bd-a5e2-8fb2029eec34'></a>

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

<a id='e4393a0c-b527-4510-b1ad-0d7fd9015397'></a>

FIGURE 2.7 Graph View

<a id='d32b9e29-4508-44e8-9d19-b96c30aa6fa3'></a>

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

<a id='bab17f1e-5052-44b4-9bc6-b1cc2c7da51d'></a>

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

<a id='1c7ff4bc-0226-4159-a4b9-bdc92e2c4e95'></a>

56

<a id='49ef4471-2e63-4e90-96f8-1fed88380d42'></a>

OOO Mastering Multi-Agent Systems » MAS (

<a id='0651a79c-e70a-4c52-9d1f-3cb769fe2756'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='1cbd171e-a6cd-4ad0-a777-bad463fe78b1'></a>

Chapter 02

<a id='65a0d0e8-eb79-4980-90c3-06883731dcd9'></a>

Why Multi-Agent Systems Fail

<a id='47804f5a-71f7-45ee-b33b-920bbb130b48'></a>

<::logo: [Unknown] [None] [A red asterisk-like symbol with four thick, curved arms extending outwards from a central point]::>

<a id='76983d2e-e1dc-40b8-8975-0122399481e8'></a>

4. Configure Continuous Monitoring and Alerting

Set up alerts based on patterns detected in the Log Stream to catch issues early. Configure thresholds in the Timeline View to notify you when agent coordination exceeds acceptable limits.

<a id='561a1159-c0fe-4370-bc2d-09bb70aa9f35'></a>

**Intelligent Alerting**: Anomaly detection that learns your system's patterns and flags deviations

<a id='207410c5-5279-41ee-9cf7-4093536d263f'></a>

Custom Dashboards: Combine Trace, Graph, and
Timeline views into unified monitoring screens

<a id='90f99f25-0a38-4c7f-91d0-069b8e5f6f48'></a>

Integrations: Native connectors for LangGraph,
CrewAI, and other frameworks

<a id='a376d4b7-9434-4270-8f0a-173711942eab'></a>

API Access: Programmatic access to all metrics for custom analysis

<a id='4a5e1f5b-2f96-4c84-bd9f-6190737c169c'></a>

Treat these visualization and monitoring tools as a continuous
feedback loop:

-> Trace View shows what happened
-> Graph View shows why it happened
-> Timeline View shows how fast it happened

<a id='f2a285c6-4208-481f-a08d-defdeb4cc9b1'></a>

57

<a id='5641fb6d-c780-4a64-815c-c33447854c8d'></a>

Mastering Multi-Agent Systems )) MAS ((

<a id='db5b35f9-0332-49a9-81ad-cdb184f516f8'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='59bb4124-6c91-4c23-825d-f3df809970ec'></a>

Chapter 02

<a id='3b532e50-c406-4bb7-b096-f7452db28e2a'></a>

Why Multi-Agent Systems Fail

<a id='d3417629-7833-4c2c-97f9-17599b0be579'></a>

<::logo: [Unknown] [None] [A red asterisk-like symbol with four thick, curved arms extending outwards from a central point]::>

<a id='a9eabe4b-5b87-4925-a2fe-776309fa39a4'></a>

Your Path To Reliability

<a id='392a8850-9103-47de-b3be-eb75bb7ef835'></a>

Multi-agent systems aren't inherently bad.
The excitement around them stems from
an intuitive but flawed assumption: if one
smart agent is good, many must be better.

<a id='5ed84d67-71a1-4ad2-a9be-d66cb0cc7de6'></a>

The most successful approach follows a simple progression:

1. Start with single agents and master prompt engineering and context management
2. Understand your task's true dependencies through careful analysis, not assumptions
3. Measure actual parallelization potential with real data, not theoretical benefits
4. Only consider distribution when you hit genuine single-agent limitations

<a id='7c29a11b-3a50-440b-b3ea-2206079e7983'></a>

Remember that models are improving
quickly. Don't over-engineer a distributed
solution today for a problem that a
simpler system will solve tomorrow.

<a id='1d093b1d-bdb5-47f7-a895-29f9f13b8fb8'></a>

The core challenges that cause multi-agent failures, such as context loss, coordination overhead, and debugging complexity, have solutions, as shown in FIGURE 2.8. Galileo addresses these through semantic context compression, standardized agent protocols, and comprehensive observability tools.

<a id='997c7ad6-27f7-497f-883a-3dfe0dbdf34c'></a>

But the fundamental question remains: does your use case justify the complexity?

<a id='9d3e8b22-66ee-4e51-8b5e-72bc6ba9d0b1'></a>

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

<a id='5dc5585f-0e03-451a-904a-8bb89ffe6b53'></a>

FIGURE 2.8 Galileo's approach to solving multi-agent system challenges

<a id='2df5bf72-c2ea-4b0b-a724-83106a990b8f'></a>

58

<a id='f69fba56-0106-4174-8d02-f099a41d8a3d'></a>

Mastering Multi-Agent Systems )) MAS ((

<a id='3f73bab4-2598-466e-86ca-ccdf707a2ec6'></a>

→ galileo.ai

<!-- PAGE BREAK -->

<a id='7f665599-4d11-4710-b227-37fd23b9af7e'></a>

Chapter 02

<a id='22154bcc-c492-49b7-b54d-d6b17eec08fa'></a>

Why Multi-Agent Systems Fail

<a id='b880694a-1f5e-45c2-a705-7eb92337ab25'></a>

<::logo: [Unknown] [No readable text] [A red, star-like symbol with four curved arms pointing outwards]::>

<a id='8ef554eb-c046-4b52-a73d-e2d463ad38ca'></a>

What You've Learned

<a id='1e584c2d-50d0-4ad2-90e9-fa9ebdc8cd5b'></a>

You learned why coordination costs often destroy the benefits of specialization and gained a practical framework for deciding whether your use case actually needs multiple agents.

<a id='ce8c2b98-9227-4919-91ed-1c7dcb401b48'></a>

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

<a id='54b5ffc6-0d7f-479e-a308-23900e4e1ee0'></a>

TABLE 2.2
Multi-Agent Systems: Where they work and where they may not

<a id='ebc4c33c-8f64-4365-acec-6359727c6720'></a>

59

<a id='a90ba44d-6921-4cf7-ac09-3196ec14fb0c'></a>

Mastering Multi-Agent Systems » MAS (

<a id='25e59e57-accf-4317-8df5-b7e3f189b5b5'></a>

-> galileo.ai

<!-- PAGE BREAK -->

<a id='9ec1af3e-5408-4b8f-b9a9-f03485357183'></a>

Chapter 02

<a id='2f3e20e1-7662-44ea-afa9-8099f53fe8ce'></a>

Why Multi-Agent Systems Fail

<a id='7b4303cf-6d2b-4100-9480-a809584af1b5'></a>

<::logo: [Unknown] [No readable text] [A red abstract symbol with four curved elements pointing inwards, forming a star-like shape]::>

<a id='c9ff7939-6dca-4cb0-bf45-e695d5080713'></a>

TABLE 2.2 summarizes the key decision factors from this chapter. Multi-agent systems are effective when you require parallel processing for scalability, validation layers for accuracy, and flexible routing for cost optimization. They struggle when you need sub-second response times, minimal operational complexity, and have tight budget constraints.

<a id='19f6dd3b-434a-404b-b453-86190dcc6439'></a>

The pressing question is, which specific problems in your stack
would benefit most from specialized agent teams?

<a id='380dc46e-821f-4e07-b3d4-07f3665420f3'></a>

Understanding when multi-agent systems fail is only half the battle. When you do decide that coordination costs are worth the benefits, you face another challenge: how do you actually build these systems? The architecture you choose determines not just performance, but which problems become solvable at all.

<a id='44a6f980-d5a0-447e-9072-93f8094b331f'></a>

In Chapter 3, we'll explore the four primary architectures for multi-agent systems and how each one creates different capabilities and constraints. You'll learn when centralized orchestration works better than peer-to-peer coordination, how hierarchical systems handle complex workflows, and which frameworks actually deliver on their promises versus which ones add unnecessary complexity.

<a id='63a92cb6-a72c-4bdc-b1b5-965d63c67455'></a>

60

<a id='bd2b16a4-5a83-4c22-a268-43309d2c0068'></a>

Mastering Multi-Agent Systems )) MAS (

<a id='60fd1d97-b492-4335-96be-39263fc60a63'></a>

→ galileo.ai

<a id='15e83813-e185-438b-9685-0acf2a2aea59'></a>

<::logo: [Unknown] [None] [A red outline of a U-turn arrow pointing right]::>

<!-- PAGE BREAK -->

<a id='78822b6d-4568-4fd9-8754-e2e7e4581a79'></a>

<::logo: Galileo
Galileo
A red, abstract star-like shape is to the left of the text "Galileo"::>

<a id='e351bd56-aa54-4b93-a603-cb9d059abe80'></a>

<::logo: [N/A]
Chapter
03
Black text "Chapter" above red text "03" on a white background with a subtle textured pattern.::>

<a id='c281126c-a0cb-4568-94b0-d737daf03fb6'></a>

Architectures
for Multi-Agent
Systems

<a id='56942f6e-198a-43db-bb7a-253cad9cd183'></a>

Mastering Multi-Agent Systems

<a id='0571ae43-8849-4f57-9437-d72674312a60'></a>

-> galileo.ai