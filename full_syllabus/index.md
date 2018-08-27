---
layout: default
title: Brain Networks: Full Syllabus
---
Revised 08/27/2018
## Overview of the course

An essential aspect of the brain is its complex pattern of connectivity between neurons across different areas.  This course will provide a comprehensive overview of the networks of the brain, analyzed from a range of standpoints from the microscopic to the macroscopic, with a particular focus on the organization of the human brain.  Specific topics include brain anatomy, connectomics, structural and functional neuroimaging, graph theory and network science, dynamic models, and causal inference. The course will comprise a combination of lectures, paper discussions, and hands-on analysis exercises.   The first session each week will be composed of lecture and discussion, and the second session will be focused on discussion and hands-on analyses, with students assigned to lead each discussion.

**Prerequisites**:

- Basic knowledge of neuroscience (e.g. equivalent to Psych 50)
- A moderate level of programming experience will be required for hands-on exercises and problem sets. Primary exercises will be in Python.
- A laptop will be necessary for every class.
- An account on github.com will be required for assignment submission - students will be expected to have basic facility with use of git version control system.

**Course Requirements**:  You will need a laptop computer for use in every class.  If you do not have access to a laptop please contact the instructor ASAP and we will help you obtain access to one.  

**Website**: The primary web site for the class is [http://BrainNetworksCourse.github.io](http://BrainNetworksCourse.github.io).  

**Materials**:

Stanford University and its instructors are committed to ensuring that all courses are financially accessible to all students. If you are an undergraduate who needs assistance with the cost of course textbooks, supplies, materials and/or fees, you are welcome to approach me directly. If would prefer not to approach me directly, please note that you can ask the Diversity & First-Gen Office for assistance by completing their [questionnaire on course textbooks & supplies](http://tinyurl.com/jpqbarn) or by contacting Joseph Brown, the Associate Director of the Diversity and First-Gen Office (jlbrown@stanford.edu; Old Union Room 207). Dr. Brown is available to connect you with resources and support while ensuring your privacy.

## Assessment and grading

Grades will be determined as follows:

- Weekly problem sets/discussion questions (50%)
- Final project
    - Proposal (5%) - Due 10/21
    - Final submission (15%) - Due
    - Presentation (5% for stand-up on 10/18, 5% for final presentation)
- Class participation (25%)
    - Each student will be responsible for presenting at least one paper for discussion during the course
    - To get full credit you should also show up for each session having read the assigned materials and be engaged in the discussion

Unless otherwise stated, you can use any published resource you wish to complete the assessments (textbook, Internet, etc).  However, you should not discuss the answers with your fellow students in person or electronically unless instructed to do so by the instructors; sharing answers (including computer code) will be viewed as a violation of the Honor Code.

**Final project**:
Each student will complete a final project in which they use an open dataset to test a hypothesis about brain connectivity.  The final submission should be a github repository with a computational notebook that includes a writeup of the analyses as well as the code and any data needed to execute the code.  Students may work in groups of up to 3 people for the project, but the contribution of each student to the group must be clear and distinct, and group projects are expected to be substantially more involved than individual projects.

**Problem sets**: Most weeks you will be given one written assignment or problem set to complete.  Unless otherwise noted, these will be due at 7 PM on Mondays, submitted via [Github Classroom](https://classroom.github.com/classrooms/42592663-brainnetworkscourse). We will accept late problem sets for up to three days after the PSet is due; after that, no late submissions will be accepted.  For unexcused late submissions, one point will be deducted for each day that the PSet is late.  Excused late submissions must be accompanied by documentation of an official university function within one day of the due date, or a documented medical excuse.

**Excused absences**: If you are going to miss an in-class assessment due to an absence for an official University trip, please alert the TAs *prior to your absence* to schedule a make-up activity.

**Grade disputes**:  Students must wait 24 hours after receiving a grade before they can dispute it, after which disputes must be received within 7 days of receipt of the grade. Grade disputes must be submitted to the instructor by email.

## General course policies
**Feedback**: We welcome student feedback regarding the course at any point.  Please feel free to email us directly, or leave anonymous feedback for the instructional team by placing an anonymous note in Dr. Poldrack’s mailbox at Jordan Hall.  

**Gender expression/identity:**
This course affirms people of all gender expressions and gender identities. If you prefer to be called a different name than what is indicated on the class roster, please let me know. Feel free to correct me on your preferred gender pronoun. If you have any questions or concerns, please do not hesitate to contact me.

**Code of conduct:**
You are expected to treat the instructional team and your fellow students with courtesy and respect.  
This class should be a harassment-free learning experience for everyone regardless of gender, gender identity and expression, sexual orientation, disability, physical appearance, body size, race, age or religion. Harassment of any form will not be tolerated.
If someone makes you or anyone else feel unsafe or unwelcome, please report it as soon as possible to one of the instructors. If you are not comfortable approaching the instructional team, you may also contact the [Stanford Office of the Ombuds](https://ombuds.stanford.edu/)

**Students with Documented Disabilities:**
Students who may need an academic accommodation based on the impact of a disability must initiate the request with the Office of Accessible Education (OAE).  Professional staff will evaluate the request with required documentation, recommend reasonable accommodations, and prepare an Accommodation Letter for faculty dated in the current quarter in which the request is being made. Students should contact the OAE as soon as possible since timely notice is needed to coordinate accommodations.  The OAE is located at 563 Salvatierra Walk (phone: 723-1066, URL: http://studentaffairs.stanford.edu/oae).
## Class Schedule

| Date|Topic|Reading|
| ---|---|---|
| 9/25|Introduction: The concept and biology of brain connectivity<br><br>Learning Objectives:<br><br>After this lecture, you should be able to:<br>* Describe the different ways in which the concept of "brain connectivity" can be defined<br>* Describe the structural and functional basis of brain connectivity<br><br>|- [Brain connectivity](http://www.scholarpedia.org/article/Brain_connectivity)<br>- [From Cajal to Connectome and Beyond](https://www.annualreviews.org/doi/abs/10.1146/annurev-neuro-071714-033954)|
| 9/27|Hands on: Visualizing white matter structure with [FSLeyes](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/FSLeyes) and [nilearn](https://nilearn.github.io/index.html)<br><br>Learning Objectives:<br><br>After this lecture, you should be able to:<br>* Identify major white matter tracts in probabilistic atlases<br>* Load and visualize tract atlases in both FSLeyes and Python<br><br>||
| 10/2|Graph theory<br><br>Learning Objectives:<br><br>After this lecture, you should be able to:<br>* Describe the basic concepts of graph theory<br><br>|- [Network Science](https://pdfs.semanticscholar.org/54c8/9331fe520d77c2cb2581dd4c63af461d07e9.pdf)|
| 10/4|Hands on: Graph theory<br><br>Learning Objectives:<br><br>After this lecture, you should be able to:<br>* Use NetworkX to create and analyze graph data<br><br>||
| 10/9|Network modeling<br><br>Learning Objectives:<br><br>After this lecture, you should be able to:<br>* Describe the concepts of integration and segregation<br>* Describe the concept of modularity<br>* Describe the concept of community detection and the different approaches<br><br>|- [Brain graphs: graphical models of the human brain connectome](https://www.ncbi.nlm.nih.gov/pubmed/21128784)<br>- [Complex network measures of brain connectivity: uses and interpretations](https://www.ncbi.nlm.nih.gov/pubmed/19819337)<br>|
| 10/11|Hands on: Network modeling<br>||
| 10/16|Micro/nanoscale connectomics<br>|- [Micro-connectomics: probing the organization of neuronal networks at the cellular scale](https://www.nature.com/articles/nrn.2016.182)<br>- [Saturated Reconstruction of a Volume of Neocortex](https://www.sciencedirect.com/science/article/pii/S0092867415008247?via%3Dihub)|
| 10/18|Stand-up for paper proposals - each student presents a short overview of their project idea for discussion and feedback<br>||
| 10/23|Tract tracing<br>|- [A mesoscale connectome of the mouse brain](https://www.ncbi.nlm.nih.gov/pmc/articles/pmid/24695228/)<br>- [Classic and Contemporary Neural Tract-Tracing Techniques](https://www.sciencedirect.com/science/article/pii/B9780123964601000172)|
| 10/25|Hands on: Tract-tracing data<br>|- [A Weighted and Directed Interareal Connectivity Matrix for Macaque Cerebral Cortex](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3862262/)|
| 10/30|Diffusion MRI<br>|- [Using diffusion imaging to study human connectional anatomy](https://www.ncbi.nlm.nih.gov/pubmed/19400718)<br>- [Limits to anatomical accuracy of diffusion tractography using modern approaches](https://www.biorxiv.org/content/biorxiv/early/2018/08/16/392571.full.pdf)<br>|
| 11/1|Hands on: Diffusion MRI analysis with [dipy](http://nipy.org/dipy/) (Chris Gorgolewski, Guest lecturer)<br>|TBD|
| 11/6|Resting fMRI<br>|TBD|
| 11/8|Hands on: Resting fMRI analysis<br>||
| 11/13|Task fMRI<br>|- [Six problems for causal inference from fMRI](https://www.ncbi.nlm.nih.gov/pubmed/19747552)<br>- [Tools of the trade: psychophysiological interactions and functional connectivity](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3375893/)|
| 11/15|Hands on: Network modeling with fMRI data<br>|- [Network modelling methods for fMRI](http://mri-q.com/uploads/3/4/5/7/34572113/smith-fmri-2011.pdf)|
| 11/27|Large-scale brain networks<br>|- [The organization of the human cerebral cortex estimated by intrinsic functional connectivity](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3174820/)<br>- TBD|
| 11/29|Hands on: Parcellation and large-scale networks<br>||
| 12/4|Dynamics of brain networks<br>|TBD|
| 12/6|Hands on: Simulating dynamics using the Virtual Brain<br>|TBD|
| 12/10|Final meeting with project presentations, 12:15-3:15 pm <br>||
