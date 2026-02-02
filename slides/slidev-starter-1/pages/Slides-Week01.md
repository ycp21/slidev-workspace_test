---
title: SPCE 301 Week 01
theme: seriph
revealOptions:
  transition: 'fade'

---

# Welcome to SPCE301!

Yvette Perrott, Betina Pavri and Uli Zuelicke

---

## Plan for the course

<v-clicks>

- Bring together all the elements learned so far in SPCE101 and 201 (plus some more)
- Design your own mission!
- We will start by coming up with mission concepts in small groups (~3 people)
- At the end of Week 3 you will present your concepts to the class
- We will downselect to a single mission concept for developing further

</v-clicks>

---

## Assessments

<v-clicks>

* 10 lab sessions (30%) 
  * Marking will be a bit more strict than previously, some component expected to be completed outside of class 
* Peer feedback (5%) 
* Project management log (5%)
* Initial design document and presentation (10%) 
* Mid-design document (20%) 
* Final design document and presentation (30%) 

</v-clicks>

---

## Use of AI

* Okay to use AI to aid learning
  * Need clear statements on how AI was used for learning
  * Submit your AI prompts 
* All writing has to be own work. No AI allowed.
  * If AI is used to help improve language, submit the original and the final output. 

---

## Nuku

[Make sure you look through Nuku](https://nuku.wgtn.ac.nz/courses/33216)/

---
layout: iframe-right
url: https://pressbooks-dev.oer.hawaii.edu/epet302/
class: my-cool-content-on-the-left
---

## Recommended reading

---

## SPCE301 Week 01:
# Mission design overview

---

## Module Learning Objectives

<v-clicks>

- Elements of space missions that must be considered to build a successful mission
- Science or engineering questions as primary drivers of mission concepts and requirements
- Funding of space missions

</v-clicks>

---

### Mission components/mission architecture

<figure>
<img src="/Images/mission_components.png" width="80%"/>
<figcaption>Adapted from <a href="https://pressbooks-dev.oer.hawaii.edu/epet302/chapter/3-3-mission-components/">Zhu, Chap 3.3</a>.</figcaption>
</figure>

---

### Mission components - subject

1.  The *subject* of the mission is the thing that is sensed by or interacts with the space payload.  <br><br>

<v-clicks>

- This can be a *passive subject* (eg the fire in the FireSat example we considered previously) or an *active subject* (eg GPS receivers, direct broadcast television dishes).
- In the case of the passive subject, the mission designers don't control the subject itself but do control how the mission interacts with or senses it
- In the case of the active subject, the mission designers can directly control its design and basic parameters.

</v-clicks>

---

### Mission components - payload

2. The *payload* consists of the hardware and software that sense or interact with the subject.<br><br>

<v-clicks>

- If the subject is the "what", the payload is the "how".  
- As shown in the diagram, the subject defines the payload requirements.  
- We will investigate the relationship between the subject and payload further in this week's lab activity.

</v-clicks>

---

### Mission components - spacecraft bus

3. The *spacecraft bus* consists of a set of subsystems that support the payload by providing orbit and attitude maintenance, power, data handling, etc.<br><br>

<v-clicks>

- The payload and spacecraft bus together are called the *spacecraft, space segment* or *launch vehicle payload*.  
- As indicated by the thick arrow in the diagram above, the payload requirements are the main driver for the design of the spacecraft bus.

</v-clicks>

---

### Mission components - launch system

4. The *launch system* includes the launch facility, launch vehicle and any upper stage required to place the spacecraft in orbit, as well as interfaces, payload fairing and associated ground support equipment and facilities.<br><br>

<v-clicks>

- The launch system which will be used also generally drives the payload design, unless the whole launch system is being designed from scratch to accommodate a specific payload (which would be unusual).

</v-clicks>

---

### Mission components - orbit

5. The *orbit* is the spacecraft's path or trajectory in space.<br><br>

<v-clicks>

- Typically, there is a separate initial parking orbit, transfer orbit and final mission orbit.  There may also be an end-of-life/disposal orbit.  
- The orbit determines the space environment that the payload will experience, which also drives some aspects of its design.

</v-clicks>

---

### Mission components - C3

6. The *command, control and communications (C3) architecture* is the arrangement of components that satisfy the mission's C3 requirements.<br><br>

<v-clicks>

- This depends on the amount of data and timing requirements for the data to be transferred, as well as the number, location, availability and communicating ability of the space and ground assets.
- Crucial decision: how much autonomy to design into the system? Autonomy is expensive and difficult to test comprehensively, but may be necessary.

</v-clicks>

---

### Mission components - ground system

7. The *ground system* consists of the facilities and communications equipment associated with both fixed and mobile ground stations around the world, connected by data links.<br><br>

<v-clicks>

- The choice of communication frequency is a critical part of this architecture.

</v-clicks>

---

### Mission components - mission operations

8. *Mission operations* consist of the people, computers and software that execute the mission operations and assess the data returned.<br><br>

<v-clicks>

- They can be a separate team in the case of a big project, or the team that designs the mission can also be the mission operations team in smaller projects.

</v-clicks>

---

### Space Mission Engineering process

How do we go about designing all these different mission components?  We start by thinking about the *mission objective*.  There are two general categories we can think about here:

1) *Needs-based missions*: we want to fulfil a specific set of mission objectives.  For example, monitoring concentrations of CO$_2$ in the atmosphere, landing humans on the Moon, or observing astronomical objects in the infrared.

