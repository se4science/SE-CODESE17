## 2017 International Workshop on Software Engineering for High Performance Computing in Computational and Data-Enabled Science and Engineering (SE-CODESE17) *held in conjunction with SC17*

**Sunday, November 12, 2017, 2:00pm - 5:30pm, Room 501**

**Website for this workshop is [https://se4science.github.io/SE-CODESE17/](https://se4science.github.io/SE-CODESE17/)**

[https://sc17.supercomputing.org/session/?sess=sess419](http://se4science.org/workshops/se-codese17/)

[Document for collaborative note taking](https://docs.google.com/document/d/1unkflER1MbbLplkEdOqCy6VW9O52YCE4nQ0ZQzHfFA0/edit)

### Agenda

  - 2:00 - 2:05 -- Welcome and Introductions

  - 2:05 - 2:35 -- Invited Talk: [Software Engineering for Computational Science and Engineering: What Can Work and What Will Not](https://sc17.supercomputing.org/presentation/?id=wkpr154&sess=sess419), Mike Heroux

  - 2:35 - 2:55 -- FULL PAPER: Supporting Software Engineering Practices in the Development of Data-Intensive HPC Applications with the JuML Framework by Markus Götz, Matthias Book, Christian Bodenstein and Morris Riedel

  - 2:55 - 3:30 -- COFFEE BREAK

  - 3:30 - 3:45 -- POSITION PAPER: [Experiences on Clustering High-Dimensional Data using pbdR](https://sc17.supercomputing.org/?post_type=page&p=5407&id=wkpr160&sess=sess419) by Sadika Amreen and Audris Mockus

  - 3:45 - 4:00 -- POSITION PAPER: [Software engineering for efficient development of flexible numerical software](https://sc17.supercomputing.org/?post_type=page&p=5407&id=wkpr170&sess=sess419) by Nathan Wukie and Paul Orkwis

  - 4:00 - 4:15 -- POSITION PAPER: [pFLogger: The parallel Fortran logging framework for HPC applications](https://sc17.supercomputing.org/?post_type=page&p=5407&id=wkpr171&sess=sess419) by Thomas Clune and Carlos Cruz

  - 4:15 - 4:30 -- POSITION PAPER: [Proposal for a Scientific Software Lifecycle Model](https://sc17.supercomputing.org/?post_type=page&p=5407&id=wkpr162&sess=sess419) by Anshu Dubey and Lois McInnes

  - 4:30 - 4:40 -- [Introduction to small group discussion exercise](#discussion-exercise)

  - 4:40 - 5:15 -- [Small Group Discussions](#discussion-exercise)

  - 5:15 - 5:30 -- Small Group Reports and Workshop Wrapup (including [related sessions](#related-sessions) and [code review survey](#code-review-survey))


### Goals of workshop

This workshop is concerned with identifying and applying appropriate software engineering (SE) tools and practices (e.g., code generators, static analyzers, validation + verification (V&V) practices, testing, design approaches, and maintenance practices) to support and ease the development of reproducible Computational and Data-enabled Science & Engineering (CoDeSE) software for High Performance Computing (HPC). Specifically:
  - CoDeSE applications that include large parallel models/simulations of the physical world running on HPC systems.
  - CoDeSE applications that utilize HPC systems (e.g., GPUs computing, compute clusters, or supercomputers) to manage and/or manipulate large amounts of data.

Despite the increasing demand for utilizing HPC for CoDeSE applications, software development for HPC historically attracted little attention from the SE community. Paradoxically, the HPC CoDeSE community has increasingly been adopting SE techniques and tools. Indeed, the development of CoDeSE software for HPC differs significantly from the development of more traditional business information systems, from which many SE best practices and tools have been drawn. These differences appear at various phases of the software lifecycle as described below:

  - Requirements
    - Risks due to the exploration of relatively unknown scientific/engineering phenomena;
    - Supporting reproducible science, particularly on non-deterministic systems;
    - Constant change as new information is gathered;
  - Design
    - Data dependencies within the software;
    - The need to identify the most appropriate parallelization strategy for CoDeSE algorithms;
    - The presence of complex communication among HPC nodes that could degrade performance;
    - Challenges in designing unit and system tests at appropriate scales;
    - The need for fault tolerance and task migration mechanisms to mitigate the need to restart time-consuming computations due to software or hardware errors;
  - V&V
    - Results are often unknown when exploring novel science or engineering areas, algorithms, and datasets;
    - Challenges in applying unit and system tests at appropriate scales;
    - Challenges in retrospectively designing and implementing tests for legacy code;
    - Popular tools often do not work on the latest HPC architectures; they need to be tuned to handle many threads executing at the same time.
  - Deployment
    - Failure of components within running systems is expected due to system size;
    - Continuous integration on platforms with high available and infrequent downtimes;
    - Long system lifespans necessitate porting across multiple platforms

Therefore, in order to identify and develop appropriate tools and practices to support HPC CoDeSE software, members of the SE community, the CoDeSE community and the HPC community must interact with each other. This workshop aims to provide a platform to facilitate this interaction by encourage paper submission and workshop participation by people from all three communities. In addition to presentation and discussion of the accepted papers, significant time during the workshop will be devoted to large and small group discussions among the participants to identify important research questions at the intersection of SE and HPC CoDeSE that are in need of additional study. 

Previous editions of this workshop have focused discussion around a number of interesting topics, including: bit-by-bit vs. scientific validation, reproducibility, unique characteristics of CoDeSE software that affect software development choices, major software quality goals for CoDeSE software, crossing the communication chasm between SE and CoDeSE, measuring the impact of SE on scientific productivity, SE tools and methods needed by the CoDeSE community, and how to effectively test CoDeSE software. 

Motivated by the discussion during the 2015 and 2016 workshops, in this edition of the workshop, we expand the previous workshops by continuing and extending two special focus areas, and emphasizing data-enabled science and engineering as a partner of computational science and engineering, turning CSE into CoDeSE. First, we will place special emphasis on experience reports (including positive, negative, and neutral) of applying software engineering practices to the development of HPC scientific software. It is important to document those successes and failures for the community. Second, as quality assurance is a challenge in the scientific HPC domain, which was specifically discussed in 2016, we will also recruit papers describing quality assurance techniques for HPC science and their use in practice focussing specifically on the challenges of unit testing, system testing, and continuous integration for HPC codes, addressing both legacy code and testing at scale on different architectures and platforms. 

### <a name="discussion-exercise">Discussion Exercise</a>

We will split into small groups to discuss the topic of **software lifecycles models for scientific software**.

Each group will start by discussing one of the following questions:

  1. Are there any stages of the scientific software lifecycle that are fundamentally different/novel from the lifecycle for other software? [Notes from Group 1a](https://docs.google.com/document/d/142OnegzNhdWN8aiVJDsVENHZYkdvngQfi_5Ri_hyato/edit?usp=sharing), [Notes from Group 1b](https://docs.google.com/document/d/1BPllsofhPIo2euf0EEnmSsnmYEsjl9TH8tY3T6-ZxSw/edit?usp=sharing)

  2. Do any commonly identified software lifecycles from industry / open source work well for particular types of scientific software projects? If so, how can these projects be characterised? [Notes from Group 2a](https://docs.google.com/document/d/10YCPBQ-6hQ89ooHFCZnd_edPkzQ9N9h_TNkcYP-u9_I/edit?usp=sharing), [Notes from Group 2b](https://docs.google.com/document/d/1jkmpBdK4vnXadVu9eHq54N0FrxEzgEw6DBJV5PFCWNU/edit#heading=h.u99l3oc3hr7i)

  3. Are there any metrics that help us understand which software development model we should choose for a particular type/size of scientific software project? [Notes from Group 3a](https://docs.google.com/document/d/1uXtIFZqKfloOlHMPJ6MwDJ4sLfOqjIh5NoBxsj2r_qU/edit?usp=sharing), [Notes from Group 3b](https://docs.google.com/document/d/1YkGnhvobVA71-HR3UJnN5upX8L7NpuWdmGcBqdC6xps/edit?usp=sharing)
  
  4. What aspects of the software engineering lifecycle process are difficult for your projects and why? [Notes from Group 4a](https://docs.google.com/document/d/1U_Mo3_lbO3C7ZrpPyipfXlJHehnk-xv0AK0fgJX5vYY/edit?usp=sharing), [Notes from Group 4b](https://docs.google.com/document/d/1DzzskW-yMCZq-66wfoAc-DR-dNCzNP3uuJzPsAzzXL4/edit?usp=sharing)
  
Each group should nominate a facilitator who will take notes in the Google Doc documents linked above (anyone can add to these notes using the link) and keep discussion flowing. 

Your aim as a group is to:
  - (Briefly) share the knowledge that you have on this topic with the rest of your group
  - Record any good examples that inform the discussion
  - Record any places where you think further research or experiences are required to understand the topic
  - Summarize what you think it is important to understand about this topic

In the wrap-up session, each group will be asked to summarise their discussions and report them to the rest of the workshop.
If you think you have completed discussion of your question, please feel free to move on to one of the other questions.
  
### Related Sessions

You might be interested in the following related sessions at SC17:

  - [BoF on Software Engineers: Careers in Research](https://sc17.supercomputing.org/presentation/?id=bof149&sess=sess354), Tuesday 14th November, 12:15 - 13:15, Room 603
  - Booth Talk on Why Persistently Identifying Software is a Good Idea, Tuesday 14th November. 15:00 - 15:15, Booth 1136 (STFC)
  - [BoF on Software Engineering and Reuse in Computational Science and Engineering](https://sc17.supercomputing.org/presentation/?id=bof144&sess=sess374), Tuesday 14th November, 17:15 - 19:00, Room 601
  - [BoF on HPC Carpentry - Practical, Hands-On HPC Training](http://sc17.supercomputing.org/presentation/?id=bof125&sess=sess359), Tuesday 14th November, 17:15 - 19:00, Room 301-303
  - [BoF on Practical Reproducibility by Managing Experiments Like Software](https://sc17.supercomputing.org/presentation/?id=bof177&sess=sess346), Wednesday 15th November, 12:15 - 13:15, Room 601
  - Booth Talk on Why Persistently Identifying Software is a Good Idea, Thursday 14th November. 13:30 - 13:45, Booth 1136 (STFC)
  - [Panel on HPC Software: Is “Cool Stuff” Really Incompatible with Sustainability?](https://sc17.supercomputing.org/?post_type=page&p=5407&id=pan126&sess=sess250), Friday 17th November, 08:30 - 10:00, Room 205-207
  
  
### Code Review Survey

Jeffrey Carver and Nasir Eisty of the University of Alabama are conducting a research study titled “Code Review Process in Computational Science and Engineering Software”. They wish to understand the practices, impacts and barriers of code review technique in Computational Science and Engineering (CSE) software development. 

We encourage workshop participants to complete a web survey that will take about 15 minutes. This survey contains questions about your previous experience with code review process.

Complete the survey at: [http://bit.ly/CodeReview-SC17](http://bit.ly/CodeReview-SC17)

### Committees

#### Organizing Committee

  - [Jeffrey C. Carver](https://sc17.supercomputing.org/?post_type=page&p=5406&fn=jeffrey&ln=carver&uid=293453) - University of Alabama	
  - [Neil Chue Hong](https://sc17.supercomputing.org/?post_type=page&p=5406&fn=neil&ln=chue_hong&uid=761853) - University of Edinburgh	
  - [Selim Ciraci](https://sc17.supercomputing.org/?post_type=page&p=5406&fn=selim&ln=ciraci&uid=160563) - Microsoft	
  - [Daniel S. Katz](https://sc17.supercomputing.org/?post_type=page&p=5406&fn=daniel&ln=katz&uid=061143) - University of Illinois	


#### Program Committee

  - David E. Bernholdt - Oak Ridge National Laboratory
  - Jeff Daily - Pacific Northwest National Laboratory
  - Ali Jannesari - University of California, Berkeley
  - Hilmar Lapp - Duke University
  - Lois Curfman McInnes - Argonne National Laboratory
  - Sarah Mount - King's College London
  - Aleksandra Pawlik - New Zealand eScience Infrastructure
  - Tracy Teal - Data Carpentry
  - Stefan Wagner - University of Stuttgart
  - Ethan White - University of Florida
 
### Code of Conduct
 
All participants are reminded that their involvement in this session is covered by the [SC17 Code of Conduct](http://sc17.supercomputing.org/attendees/code-of-conduct/).
