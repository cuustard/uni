began: 9th October 2024

# SCC.141 Professionalism in Practice

This module of the course is taught by 4 Lecturers:

- Phil Benachour
- Elisa Rubegni
- Mo El-Haj
- Elmira Yadollahi

It aims for me to understand the fundamentals of Professionalism in Practice. This includes...

- ...the principles of responsible computing
- ...legal, social, ethical, and professional challenges

Assessed with Exams and Coursework:

| Task                | When            | Worth |
| ------------------- | --------------- | ----- |
| Groupwork           | Week 10         | 10%   |
| Groupwork           | Week 20         | 20%   |
| Exam                | Summer Term     | 70%   |

---

### Table of Contents

| Week  | Lecture                                                                                                                      | Original Slides                                                                | Noted |
| ----- | ---------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------ | ----- |
| 1     | [Lecture 1 - Module Introduction](#lecture-1---module-introduction)                                                          | [Introduction](/SCC.141.slides/a.introSlides.pdf)                              | ✅    |
| 2     | [Lecture 2 - Systems Development Lifecycle](#lecture-2---systems-development-lifecycle)                                      | [Systems Development Lifecycle](/SCC.141.slides/b.systemsDevLifecycle.pdf)     | ✅    |
| 3     | [Lecture 3 - Requirements & Requirements Engineering](#lecture-3---requirements--requirements-engineering)                   | [Requirements & Requirements Engineering](/SCC.141.slides/c.requirements.pdf)  | 🟧    |
| 4     | [Lecture 4 - Understandong Users, Usability, & User Experience](#lecture-4---understandong-users-usability--user-experience) | [Users, Usability, & User Experience](/SCC.141.slides/d.usersUsabilityUX.pdf)  | ❌    |

---

## Lecture 1 - Module Introduction

Professional issues are areas of debate about ethical or practical conduct that underpin good professional practice in a field.

The word 'ethics' is derived from the Greek word 'ethos' or 'a way of living'. Ethics is a branch of philosophy that is concerned with the behaviour of individuals in society.

The design, manufacturing, and deployment of technology have ethical issues associated with responsibility, safety, security, risk, and trust.

BCS charter requires the establishment and maintenance of a sound ethical foundation for the use of computers. This is done by laying a code of ethics - standards of behaviour that members follow.

### Professional Conduct

- The Public Interest
    - Comply with regulations and laws that govern acting in the public interest
      - Safeguards public health, protects the environment and respects the privacy, security, and well-being of others.
    - Rights of third parties, copyright, and intellectual property
    - Conduct professional activities without discrimination on the grounds of:
      - Sex, sexual orientation, marital status, nationality, colour, race, ethnic origin, religion, age, disability, or any other condition or requirement
    - Promote equal access to the benefits of IT
      - Ensures that IT systems can be used by disabled people or help to develop IT skills in groups of people who do not have them
- Professional Competence and Integrity
    - Continuous professional development
    - Being familiar with the legislation
- Duty to Relevant Authority
    - Carry out professional duties with due care and diligence in accordance with the relevant authority's requirements.
    - Behaving professionally
      - Conflict of Interest
      - Disclosing confidential information without permission
      - Misrepresentation or withholding of information
- Duty to the Profession
    - Settings member's expectations to uphold the reputation and good standing of BCS in particular, and profession in general
    - The duty to support colleagues and help them to develop their skills
    - The need to take responsibility for those that we are managing and help guide their development

## Lecture 2 - Systems Development Lifecycle

A system is a collection of interrelated parts that form a whole. It serves a purpose and a change in one part can change other parts of the system.

> A system development lifecycle is the process of determining how a system can support business needs, designing the system, building it, and delivering it to users.

### Stages of a Systems Development Lifecycle

- Planning
- Analysis
- Design
- Implementation

#### Planning

I need to understand why a system should be developed and how to create a plan for how it will be developed and delivered.

This involves doing a feasibility analysis - technical, economic, and organisational feasibility.

During economic feasibility:

- Development costs (one-time costs)
- Operational costs (ongoing costs)
- Tangible benefits (e.g. revenue)
- Intangible benefits (predicted benefits that may be harder to quantify)

Outputs of the planning stage:

- Define goals for a new system
- Definition of the project's scope
- Assessment of feasibility
- Initial work plan

#### Analysis

I need to understand **who** will use the system, **what** the system will do, and **where**/**when** it will be used.

Stages of Analysis:

1. Problem Analysis
      - Understand the existing solutions/products/situation
      - Breaking down a whole into parts to understand the functions and inter-relationships
      - May include images that capture everything relevant to the system
        - Good mental tool to understand a scenario
        - Useful for discussing with others
        - Useful for identifying stakeholders
        - Suitable for any domain
2. Determine the requirements and characteristics of the system
      - Identify potential improvements
      - Requirements change high-level objectives into precise statements of what a system should do
3. Gather requirements from stakeholders/users
      - Getting more insight into the requirements for the system by gathering data from users

PACT questions:

- **People**: What are the intended users' characteristics and skills?
    - Language
    - Level of skill and expertise
    - Cognitive characteristics such as attention, perception, and memory
    - Physical characteristics such as physical abilities, and accessibility
    - Emotions such as satisfaction, frustration, things being aesthetically pleasing
    - Infrequent vs. frequent users
- **Activities**: How is the activity currently carried out? Why? What can be improved?
    - Goals, tasks, and actions
    - Infrequent vs. frequent tasks?
    - Well-defined or vague goals
    - Continuous or interrupted?
    - Individual or cooperative?
    - Time requirements (e.g. how fast a response is needed)
    - Error Tolerance
- **Context**: what is the environment of the activity?
    - Physical environment
    - Social environment
    - Organisational context
    - When and where activities happen
- **Technology**: what tools are being used currently? How might new developments be used?
    - Input, data, and commands
    - Output
    - Communications between people, devices, speed, etc
    - Size of screen
    - Networked?

#### Design

> System Design is the determination of the overall system architecture that will satisfy the system's essential requirements

- How will the system operate; deciding how to build it
- Involves design of architecture and interface, development of database and file specifications
- Output: System Specification

User interface design defines how users will interact with the system and what kind of inputs and outputs the system accepts and produces.

- **Navigation Mechanisms**: How the user gives instructions to the system (e.g. buttons)
- **Input Mechanisms**: How the system captures information (e.g. forms)
- **Output Mechanisms**: How the system provides information to the user (e.g. reports)

#### Implementation

- Building the system
- Testing the system
- Construction, installation, and support plan (maintainability)

Testing:

1. Unit Testing: testing of each unit or program module separately
2. Integration Testing: checking that things should work together do so without error
3. Acceptance Testing: does the system meet requirements
4. User Testing: system tested with users

Maintenance:

- Not just about maintaining existing functionality. It can involve building new functionality.

### Models

#### Waterfall

![Waterfall Model](/images/waterfallModel.png "Waterfall Model")

Pros:

- Requirements identified at the start.
- Well suited to systems that have high-security needs.
- Clear deliverables
- Easy to arrange tasks as things progress one phase at a time

Cons:

- Time consuming
- Inflexible
- No working software until late stages
- Doesn't adjust to changing requirements
- Difficult to measure progress within stages
- High overheads

#### Rapid Application Development

E.g.:

- Iterative development
- System Prototyping
- Throwaway Prototyping
- Agile
    - Feature oriented
    - Rapid dev and delivery
    - Works in small iterations
    - Deliver in each iteration
    - Review and adapt
    - Make changes

Pros:

- Cheaper and easier to make changes
- Flexible
- Requirements can change and are adaptive
- Useful when users struggle to articulate requirements
- Get user feedback earlier
- Quicker delivery of working software

Cons:

- Can be more challenging to integrate at the end
- Planning can be difficult
- Can be harder to manage
- Less control
- Can be difficult to scale for large systems
- Less documentation

## Lecture 3 - Requirements & Requirements Engineering

### What Are Requirements & Why Are They Important?

A requirement is a clear, testable, and measurable statement, expressed in natural language without jargon, that specifies the intended functionalities, characteristics, or constraints of a product. It specifies what the product should do and ensures it meets the desired operational, functional, and accessibility needs.

Requirements are important because:

- Enables 'time to market with the right product':
    - Streamlines development by providing clear direction.
    - Reduces misunderstandings and rework.
    - Prioritizes critical features for faster delivery.
    - Aligns product with market demands to enhance success.
- Central to delivery:
    - Serves as a reference throughout the project lifecycle.
    - Guides design, development, testing, and deployment.
    - Establishes clear acceptance criteria for evaluation.
    - Aligns expectations with outcomes to ensure stakeholder satisfaction.
- Provide a 'navigation chart' for any project:
    - Helps chart a course from concept to completion.
    - Facilitates tracking progress and informed decision-making.
    - Identifies potential risks early in the process.
    - Allows for adaptability while maintaining focus on goals.

Projects can fail when there are issues with the requirements, such as being incomplete, unrealistic, or constantly changing.

### Types of Requirements

- Functional (functions of the product)
- Non-functional (characteristics of the product)
- Business
- User
- System

#### Functional Requirements

- Defines what the product must do and how it will be implemented
- "the product capabilities or things that product must do for its users"
- Processes the product must perform
    - This relates to what the system must do to be able to perform in order to support a user task
- Information the product must provide
    - This relates to what information the product should contain to enable a process

#### Non-functional Requirements

- Defines the qualities and characteristics the product must have
- "the quality attributes, design & implementation constraints, and external interfaces which a product must have"
- Usability, performance, maintainability, security, legal compliance, etc.

There are 3 types of Non-Functional Requirements:

- **Professional**: These specify how the product must behave
- **Organisational**: Formed from organisational policies and procedures
- **External**: Arise from external factors and its development process

![Type of non-functional requirements](images/nonFunctionalRequirements.png "Diagram showing the types of non-functional requirements")

Examples of non-functional requirements:

- Performance: "It should take less than 3 seconds for a user to receive confirmation of their order"
- Security: "Users must log in to a password-protected area to see their order history"
- Legal: "Data must be stored in compliance with GDPR"

There is another way that non-functional requirements can be categorised:

- Quality: e.g. maintainability, reliability, performance, usability
- Process: how the development process is going to be carried out
- Constraints: from business or operational context

## Lecture 4 - Understandong Users, Usability, & User Experience

### Understanding Users

- Computers used by larg vairety of people (not just techies)
- Problems if products can't be used effectively by intended user groups
- Need t oconsider people's capabilities, limitations, needs, & desires

> "Technology may change rapidly, but people change very slowly. The principles of good design never change." - David A. Norman, (2013). The Design of Everyday Things: Revised and Expanded Edition.

The timeline:

- 1960s: Personal computers grew in popularity, leading to usability concerns
- 1970s: Software engineering shifted its focus towards non-functional requirements like usability and maintainability
- 1980s: The discipline of Human-Computer Interaction (HCI) emerged, concentrating on how people interact with computers

Disciplines of HCI:

- Interaction Design: Intuitive and engaging user interfaces
- Human-Computer Interaction (HIC): Improving how users interact with computers
- User Experience (UX) Design: Enhancing overall user satisfaction and ease of use
- Requirements Engineering: Defining system functions and qualities

We need to consider human abilities and capabilities as well as what they want/need. We must also consider how these might change in users over time. Factors:

- Physiological Aspects: senses, movement, strength, fatigue, etc.
- Cognitive Aspects: attention, memory, learning, cognitive load, etc.
- Affective Aspects: emotional responses

People are complex and unique so we can't predict every need or behaviour, which makes it impossible to design a product for everyone. Users will also struggle to articulate needs so what they want may differ to what they say.

Techniques for considering users:

- Scenarios
  - Stories that describe how users interact with a system
  - Help designers imagine how users will use the system in various ways
- Personas
  - Fictional characters that represent a typical user
  - Based on real data about users

### Usability
