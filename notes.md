# Team Topologies

## Chapter 1: The Problem with Org Charts

### Four Types of Teams
- Enabling teams
- Stream aligned team
- Complicated-subsystem team
- Platform team

### Three Interaction Modes
- Collaboration
- X-as-a-service
- Facilitating

### Conway's Law
- Organisations that design systems will produce systems that mirror the communication setup they have

### Cognitive Load
- As with individuals all teams have a max cognitive load
- Team responsbilities naturally grow with team
- Takes effort to ensure teams do not exceed their cognitive load
- Too often teams taking on new responsibilities are treated as if they have full availabilty and cognitive load

### How Exceeding Cognitive Load on Team Lowers Motivation
- Autonomy: decreases because the team is juggling too many requests and responsibilities
- Mastery: decreases as team members become *"jack of all trades, master of none"*
- Purposes: decreases as the therere are too many domains of responsibility

### Cultural and Organisational Changes
- Lessons from Agile, DevOps and Lean Management on tooling and automation are relatively easy to absorb
- Advice on cultural and org changes are harder to visualise and measure

## Chapter 2: Conway's Law and Why It Matters

### Reverse Conway Maneuver
- Ensure the communication lines between teams matches the desired architecture
  -  E.g. to achieve a microservice architecture it's better to have a database developer in each subteam rather than a separate database team which all teams talk to
- *"Team assignements are the first draft of the architecture"* - Michael Nygard

### Team-Scoped Flow
- Microservice example: App Dev --> API Dev --> DB Dev
- Well structured organisations help teams to follow good software architecture principles
  - Loose coupling
  - Clearly bounded responsibilities
  - Clear version compatibility
  - Good cross-team testing

### Software Architects
- Given the importance of team organisation in matching software design technical expertise is needed when organising teams
- Because of software architects also need to be good at managing people

### Restricting Communication
- Best communication between teams is no communication
- If two teams are communicating more than expected it might be a sign of poor software architecture
  - E.g. inadequate API, missing component, etc
- If everyone communicates with everyone this will lead to tighly couple monoliths

### Things To Watch Out For
- Tools
  - Teams that need to collaborate should use the same communication tools
  - Use separate communication tools for teams team that don't need to collaborate (is using different Slack channels for each project an example of this?)
- Complicated-Subsysteam Teams
  - Often created when not needed
  - Only really needed in exceptional circumstances
  - Better to have stream aligned teams
- Regular Reorganisations For Manager's Convenience
  - Violates Conway's Law
  - Very destructive
  - Not aligned with software architecture

  