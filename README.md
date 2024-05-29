# Joplin, MO Community Resilience Analysis: A Case Study of Tornado Impact Using [IN-CORE](https://incore.ncsa.illinois.edu/)

```
Lee, J. S., Navarro, C., Wang, C., Kim, Y. W., Panchani, R., Yang, Y., Kooper, R., Mohanarajan, V., & Watkins, L., 
Wang, W. (2024). 
IN-CORE US-RSE’24 Submission: Joplin, MO Community Resilience Analysis: A Case Study of Tornado Impact Using IN-CORE (Version 1.0.0) 
[Computer software]. https://github.com/IN-CORE/incore-usrse24-submission
```

**Authors**:

- Jong S. Lee <jonglee1@illinois.edu>
- Chris Navarro <cmnavarr@illinois.edu>
- Chen Wang <cwang138@illinois.edu>
- Yong Wook Kim <ywkim@illinois.edu>
- Rashmil Panchani <rmp6@illinois.edu>
- Ya-Lan Yang <ylyang@illinois.edu>
- Rob Kooper <kooper@illinois.edu>
- Vismayak Mohanarajan <mohanar2@illinois.edu>
- Lisa Watkins <watkinsl@illinois.edu>
- Wanting (Lisa) Wang <Lisa.Wang@colostate.edu>

**Affiliation**: All the mentioned authors are working at
the [National Center for Supercomputing Applications](https://www.ncsa.illinois.edu/),
University of Illinois at Urbana-Champaign.

---

Note: This repository contains the submission materials for the US-RSE’24 conference from the IN-CORE framework. It
demonstrates the application of IN-CORE (Interdependent Networked Community Resilience Modeling Environment) for
assessing community resilience, focusing on the Joplin, Missouri Tornado damage case study.

### Abstract

Community resilience research is essential for anticipating, preventing, and mitigating the impacts of natural and
anthropogenic disasters. Among these, tornadoes occur at a high frequency in the United States compared to other
natural hazards such as earthquakes and tsunamis. Even a single high-intensity tornado can result in high casualty
rates and catastrophic economic losses and social consequences, particularly for small to medium communities. Hence,
studying the impact of tornadoes on community resilience is crucial. The city of Joplin, Missouri, USA, was hit by an
EF-5 tornado on May 22, 2011. For more details regarding this event, please refer to the technical investigation of
this devastating event in the [NIST Report](https://nvlpubs.nist.gov/nistpubs/NCSTAR/NIST.NCSTAR.3.pdf).

The [Center for Risk-Based Community Resilience Planning](http://resilience.colostate.edu/), funded by
the [National Institute of Standards and Technology (NIST)](https://www.nist.gov/), developed the measurement science
to support community resilience assessment. This measurement science is implemented on a platform called
the [Interdependent Networked Community Resilience Modeling Environment (IN-CORE)](https://incore.ncsa.illinois.edu/).
On IN-CORE, users can run scientific analyses that model the impact of natural hazards and community resilience against
these impacts. This Jupyter Notebook provides an example of how to use IN-CORE to simulate this event for buildings and
the electrical power network of Joplin.

The initial damage prediction utilized the tornado path, tornado fragility curves representative of a 19-archetype
building dataset, and electric power network datasets. Generic tornado paths are also available in IN-CORE, or a
user-defined tornado path can be used. The functionality of the infrastructure was linked with a computable general
equilibrium (CGE) economics model that computes specific community resilience metrics in economic terms. A population
dislocation model provides resilience metrics related to socio-demographics such as population dislocation as a
function of income or race/ethnicity. Lastly, the housing household recovery analysis computes the series of household
recovery states given a population dislocation, a transition probability matrix (TPM), and an initial state vector. The
history of housing recovery changes for each household unit will be predicted.

To further facilitate resilience planning, several building retrofit strategies were applied to simulate the potential
mitigation of future tornado impacts. Building retrofit involves enhancing the structural integrity of existing
buildings to withstand natural hazards. The retrofit plan is generated as an optimal solution given budget and other
constraints. The first step is computing the building damage considering no retrofit effort implemented on the building
inventory. Then, the selected retrofit plan is implemented on the building inventory, and the building damage is
computed again. Using results from the building damage with and without retrofit efforts, we can calculate population
dislocation or other resilience metrics to see if the potential impact is reduced by the retrofit plan.

Last but not least, the core logic of this notebook was also used to power
the [IN-CORE Community Resilience Playbook](https://incore.ncsa.illinois.edu/playbook/joplin/), an interactive guide
for community resilience planning. The Playbook provides practical steps and analytical tools to help communities
prepare for, respond to, and recover from disasters. IN-CORE is in partnership with the city of Joplin and conducted
four workshops with the city planners and government officials, making it a valuable resource for resilience planning.

