═══════════════════════════════════════════════════════════════════════════════
                    🤖 AI AGENTS EXPLAINED
                    A Simple Guide for Gemma
═══════════════════════════════════════════════════════════════════════════════

SLIDE 1: WHAT IS AN LLM?
═══════════════════════════════════════════════════════════════════════════════
┌─────────────────────────────────────────────────────────────────────────────┐
│  Think of an LLM like a super-smart person who's read        │
│  EVERYTHING on the internet. Ask them anything!              │
│                                                             │
│  • LLM = Large Language Model                                │
│  • It's been trained on billions of pieces of text           │
│  • It predicts what comes next in a sentence                 │
│  • Ask it anything - it can answer in plain English          │
│                                                             │
│  Example: "What's the weather?" → "It's sunny and 72°"      │
└─────────────────────────────────────────────────────────────────────────────┘

SLIDE 2: BUT WAIT - AN LLM ISN'T PERFECT
═══════════════════════════════════════════════════════════════════════════════
┌─────────────────────────────────────────────────────────────────────────────┐
│  ⚠️ The problem with LLMs:                                   │
│                                                             │
│  1. HALLUCINATIONS - Sometimes they make things up!           │
│     (like a confident person lying)                           │
│                                                             │
│  2. NO MEMORY - Each question is brand new to them             │
│     (starts fresh, no memory of before)                       │
│                                                             │
│  3. LIMITED TOOLS - Can't do math, search web, or send email   │
│     (just talks - can't take action)                           │
│                                                             │
│  That's where AGENTS come in!                                │
└─────────────────────────────────────────────────────────────────────────────┘

SLIDE 3: INTRODUCING AGENTS
═══════════════════════════════════════════════════════════════════════════════
┌────────���────────────────────────────────────────────────────────────────────┐
│  AGENT = LLM + A BRAIN + TOOLS + MEMORY + LOOPS              │
│                                                             │
│           ┌──────────────┐                                 │
│           │  THE AGENT   │ 🎯                                │
│           ├──────────────┤                                 │
│           │ LLM (brain)  │ ← Thinks and decides              │
│           │ Tools        │ ← Can take actions                │
│           │ Memory       │ ← Remembers stuff                 │
│           │ Loop         │ ← Keeps trying until done           │
│           └──────────────┘                                 │
│                                                             │
│  Think: A smart intern with a computer, notes, and to-do list   │
└─────────────────────────────────────────────────────────────────────────────┘

SLIDE 4: HOW AN AGENT WORKS - THE LOOP
═══════════════════════════════════════════════════════════════════════════════
┌─────────────────────────────────────────────────────────────────────────────┐
│                                                             │
│     ┌─────────────┐                                           │
│     │  1. ASK   │ ← "What's the weather?"                     │
│     └─────┬─────┘                                           │
│           │                                                   │
│           ▼                                                   │
│     ┌─────────────┐                                           │
│     │  2. THINK │ ← LLM decides what to do                   │
│     └─────┬─────┘                                           │
│           │                                                   │
│           ▼                                                   │
│     ┌─────────────┐                                           │
│     │  3. ACT    │ ← Call a tool (if needed)                  │
│     └─────┬─────┘                                           │
│           │                                                   │
│     ┌────┴────┐                                             │
│     │ Done?  │                                               │
│     └────┬────┘                                             │
│       Yes │ No                                                │
│     ┌────┘  ▼                                               │
│     │  ┌─────────────┐                                       │
│     │  │ REPEAT!    │ ← Loop back                            │
│     └──┘ └─────────────┘                                       │
│           │                                                   │
│           ▼                                                   │
│     ┌─────────────┐                                           │
│     │  4. ANSWER│ ← Final response                          │
│     └─────────────┘                                           │
│                                                             │
└─────────────────────────────────────────────────────────────────────────────┘

SLIDE 5: TOOLS - WHAT THE AGENT CAN DO
═══════════════════════════════════════════════════════════════════════════════
┌─────────────────────────────────────────────────────────────────────────────┐
│  TOOLS = Things the agent can DO (not just talk about)          │
│                                                             │
│  Example Tools:                                              │
│  ┌─────────────────────────────────────────────────────────┐ │
│  │ 🔍 WEB SEARCH    │ Search the internet                   │ │
│  │ 🧮 CALCULATOR   │ Do math properly                      │ │
│  │ 📧 EMAIL       │ Send emails                          │ │
│  │ 📅 CALENDAR   │ Check/schedule meetings              │ │
│  │ 💻 CODE RUNNER │ Write and run code                   │ │
│  │ �️ BROWSER     │ Browse websites                      │ │
│  └─────────────────────────────────────────────────────────┘ │
│                                                             │
│  Tools are like giving your intern superpowers!               │
│  The agent DECIDES when to use each tool.                     │
└─────────────────────────────────────────────────────────────────────────────┘

SLIDE 6: FUNCTION CALLING = TOOLS
═══════════════════════════════════════════════════════════════════════════════
┌─────────────────────────────────────────────────────────────────────────────┐
│  Function Calling is HOW tools work:                            │
│                                                             │
│  Step 1: Tell agent "You have a calculator tool"                │
│          (with description of what it does)                     │
│                                                             │
│  Step 2: Ask a question needing math                             │
│          "What's 25 * 17?"                                     │
│                                                             │
│  Step 3: Agent RECOGNIZES it needs calculator                  │
│          → Calls calculator with "25*17"                         │
│                                                             │
│  Step 4: Tool returns "425"                                    │
│                                                             ���
│  Step 5: Agent responds "It's 425!"                            │
│                                                             │
│  Magic: The agent figured out WHEN to use the tool!               │
└─────────────────────────────────────────────────────────────────────────────┘

SLIDE 7: SKILLS
═══════════════════════════════════════════════════════════════════════════════
┌─────────────────────────────────────────────────────────────────────────────┐
│  SKILLS = Collections of related tools + instructions          │
│                                                             │
│  Example: RESEARCHER Skill                                   │
│  ┌─────────────────────────────────────────────────────────┐ │
│  │ •web_search tool                                        │ │
│  │ •scrape_website tool                                   │ │
│  │ •summarize tool                                        │ │
│  │ Instructions: "Search → Read → Summarize"              │ │
│  └─────────────────────────────────────────────────────────┘ │
│                                                             │
│  Example: CALCULATOR Skill                                     │
│  ┌─────────────────────────────────────────────────────────┐ │
│  │ •calculator tool                                      │ │
│  │ •unit_converter tool                                  │ │
│  │ Instructions: "Calculate and format results"        │ │
│  └─────────────────────────────────────────────────────────┘ │
│                                                             │
│  Think: Skill = Tool belt + Instructions                        │
└─────────────────────────────────────────────────────────────────────────────┘

SLIDE 8: ROUTERS - DIRECTING TRAFFIC
═══════════════════════════════════════════════════════════════════════════════
┌─────────────────────────────────────────────────────────────────────────────┐
│  ROUTER = Decides WHICH skill/agent to use                     │
│                                                             │
│           User Question                                       │
│                │                                              │
│                ▼                                              │
│         ┌──────────────┐                                     │
│         │   ROUTER    │ ← "What should handle this?"          │
│         └──────┬──────┘                                     │
│                │                                              │
│    ┌───────────┼───────────┬──────────────┐                   │
│    ▼           ▼           ▼            ▼                    │
│  ┌─────┐   ┌─────┐   ┌─────┐     ┌─────┐                    │
│  │Math │   │Search│   │ Email│     │ Code│                    │
│  └─────┘   └─────┘   └─────┘     └─────┘                    │
│                                                             │
│  Like a customer service rep transferring your call           │
│  to the right department!                                    │
└─────────────────────────────────────────────────────────────────────────────┘

SLIDE 9: MEMORY
═══════════════════════════════════════════════════════════════════════════════
┌─────────────────────────────────────────────────────────────────────────────┐
│  MEMORY = How the agent remembers what happened before             │
│                                                             │
│  Types of Memory:                                            │
│                                                             │
│  ┌─────────────────────────────────────────────────────────┐ │
│  │ CONVERSATION MEMORY                                      │ │
│  │ • Remembers chat history                                  │ │
│  │ • "Hi there!" + "Hi!" + "How are you?"                 │ │
│  └─────────────────────────────────────────────────────────┘ │
│                                                             │
│  ┌─────────────────────────────────────────────────────────┐ │
│  │ WORKING MEMORY / STATE                                   │ │
│  │ • Current task progress                                 │ │
│  │ • Collected information                                 │ │
│  │ • What step of the process you're on                    │ │
│  └─────────────────────────────────────────────────────────┘ │
│                                                             │
│  ┌─────────────────────────────────────────────────────────┐ │
│  │ LONG-TERM MEMORY (optional)                              │ │
│  │ • User preferences                                      │ │
│  │ • Past interactions                                    │ │
│  └─────────────────────────────────────────────────────────┘ │
│                                                             │
│  No memory = agent forgets everything each question!           │
└─────────────────────────────────────────────────────────────────────────────┘

SLIDE 10: STATE
═══════════════════════════════════════════════════════════════════════════════
┌─────────────────────────────────────────────────────────────────────────────┐
│  STATE = What's currently happening in the agent                 │
│                                                             │
│       Agent State Example:                                       │
│       ┌─────────────────────────────────────────────────────┐ │
│       │ task: "Research AI trends 2024"                      │ │
│       │ current_step: 2 of 5                                │ │
│       │ collected_info: ["GPT-5 announced", "Anthropic..."]│ │
│       │ status: "working"                                     │ │
│       │ completed: false                                     │ │
│       └─────────────────────────────────────────────────────┘ │
│                                                             │
│  Think of it like a todo list + collected research materials   │
│  All in one place that the agent can see and update!           │
└────────────────────────────────────────────────────��─��──────────────────────┘

SLIDE 11: OBSERVABILITY - SEEING WHAT'S HAPPENING
═══════════════════════════════════════════════════════════════════════════════
┌─────────────────────────────────────────────────────────────────────────────┐
│  OBSERVABILITY = Looking inside the agent to see what it does │
│                                                             │
│  Traditional Software Logs:                                    │
│  "User clicked button" → "API called" → "Success"            │
│                                                             │
│  Agent Traces:                                                │
│  ┌─────────────────────────────────────────────────────────┐ │
│  │ Think step: "I need to calculate 25*17"                │ │
│  │ Tool call: calculator(25*17)                           │ │
│  │ Tool result: 425                                       │ │
│  │ Think step: "Got result, now format answer"             │ │
│  │ Final: "The answer is 425"                            │ │
│  └─────────────────────────────────────────────────────────┘ │
│                                                             │
│  LANGCHAIN TRACING shows every step!                           │
│                                                             │
│  Why it matters:                                              │
│  • Debug when things go wrong                                  │
│  • Verify agent is using right tools                         │
│  • See if it's hallucinating                                │
└─────────────────────────────────────────────────────────────────────────────┘

SLIDE 12: TRADITIONAL VS AGENT OBSERVABILITY
═══════════════════════════════════════════════════════════════════════════════
┌─────────────────────────────────────────────────────────────────────────────┐
│                                                             │
│  TRADITIONAL SOFTWARE         vs        AGENT SYSTEMS          │
│  ──────────────────────                  ──────────────       │
│                                                             │
│  Same input = Same output      →       Same input ≠ Same out   │
│  (eterministic)                    (probabilistic)           │
│                                                             │
│  Logs show WHAT broke           →       Traces show WHY         │
│                                                             │
│  Stack traces                →        Reasoning traces       │
│                                                             │
│  Unit tests work            →        Need SPECIFIC evals    │
│                                                             │
│  Easy to test               →        Need to test behavior   │
│                                                             │
│  Key difference: Agents can make mistakes in NEW ways!       │
└─────────────────────────────────────────────────────────────────────────────┘

SLIDE 13: EVALUATING AGENTS - THE PROBLEM
═══════════════════════════════════════════════════════════════════════════════
┌─────────────────────────────────────────────────────────────────────────────┐
│  Why testing agents is harder than testing regular code:         │
│                                                             │
│  1. PROBABILISTIC OUTPUT                                      │
│     "What's 2+2?" could be:                                  │
│     • "4"                                                    │
│     • "The answer is 4"                                       │
│     • "Two plus two equals four"                               │
│     All are correct!                                          │
│                                                             │
│  2. MULTI-STEP PROCESS                                       │
│     It matters HOW it got there, not just the answer!         │
│                                                             │
│  3. HALLUCINATIONS                                           │
│     Can make up facts! Need to catch this.                    │
│                                                             │
│  4. TOOL USAGE                                               │
│     Did it use the RIGHT tool for the job?                    │
│                                                             │
│  One test isn't enough - need THOUSANDS of cases!              │
└─────────────────────────────────────────────────────────────────────────────┘

SLIDE 14: TYPES OF AGENT EVALS
═══════════════════════════════════════════════════════════════════════════════
┌─────────────────────────────────────────────────────────────────────────────┐
│  1. OUTPUT EVALUATION                                         │
│     • Is the final answer correct?                             │
│     • Format right?                                         │
│     • Helpful?                                              │
│                                                             │
│  2. TRAJECTORY EVALUATION                                     │
│     • Did it use the right TOOLS?                            │
│     • How many steps?                                        │
│     • Efficient path?                                       │
│                                                             │
│  3. RAG EVALUATION (for knowledge)                          │
│     • Retrieved correct info?                               │
│     • Cited sources?                                        │
│     • Not hallucinating?                                    │
│                                                             │
│  4. SAFETY EVALUATION                                       │
│     • No harmful outputs?                                   │
│     • No hallucinations?                                     │
│     • No private info leaked?                               │
└─────────────────────────────────────────────────────────────────────────────┘

SLIDE 15: HOW LANGSMITH HELPS
═══════════════════════════════════════════════════════════════════════════════
┌─────────────────────────────────────────────────────────────────────────────┐
│  LANGSMITH = The tool for evaluating agents                   │
│                                                             │
│  ┌─────────────────────────────────────────────────────────┐ │
│  │ What it does:                                          │ │
│  │ • Records EVERY run with full trace                     │ │
│  │ • Stores test datasets (input + expected)              │ │
│  │ • Runs evaluators on outputs                           │ │
│  │ • Shows pass/fail + scores                          │ │
│  │ • Helps debug issues                                 │ │
│  └─────────────────────────────────────────────────────────┘ │
│                                                             │
│  The pipeline:                                              │
│                                                             │
│  Dataset ──→ Agent ──→ Output ──→ Evaluator ──→ Results    │
│     │                    │                    │                 │
│  Test cases         Predictions       Pass/Fail+Score        │
│                                                             │
│  This is how we know agents are working correctly!            │
└───────────────────────────────────────────────────────────────────────────────┘

═══════════════════════════════════════════════════════════════════════════════
                         🎉 END OF PRESENTATION 🎉
═══════════════════════════════════════════════════════════════════════════════