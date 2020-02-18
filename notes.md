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

## Chapter 3: Team First Thinking

### Team As Units
- Work should always be assigned to teams not individuals
- Teams are the smallest entity of delivery within an organisation
- Teams are stables groups of five to nine people

### Scaling with Dunbar's Number
- Depth of relationships someone can have scales according to Dunbar's number
- 5, 15, 50, 150 (roughly triples each time)
- Keeping teams small maximises trust which is essential for high performing teams

### Importance of Long-Lived Teams
- Teams take time to form and be effective
- Typically two to three months
- Adding more people to a team will reduce capacity while the new memger aclimates and the team adjusts

### Team Ownership
- Vital to achieve continuity of care of software
- Teams with strong ownership can think in multiple horizons
  - Immediate future: Results that are near
  - Intermediate future: Expand reach of products and services
  - Far future: Experimentation needed
- If multiple teams have ownership of the the same code the teams will struggle to code effectively
  - E.g. can't decide to tolerate a shortcut now secure in the knowledge this will be addressed in refactorings later

### Teams Over Individuals
- Needs of team always above individuals
- Individuals should always prioritise others on their team
  - E.g. prioritise unblocking other people, try to explore options rather than win arguments

### Team Diversity
- It helps
- Produces better solutions
- More diverse teams will have less of the same assumptions

### Individuals Bonuses Are Bad
- Don't reward individuals, focus on the team
- Incentives should not undermine team cohesion
- Training budgets should be for the whole team to decide what to do not for individuals

### Restricting Team Responsibilities
- Essentials to ensure teams do not exceed their cognitive load
- Three types of cognitive load
  1. Intrinsic: Fundamental to the problem space (What's the format for a function in Language X?)
  2. Extraneous: Environment of the task (What's the correct way to deploy this code?)
  3. Germane: Needs special attention or high perfomrance (How should this service interact with it dependencies?)
- Organisations should work to reduce intrinsic cognitive load and eliminate extraneous cognitive load
- Real value is in germane cognitive load

### Relative Domain Complexity
- Teams are overloaded when unable to be effective and respond in a timely fashion
- Different domains have varying levels of complexity
- Can be useful to split teams up

### 3 Types Of Domains
1. Simple: Clear path of action
2. Complicated: Changes need to be analysed
3. Complex: Lots of experimenation and discovery

### Assigning Domains
- Don't split responsbilities for a single large domain across several teams
- Instead split up a large domain into sub-domains and assign to separate teams
- A single team can handle two to three simple domains, though there is a danger they will get bored by their repetitive work
- Teams assigned a complex domain should not work on any other domain
- Teams should not be assigned two complicated domains, better to split the team in two with each each taking one domain

### Team First Not Monolith Or Microservice
- Design software for team load
- Doing this will naturally lead to small, decoupled services

### Optimizing Team Environment
- Team-first working environment
- Minimise distractions
- Goals over process
- Adopt best practices to optimize developer experience
- Use a platform that reduces cognitive load for devs

### Team API
- Code: produced by team
- Versioning: how changes are communicated
- Wiki and documentation: docs such as how-to guides
- Practices and principles: team's preffered way of thinking
- Communication tools: all tools used e.g. Slack, Gmail, Ticketing System
- Work info: current work, next work, priorities
- Other: how other teams interact with the team