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

| Week  | Lecture                                                                                                                                                    | Original Slides                                                                                   | Noted |
| ----- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ----- |
| 1     | [Lecture 1 - Module Introduction](#lecture-1---module-introduction)                                                                                        | [Introduction](/SCC.141.slides/a.introSlides.pdf)                                                 | ✅    |
| 2     | [Lecture 2 - Systems Development Lifecycle](#lecture-2---systems-development-lifecycle)                                                                    | [Systems Development Lifecycle](/SCC.141.slides/b.systemsDevLifecycle.pdf)                        | ✅    |
| 3     | [Lecture 3 - Requirements & Requirements Engineering](#lecture-3---requirements--requirements-engineering)                                                 | [Requirements & Requirements Engineering](/SCC.141.slides/c.requirements.pdf)                     | ✅    |
| 4     | [Lecture 4 - Understandong Users, Usability, & User Experience](#lecture-4---understandong-users-usability--user-experience)                               | [Users, Usability, & User Experience](/SCC.141.slides/d.usersUsabilityUX.pdf)                     | ✅    |
| 5     | [Lecture 5 - Accesesibility](#lecture-5---accessibility)                                                                                                   | [Accessibility](/SCC.141.slides/e.accessibility.pdf)                                              | ✅    |
| 6     | [Lecture 6 - Solving Problems](#lecture-6---solving-problems)                                                                                              | [Solving Problems](/SCC.141.slides/f.solvingProblems.pdf)                                         | ❌    |
| 7     | [Lecture 7 - Intellectual Property, Software Protection, & Limiting Liability](#lecture-7---intellectual-property-software-protection--limiting-liability) | [Intellectual Property, Software Protection, & Limiting Liability](/SCC.141.slides/g.lawShit.pdf) | ✅    |

---

---

## Lecture 1 - Module Introduction

Professional issues are areas of debate about ethical or practical conduct that underpin good professional practice in a field.

The word 'ethics' is derived from the Greek word 'ethos' or 'a way of living'. Ethics is a branch of philosophy that is concerned with the behaviour of individuals in society.

The design, manufacturing, and deployment of technology have ethical issues associated with responsibility, safety, security, risk, and trust.

BCS charter requires the establishment and maintenance of a sound ethical foundation for the use of computers. This is done by laying a code of ethics - standards of behaviour that members follow.

### Professional Conduct

- The Public Interest
  - Comply with regulations and laws that govern acting in the public interest
    - Safeguard public health, protect the environment, and respect the privacy, security, and well-being of others.
  - Respect the rights of third parties, copyright, and intellectual property
  - Conduct professional activities without discrimination on the grounds of:
    - Sex, sexual orientation, marital status, nationality, color, race, ethnic origin, religion, age, disability, or any other condition or requirement
  - Promote equal access to the benefits of IT
    - Ensure that IT systems can be used by disabled people or help to develop IT skills in groups of people who do not have them
- Professional Competence and Integrity
  - Continuous professional development
  - Being familiar with the legislation
- Duty to Relevant Authority
  - Carry out professional duties with due care and diligence in accordance with the relevant authority's requirements.
  - Behave professionally
    - Avoid conflicts of interest
    - Do not disclose confidential information without permission
    - Avoid misrepresentation or withholding of information
- Duty to the Profession
  - Set members' expectations to uphold the reputation and good standing of BCS in particular, and the profession in general
  - Support colleagues and help them to develop their skills
  - Take responsibility for those that we are managing and help guide their development

---

---

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
- **Context**: What is the environment of the activity?
  - Physical environment
  - Social environment
  - Organisational context
  - When and where activities happen
- **Technology**: What tools are being used currently? How might new developments be used?
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

![Waterfall Model](images/waterfallModel.png "Waterfall Model")

| Pros                                                         | Cons                                        |
| ------------------------------------------------------------ | ------------------------------------------- |
| Requirements identified at the start.                        | Time consuming                              |
| Well suited to systems that have high-security needs.        | Inflexible                                  |
| Clear deliverables                                           | No working software until late stages       |
| Easy to arrange tasks as things progress one phase at a time | Doesn't adjust to changing requirements     |
|                                                              | Difficult to measure progress within stages |
|                                                              | High overheads                              |

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

| Pros                                                  | Cons                                            |
| ----------------------------------------------------- | ----------------------------------------------- |
| Cheaper and easier to make changes                    | Can be more challenging to integrate at the end |
| Flexible                                              | Planning can be difficult                       |
| Requirements can change and are adaptive              | Can be harder to manage                         |
| Useful when users struggle to articulate requirements | Less control                                    |
| Get user feedback earlier                             | Can be difficult to scale for large systems     |
| Quicker delivery of working software                  | Less documentation                              |

---

---

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

---

---

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

Usability is the degree to which an interactive product enables specified users to achieve specific goals with ease, efficiency, and satisfaction within a defined context of use. It ensures that the product is intuitive to learn, effective in its functionality, and enjoyable from the user's perspective.

![System Acceptability Tree](images/usabilityTree.png "Diagram showing System Acceptability Tree")

#### Nielsen's Usability Characteristics

- Learnability: easy-to-learn system
- Efficiency: efficient system
- Memorability: memorable system
- Errors: low error rate
- Satisfaction: satisfying to use

#### Methods to Evaluate Usability

1. Inspection Methods (Expert Evaluation)

- Heuristic evaluation: experts check against usability principles
- Walkthroughs: experts simulate user interactions
- Standards/Guidline Checklist: review compliance with standards or guidlines

2. Inquiry Methods (User Evaluation)

- Observations: watch users interact with the system
- Interviews/Focus Groups: gather feedback through discussions
- Questionnaires: collect structured user feedback

3. Testing Methods (User Evaluation)

- Usability Testing: users complete tasks while being observed to identify issues

#### Nielsen's Usability Heuristics

A heuristic is a practical approach to problem-solving. It relies on guidelines, shortcuts, or rule of thimb to find a solution. It aims for a sufficient solution rather than a perfect one.

1. **Simple & Natural Dialogue**: Easy-to-use and intuitive interfaces
2. **Speak The Users' Language**: Use terms & concepts familiar to the uesr
3. **Minimise Memory Load**: Users shouldn't need to remember too many rules to use the system
4. **Consistency**: Actions should always have the same effect
5. **Feedback**: The system should always inform users about its actions and their input
6. **Clearly Marked Exits**: Make it easy to cancel or undo actions to recover from mistakes
7. **Shortcuts**: Provide shortcuts for experienced users to speed up tasks
8. **Good Error Messages**: Error messages should be clear, helpful, and polite
9. **Prevent Errors**: Design the system to avoid mistakes before they happen
10. **Help & Documentation**: Provide easy-to-find, well-structured help, but keep it simple, as most users avoid reading it

| Pros                                                                                          | Cons                                                                       |
| --------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| Quick & inexpensive                                                                           | Requires expertise                                                         |
| Provides fast feedback without need of large user groups, saving time and money               | Needs trained usability experts to be effective                            |
| Fewer ethical/logistical concerns                                                             | Hard to find experts                                                       |
| No need to recruit users or worry about privacy and consent, as experts handle the evaluation | Often identifies minor problems but can overlook larger usability concerns |

#### Survey Measures for Usability

The System Usability Scale (SUS) is often used after usability evaluations to get quantitative feedback from real users on how they perceive the usability of a system.

![The System Usability Scale](images/systemUsabilityScale.png)

#### Usability Testing & Metrics

Usability Testing is often conducted to observe how users interact with the system in real time. Real users are assigned tasks and their performance is measured. Things such as completion time, number of errors, and success rate.

Usability Metrics are key measurements used t oevaluate system usability, focusing on how well and how efficiently userse can complete tasks.

- Effectiveness is measured as the percentage of tasks successfully completed. `(completed tasks / total tasks) * 100`.
- Efficiency is measured by the time taken for users to complete a task. Faster task completion is correlated with a higher efficiency.

### User Experience

UX refers to the overall experience and feelings a user has when interacting with a system, device, or product, including the context of its use. It recognises that technology is no longer just about improving productivity in the workplace but also about creating a satisfying and seamless experience for users. It focuses on how a system feels to the user. User experience (UX) design is the intentional creation of experiences through technology, focusing on how users feel and interact with a product.

- **Why**: Understand the user's needs, emotions, and motivations behind the activity
- **How**: Design the interaction - how the users achieve their goals
- **What**: Determine what activities the product enables users to perform

### Dark Patterns

Dark Patterns are deceptive UI design features that mislead users into making choices that are not in their best interest. The exploit human weaknesses and behaviours for the benefit ofthe service provider. Users often end up taking actions they didn't intend.

- The Roach Motel is a situation in which it is easy for a user to to enter, but very difficult to exit.
- Forced Continuity is when users are required to provide their credit card information to sign up for a free trial. Once over, they are automatically billed without proir notice.
- Bait and Switch is when users into to complete one action, but an undesirable action occurs instead.
- Privacy Zuckering is the practice of designing confusing jargon and user interfaces that deceive users into sharing more personal information than they intend to.

---

---

## Lecture 5 - Accessibility

Accessibility is the concept of whether a product or service can be used by everyone.

Digital Accessibility is the design of and building of websites and web apps that disabled people can interact with in a meaningful and equivalent way.

When considering the user experience and designing a product:

- **Who** is using the product?
- **What** are they doing?
- **Where** are they doing it?
- **When** are they doing it?
- **Why** are they doing it?
- **How** are they doing it?

Usability is a part of usefulness which has two key parts:

- **Utility**: Does the system do what users need?
- **Usability**: can users easily use the system's features?

Nielsen's Usability Characteristics:

- **Learnability**: The system should be easy to learn
- **Efficiency**: The system should be efficient to use
- **Memorability**: The system should be easy to remember
- **Errors**: The system should have a low error rate
- **Satisfaction**: The system should be satisfying to use

> "The power of the Web is in its universality. Access by everyone regardless of disability is an essential aspect." - Tim Berners-Lee, W3C Director and inventor of the WWW

Usability features can benefit those without disabilities as well as those with. For example:

- Small-screen devices
- Older people
- Temporary disabilities
- Situational limitations
- Slow internet connections

Accessibility is also important for Businesses:

- Drive innovation
- Enhances the brand
- Extend the market reach
- Minimise the legal risk

### Web Accessibility Principles

- **Perceivable**: Users must be able to percieve all essential information on the screen, and it must be conveyed to multiple senses
- **Operable**: Users must be able to operate the digital product's interface and it can not require interaction that a user cannot perform
- **Understandable**: Users must be able to understand the information andthe operation of the user interface
- **Robust**: Supporting assistive technologies and ensuring that, as users and technology evolves, the product remains accesesible.

---

---

## Lecture 6 - Solving Problems

---

---

## Lecture 7 - Intellectual Property, Software Protection, & Limiting Liability

### Intellectual Property

**Intellectual Property** is any unique product of human intellect that has commercial value.

**Propert Rights**: People have the natural right to things which they remove/create through labour. We can extend this to Intellectual Property. If you 'steal' intellectual property you 'steal' the revenue derived from use of the use rather than the item.

Intellectual Property is protected:

- Protecting Intellectual Property:
  - You can protect your IP by hiding it
  - but then you do not benefit from it.
- Benefits of grant intellectual property rights to:
  - Encourage the createion of valuable ideas or
  - Encourage trade based on ideas
- Intellectual property rights tcompromise:
  - Give authors/inventors exclusive rights
  - But only for a finite period of time

Intellectual Property Rights (IPR) is the name given to legal rights that protect:

- Creative works
- Inventions
- Intangible assets of a business

#### The Rights

- **Copyright**
  - This extends to literary, artistic, and musical works
  - Governed by Copyright, Deisng, & Patents Act 1988 (CDPA)
  - **Copyright Infringement** is the violation of copyright law
- **Patents**
  - A strong form of intellectual property rights and gives the owner the exclusive right of an invention for up to 20 years
  - Protects againts independent development of something based on the same idea
  - The application is long and expensive
  - The invention must be new, involve an inventive step, be capable of industrial application, and fully disclosed
- **Law of confidence**
  - A useful supplement to copyright and patents
  - It protects ideas before they become copyrighted/patented
  - protects information like trade secrets, business know-how, lists of clients and contacts, and ideas not yet expressed in a tangible form
- **Design rights**
  - Protects original designs
- **Trademarks**
  - Sign capable of being represented graphically to distinguish goods/services

#### AI & Intellectual Property:

- Patent law is written assuming a human inventor
- By not granting IPR to AI, companies can not profit from inventions by AI
- If IPR was granted to AI, who would be responsible for it?

#### Piracy

**Piracy** is the act of unfairly trading on a person's creation.
**Digital Piracy** is the act of unfairly trading (downloading) on a person's creation.

- Copyright holder's claim: 1 download == 1 lost sale

Digital Rights Management (DRM) accesses control mechanisms used to restrict medium usage (inhibits usage by multiple parties).

The Digital Economy Act 2017\*\* increases max jail term for internet piracy to 10 years.

### Software Protection

Copying software reduces the purchase of the legitimate software. This leads to decreased income for the producers leading to lower production of new software.

**Open Source** Software allows people to run the program for any prupose, study how the program works, and adapt it, redistribute it with changes too, improve the program and release improvements.

Software copyright is now covered by the CDPA.

The CDPA covers software, preparatory design materials, and databases. This is important for sofware as it restricts the copying of the work, distribtution of copies, and adaptations of it. Performing a restricted act without permissions results in infringement of copyright.

The CDPA has two types of computer-produced work:

- Owner of a copyright is the author of the work unless by employee in the course of his employment
- Author of computer-generated work is the person by whom the arrangements necessary for the creation of the works are undertaken.

Things to remember:

1. Do not copy non-literal parts of computer software
2. Prepare, date, and keep preparatory materials for developement
3. Insert Deliberate Mistakes or redundant code
4. Be aware that copyright extends to the compilation of a program
5. Ensure that employees do not use materials or confidential information from previous emplyoment
6. Honour confidentiality
7. Give credit if adapting Open Source code

### Limiting Liability

- For products and services:
  - Specify a warranty period
  - Specify 'appropriate use'
  - Specify maximum reasonable liability
  - Get liability insurance
- For me:
  - Ensure I follow my emploter's standards and guidelines
  - Ensure thorough and regorous testing

#### Product Liability

**Consumer Protection Act 1987** (CPA) imposese a liability on the producer of a defective product. CPA applies to computer hardware. For examlpe, if a customer buys a disk containing software, the disk is deemed to be a 'product' and is protected. CPA however does not apply to computer software.

#### Contractual Liability

**Suply of Goods and Services Act 1982** (SGSA)

Contract for the suply of services, where a supplier writes software for a client. It does not apply to software sold without some form of contract (licence agreement).

It also binds the software supplier to provide a service with reasonable care. If the supplier fails, they could be liable for damages. The user is bound to the terms of licence.

#### Negligence (Personal Liability)

Imposes liability on a person who has acted carelessly under common law. Liability for negligence in software development can be significant in health-system failure, security-system malfunction, and e-commerce system security loopholes.