2) *Capability-based missions*: we have developed a new capability and we want to see what we can do with it.  An example of this might be the electric propulsion technology being developed at RRI.

---

### Mission novelty

Note that missions are funded because they’re doing something fundamentally new, whether that's science, engineering, or capability development.  Proposers should know: 

- What has been done before?  
- What is the current state of the art and how will the proposed mission advance that?

---

### Needs-based mission categories

<figure>
<img src="/Images/mission_engineering_process2.png" width="80%"/>
<figcaption>The wide range of space mission applications.  Adapted from Fig 1-15, New SMAD.</figcaption>
</figure>

---

### Space mission design process

<figure>
<img src="/Images/mission_engineering_process.png" width="80%"/>
<figcaption>Adapted from Table 3-1, New SMAD.</figcaption>
</figure>

---

### Space mission design process

- We will obviously not have time to go through all these steps in this course
- We will go through steps 1 to 4, (partially) define one mission architecture (step 5) and then skip straight to steps 13 and 14
- Our mission will not actually fly :(

---

### Step 1: mission objectives

- What are we trying to do with our mission?  Why?

---

### Eg: FireSat

<ul>
    <li>Primary objective:</li>
        <ul>
            <li>to detect, identify, monitor and report forest fires throughout the USA, including Alaska and Hawaii, in near real time and low cost.</li>
        </ul>
    <li>Secondary objectives:
        <ul>
            <li>to demonstrate to the public that positive action is underway to contain forest fires.</li>
            <li>to collect statistical data on the outbreak and growth of forest fires.</li>
            <li>to monitor forest fires for other countries.</li>
            <li>to collect other forest management data.</li>
        </ul>
    </li>
</ul>

---

### Step 1: mission objectives

- These objectives are very broad and high-level.  
- The rest of the design process determines exactly how and with what level of accuracy they will be achieved, and the technical requirements to achieve them. 
- But the aim of the overall mission is to meet these fundamental requirements.

---

### Needs-based missions

<figure>
<img src="/Images/mission_engineering_process2.png" width="80%"/>
<figcaption>The wide range of space mission applications.  Adapted from Fig 1-15, New SMAD.</figcaption>
</figure>

---

### Step 5: mission components

- Skipping forward a bit: what kind of technology do we need to achieve our high-level objective?

---

### Eg: FireSat

- Our high-level objective has defined our subject: fires, which are a passive subject to be sensed.  
- How could we sense them?  
- Fires give out heat and light, so we could use thermal or optical sensors to detect them
- They also produce chemicals and particles in the atmosphere that we might be able to detect as well.

---

### Needs-based missions

<figure>
<img src="/Images/mission_engineering_process2.png" width="80%"/>
<figcaption>The wide range of space mission applications.  Adapted from Fig 1-15, New SMAD.</figcaption>
</figure>

---

### Why do we need space?

- Going to space is expensive so it's important to consider whether we really need to do it!
- Some reasons include:
   - Global perspective
   - Above the atmosphere
   - Gravity-free environment
   - Abundant resources
   - Exploration of space itself

---

### Science Traceability Matrix

- A tool that has been developed to help address these questions and break them down in a systematic way is the "[Science Traceability Matrix](https://psyche.asu.edu/science-traceability-matrix/)" (STM).  
- We will use these to help develop your initial mission proposals.

---

Here is a description of the different parts of the STM:

<figure>
<img src="/Images/Science-Traceability-Matrix-Example_1.png" width="100%"/>
<figcaption>From <a href="https://psyche.asu.edu/science-traceability-matrix/">NASA's Psyche mission</a>.</figcaption>
</figure>

---

Here is a description of the different parts of the STM:

<figure>
<img src="/Images/Science-Traceability-Matrix-Example_2.png" width="100%"/>
<figcaption>From <a href="https://psyche.asu.edu/science-traceability-matrix/">NASA's Psyche mission</a>.</figcaption>
</figure>

---

And an example of an STM for the Psyche mission:

<figure>
<img src="/Images/Science-Traceability-Matrix-Example-Table-1.png" width="70%"/>
<figcaption>From <a href="https://psyche.asu.edu/science-traceability-matrix/">NASA's Psyche mission</a>.</figcaption>
</figure>

---
layout: iframe
url: http://www.csc.caltech.edu/references/2005%20Weiss%20et%20al%20IEEE%20STM.pdf
---

Another example:


---

## Starting point for your mission design

- What is the objective of your mission?
- Why is it important to do this?
- What similar things have been done before and why is your mission different/better?
- What kind of measurements do you need to make?
- What kind of technology could you use to achieve it?
- Why do you need to go to space to do it?

---

## Lab activity

Research at least two real space missions in detail.  They can be past, active or proposed.  Answer the "starting point" questions for these missions, fill out an STM and add any other details you think are important.  Some suggestions are:

- <a href="https://emit.jpl.nasa.gov/">EMIT</a>
- <a href="https://nisar.jpl.nasa.gov/">NISAR</a>
- <a href="https://misr.jpl.nasa.gov/">MISR</a>
- <a href="https://grace.jpl.nasa.gov/">GRACE</a>

---

## Funding space missions

- So you have your great idea for a mission, but how do you get it funded so you can build it?  
- Most of us are not billionaires who can fund things out of our own pockets, and so it's important to know about the funding "landscape" both here in NZ and internationally.

---

### Governmental funding

- In most countries, funding is available in some way through the government
- These funds are generally available through submitting a proposal to a call 
- Proposals are typically assessed by a panel, and the best ones selected to receive funding.  
- You will be competing for a limited amount of funding so your proposal has to be convincing!

---

### NZ-based funding

- Government funding in NZ is mostly available through the Ministry of Business, Innovation and Employment.
- For example, Paihau - Robinson Research Institute has received funding from the [Catalyst Fund](https://www.mbie.govt.nz/science-and-technology/science-and-innovation/funding-information-and-opportunities/investment-funds/catalyst-fund) (as part of a strategic partnership with the German Aerospace Centre, DLR) for some of their work.  
- Other relevant funds include the Endeavour fund (Smart Ideas and Research Programmes).

---

### NZ-based funding

- Also available through the [Royal Society Te Apārangi](https://www.royalsociety.org.nz/what-we-do/funds-and-opportunities/) are various research fellowships and/or funds such as the Marsden Fund 
- These could be used to fund the initial development of ideas leading to a mission, as the seed leading to a larger application to actually build and launch the mission.

---

### Science prioritization

- In the US, the National Academies of Science, Engineering and Medicine produce several "[decadal surveys](https://science.nasa.gov/about-us/science-strategy/decadal-surveys/)" which map out strategic priorities and mission directives across the next decade.  
- Those relevant to space are in Astrophysics, Planetary Science, Earth Science, Heliophysics and Biological and Physical Sciences.  
- The decadal surveys are carried out by a panel of subject experts, and researchers in the community have the opportunity to submit ideas and white papers.  
- They identify key questions and make recommendations about which missions are the most important to fund over the next decade.  

---

### "Origins, Worlds, and Life: A Decadal Strategy for Planetary Science and Astrobiology 2023-2032"

[Interactive viewer](https://nap.nationalacademies.org/resource/26522/interactive/)

---

### Science prioritization

- The very high-level "Science Goal" in an STM often connects with priorities identified in a decadal review.
- NASA releases calls for proposals, to which you can apply for funding for projects in various different categories.  
- For example the annual "Research Opportunities in Space and Earth Sciences" funds US-based researchers for projects in various subject areas linked to the decadal surveys.
- There are also "[Announcements of Opportunities](https://soma.larc.nasa.gov/)" (larger projects).  
- Non-US-based researchers can be involved in the proposals but cannot receive funding.

---

### Science prioritization

- The European Space Agency has a similar series of science programmes, the most recent of which is [Voyage 2050](https://www.esa.int/Science_Exploration/Space_Science/Voyage_2050_sets_sail_ESA_chooses_future_science_mission_themes).
- NZ is an [associated country of Pillar 2 of the Horizon Europe research funding system](https://www.mbie.govt.nz/science-and-technology/science-and-innovation/international-opportunities/horizon-europe-research-fund), which means that NZ-based researchers can join or lead Horizon Europe funding.  
- Of particular interest is Cluster 4 (Digital, Industry and Space).  
- They also issue calls for proposals in various areas related to the research priorities.  You can see some of the projects funded in 2024 [here](https://defence-industry-space.ec.europa.eu/results-horizon-europe-space-related-calls-work-programme-2023-2024-implemented-hadea-and-euspa_en).

---

### Science prioritization

- While not quite at the same level, in NZ we do have a [Space and Advanced Aviation Strategy for 2024 to 2030](https://www.mbie.govt.nz/science-and-technology/space/new-zealand-space-and-advanced-aviation-strategy)
- This sets out ambitions and priorities for the space sector in this country.  
- Aligning to this strategy will likely be helpful for funding applications going forward.

---

### Commercial funding

- If you have an idea which could be commercializable, another route is seeking backing from private investors.  
- This doesn't have to be mutually exclusive with governmental funding - for example, Dawn Aerospace initially [received funding from the Catalyst fund](https://www.dawnaerospace.com/latest-news/nzsa-backs-dawn), which helped them develop their technology to the point of being attractive to [commercial funders](https://www.dawnaerospace.com/latest-news/dawn-aerospace-secures-funding-from-nzs-largest-venture-capital-firm-movac).
- For more on Dawn Aerospace and their startup journey, listen to [this WFLS podcast](https://www.youtube.com/watch?v=ry_LIUKrx7U) (from about 45:30, but the whole podcast is really interesting).

---

### Military funding

- Space and the military have always been entangled, and this could be another important source of funding if your idea has a military application.  
- For example, the US Space Force has requested a [$USD29.4 billion budget](https://www.defense.gov/News/News-Stories/Article/Article/3705820/space-force-chief-says-shift-to-warfighting-posture-continues-despite-slight-bu/) for the 2025 financial year.  
- Accessing that funding might be more complicated and subject to citizenship requirements.  
- In NZ, border and bio-security concerns could lead to funding availability as well, for example monitoring territorial waters for illegal fishing.

---

### Philanthropic funding

- One final potential funding source is philanthropic - from investors that just like your idea and want to see it work.  
- For example, the [Breakthrough Initiatives](https://breakthroughinitiatives.org/about) are funded by a foundation established by Julia and Yuri Milner.

---

### Class discussion

- How do you think funding priorities should be set, and how should funding be allocated?  
- What issues do you see with the current system, and what would you propose to change things?

