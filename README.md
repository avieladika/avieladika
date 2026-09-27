# **Aviel Adika**

I build developer tools, AI-assisted applications, and software in Python, Java, and C/C++. I’m looking for junior software engineering opportunities.

## Projects

[**Aptitude**](#aptitude) · [**Learning Agent**](#learning-agent) · [**Interlock**](#interlock) · [**Dad ’n Me**](#dad-n-me) · [**Guess Market**](#guess-market) · [**Donkey Kong**](#donkey-kong) · [**Knight’s Tour**](#knights-tour)

## Aptitude

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-222222?style=for-the-badge)

**Links:** [Project overview](https://github.com/aptitude-stack) · [Publisher](https://github.com/aptitude-stack/publisher) · [Resolver](https://github.com/aptitude-stack/resolver) · [Registry](https://github.com/aptitude-stack/registery)

A collaborative platform for packaging, publishing, discovering, and installing versioned AI skills.

**Challenge:** Skills distributed across repositories and prompts need consistent validation, dependency handling, and repeatable installation.

**Solution:** A publisher prepares and evaluates skill bundles, a registry stores versioned artifacts, and a resolver selects compatible dependencies and creates lockfiles for local installation.

**Includes:** Python CLIs, MCP interfaces, a FastAPI/PostgreSQL registry, policy checks, and lock replay.

**Technical flow:** Author → validate and publish → registry → discover and resolve → lock and install.

---

## Learning Agent

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![SwiftUI](https://img.shields.io/badge/SwiftUI-F05138?style=for-the-badge&logo=swift&logoColor=white)

**Links:** [Repository and setup](https://github.com/avieladika/learning-agent)

A question-answering application for YouTube transcripts, with a Python backend and a SwiftUI macOS client.

**Challenge:** Finding a specific explanation in long videos takes time. Keyword matches can miss related ideas, isolated transcript passages can lose context, and answers without source references are difficult to check.

**Solution:** The application combines keyword and vector retrieval, reranks candidate videos, and expands relevant passages with neighboring transcript chunks. It checks whether the retrieved evidence covers the question and can perform one targeted follow-up retrieval pass before generating an answer.

**Technical flow:** Question → query analysis → channel/video retrieval → transcript context → evidence check → answer and sources.

---

## Interlock

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-222222?style=for-the-badge)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)

**Links:** [Repository and setup](https://github.com/avieladika/interlock)

A development assistant connecting Jira, Confluence, and repository context to requirements, plans, and proposed code changes.

**Challenge:** Implementation context is often spread across tickets, documentation, and source code. Moving directly from a ticket to generated code can leave requirements, assumptions, and acceptance criteria implicit.

**Solution:** Interlock collects context before producing requirements and a plan. Each phase exchanges structured artifacts and checks whether its output is usable before continuing. The final phase produces proposed code changes for review.

**Technical flow:** Jira ticket → context discovery → evidence and requirements → technical plan → proposed changes → structural/syntax checks.

**Scope:** Produces proposed changes with structure and syntax checks; application correctness still requires review and testing.

---

<a id="dad-n-me"></a>

## Dad ’n Me

![C++20](https://img.shields.io/badge/C%2B%2B20-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![SDL3](https://img.shields.io/badge/SDL3-19486A?style=for-the-badge)
![Box2D](https://img.shields.io/badge/Box2D-6B8E23?style=for-the-badge)
![CMake](https://img.shields.io/badge/CMake-064F8C?style=for-the-badge&logo=cmake&logoColor=white)

**Links:** [Repository and setup](https://github.com/avieladika/ECS-Dadn-Me)

A collaborative C++ game exploring Entity Component System architecture, SDL3 rendering, and Box2D physics.

**Challenge:** Game entities combine movement, rendering, collision, health, and temporary combat state. Managing these behaviors together creates a challenge around shared logic and entity lifecycles.

**Solution:** The project represents gameplay state as components and processes behavior through systems and entity factories. The application loop connects that model to graphics, input, and physics.

**Technical flow:** Input → component/state updates → gameplay and physics processing → rendering → transient-state and entity cleanup.

---

## Guess Market

![Java 25](https://img.shields.io/badge/Java_25-ED8B00?style=for-the-badge)
![XML](https://img.shields.io/badge/XML-005FAD?style=for-the-badge)

**Links:** [Repository and setup](https://github.com/avieladika/guess-market)

A Java console prediction-market simulator with XML validation, share pricing, commission handling, and event settlement.

**Challenge:** A market simulation needs consistent pricing, valid input, and a clear accounting model. Mixing these rules with console interaction makes it harder to reason about trades and event settlement.

**Solution:** The application separates a passive market engine from its console interface. XML files are parsed and validated before replacing the current state, while pricing and settlement remain engine responsibilities.

**Technical flow:** XML input → parse and validate → market events → share purchases and history → outcome selection → settlement.

---

## Donkey Kong

![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Windows Console](https://img.shields.io/badge/Windows_Console-0078D6?style=for-the-badge)

**Links:** [Repository and setup](https://github.com/avieladika/Donkey-Kong)

A C++ console game with file-based levels, object-oriented game logic, and recorded-session replay.

**Challenge:** A console game must coordinate movement, collisions, enemies, and progression. Reproducing a game session adds another challenge: inputs, random behavior, and expected results need to be recorded consistently.

**Solution:** The project separates boards, game objects, and game modes into C++ classes. Recording stores input steps and random seeds, while replay uses saved data and can compare game events with expected outcomes.

**Technical flow:** Load level → initialize game objects → process input or replay steps → update collisions/state → record or compare events.

---

<a id="knights-tour"></a>

## Knight’s Tour

![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=white)
![CMake](https://img.shields.io/badge/CMake-064F8C?style=for-the-badge&logo=cmake&logoColor=white)

**Links:** [Repository and setup](https://github.com/avieladika/Chess-knight-positions)

A C implementation of a 5×5 Knight’s Tour search using move arrays, a path tree, and linked lists.

**Challenge:** A valid knight move is easy to enumerate, but finding a complete tour requires exploring alternative paths without revisiting squares. In C, the search also requires explicit handling of dynamically allocated structures.

**Solution:** The program enumerates legal moves, constructs a tree of possible paths from the supplied position, and searches that tree for a route covering the board.

**Technical flow:** Starting square → validate input → enumerate legal moves → construct path tree → search for full coverage → display result.

Aptitude and Dad ’n Me are collaborative projects. The descriptions above summarize each project as a whole.
