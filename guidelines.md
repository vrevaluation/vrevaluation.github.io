---
layout: page
title: Guidelines
navigation: 2
nav_order: 2
---

# VR object selection and manipulation study guidelines
{: .no_toc }


[Contribute via Google Docs](https://docs.google.com/document/d/1xhJFWsNdzVru21kheWnoRRrgtQAc7fqz9dYHf5kFbdU/edit?usp=sharing){:target="_blank"}

[Download pdf-version](https://github.com/vrevaluation/vrevaluation.github.io/releases/latest){:target="_blank"}

---

Version 1.0.0

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

### Define the goal of the evaluation

We recommend deciding early on whether the goal of the study is to evaluate speed or accuracy in object selection or manipulation. The main dependent variable should clearly follow from this. The purpose of this recommendation is to either eliminate errors from analysing speed (as in the Fitts’ paradigms), or to focus on analysing accuracy. The pitfalls of combining speed and accuracy in the study design include, for instance, to restrict completion time and judge errors from exceeded time when the goal is to measure accuracy. If the goal is to investigate speed (i.e., task completion time) in selection tasks, we recommend using the size difference between the cursor and the target object as the error threshold. It should also be required that the first is completely inside the second for successful task completion. If the cursor is a single-pixel cursor, the target size gives the error threshold (as the width does in ISO task). If the task is a manipulation task, we recommend using thresholds for object placement (e.g., the thresholds for aligning cubes can be expressed as *x* mm and *y* degrees, as in Yang et al. [[88]](#88)). That way, the speed can be analysed from (successful) completion times either after a selection or after the threshold of manipulation is met. If the goal is to measure accuracy, we recommend a free range for possible end-positions, confirmed with some selection trigger. Here, all selections are accepted, and the distance (whether of a single-pixel cursor from a single-pixel crosshair target [[50]](#50), or the angular difference along the three axes of rotation from the target object’s rotation [[48]](#48)) is measured and analysed as a continuous accuracy variable. Finally, while speed and accuracy should not be combined in the goals, we recommend doing so in analysis when it is possible and useful for insights. This can be done by analysing throughput with effective IDs [[71]](#71); note, however, the concerns that for instance Stuerlinger and Teather [[74]](#74) presented for doing this with non-spherical hit distributions in 3D.

### Estimate the required number of participants with power analysis

The average number of participants per study in our sample was 18. 8, whereas in general in HCI, it is 20–30 [5,15]. We should strive to reach at least that range. We also recommend reporting effect sizes with statistical tests as this helps others to conduct a priori power analyses to better estimate the required sample size. If estimation is not possible, we recommend using a minimum of 20 participants. We also recommend the inclusion of expert participants, as VR has strong novelty effects, especially on subjective measures. Including expert participants can reduce this bias and move towards assessments of VR as a mainstream technology. To measure expertise, we recommend using objective scales, such as options with how often related technology is used (e.g., daily, or N times a week as in Sidenmark and Gellersen [[69]](#69)) rather than reflective ones without a baseline (e.g., "rate your expertise from 1 to 5" [[72]](#72)).

### Strive for high control with a simple study design
{:toc}

We recommend using a maximum of three independent variables or factors. Nearly all studies (92. 7%) used a within-subject design, which we also recommend using to decrease the influence of interpersonal variability on the performance in these low-level tasks. However, counter balancing the order of study conditions in a within-subject design becomes tricky when there are many conditions (again, a simple design helps) but it’s widely accepted that counterbalancing is usually necessary to decrease learning effects. Clearly define the independent variables and their levels in the study. When there is more than one independent variable or group, we recommend reporting them and their levels in the N&times;M&times;P format. It is essential to include all the factors varied. We noticed that when following this style only partially (e.g., "for each interaction technique, there were 24 conditions (2&times;2&times;3&times;2)" [[85]](#85), there are actually two techniques, giving 48 conditions in total), the study designs are hard to follow, and the analysis methods remain unclear. However, if a study design results in many conditions, two approaches may help simplify the design. First, consider combining target distances and sizes into different IDs: you can include targets at different depths, for instance, by increasing the target size or decreasing the distance so that it matches the IDs (see an example in Tu et al. [[78]](#78)). Second, consider decreasing device&times;technique combinations by fixing either as a constant. For example, control the device type as an independent variable when your study is about a technique and vice versa.

### Use low-level tasks in evaluations

When the goal of a study is to compare interaction techniques, we recommend using low-level tasks: pointing and selection, or translation and rotation. Such tasks help to generalise the benefits of interaction techniques to any higher-level tasks: the performance in those is always dependent on the lower-level components (as LaViola et al. also suggest [[38]](#38)). Additionally, using lower-level tasks helps isolate and gain insights into the tested techniques’ particular strengths and weaknesses. For selection techniques, the lower-level tasks are pointing and selection. We recommend separating these in the study design. To do this, the study design can fix the alternate low-level task as a constant. For example selection can be made via a button press when studying pointing techniques, or by using a single pointing technique (e.g., ray-casting as in [[6]](#6)) when studying the effects of a selection method on accuracy. If these low-level tasks are combined, we recommend designing dependent measures such that the performance in the two sub-tasks can be separated. Treating both as independent variables is often unnecessary and results in a complex study design (recommendation (1)). For manipulation tasks, we recommend including at least translation and rotation tasks. We recommend performing the tasks including translation with a target object collocated in space. This target object can be a docking point (e.g., Lee et al. [[39]](#39)), or a transparent version of the object in which it needs to be co-located(e.g., Yang et al. [[88]](#88)). If the task includes rotation, the methods used for translation apply, with suitable thresholds for accurate placement or successful co-location. Alternatively, rotation-only tasks can use a dislocated duplicate model object as a target (e.g., a house [[79]](#79)). This is particularly useful when accuracy instead of error is measured(not to convey assumptions of successful orientation with visual co-location). In general, we recommend the first approach with co-located targets, to prevent other factors such as size or depth perception influencing performance in the translation or rotation task.

### Control the target distance in trials

Object selection and manipulation tasks can be discrete or serial. Discrete tasks have a particular starting position for the task. In contrast, a serial task consists of a sequence of targets with the starting position for the next target being the previous target (see, e.g., the two schemes for implementing the Fitts paradigm in Soukoreff and MacKenzie [[71]](#71)). We recommend using discrete tasks, as they are simpler to implement. For example, the task can always be started at the same point in space and in relation to the target arrangement. Therefore, it is also easy to systematically count for variation in the resulting distances of targets, movement directions toward them, etc. A serial task is more complex to implement if a circular layout (as in the ISO tapping task) is not used. This is because systematic target distance and size variation, as well as possible distractor targets on the optimal motion path, need to be carefully designed and controlled. Most studies that did not use the ISO task used a discrete task. Those that did use a serial task outside of ISO, randomised the target layout instead of using a systematic control of distance—and then failed to report the target distances resulting from randomisation. The recommendation of a discrete task and starting position holds for selection and translation and for rotation (that is, always starting from the same object orientation).

### Control the target size

We recommend using spherical targets to enable clear size control using the sphere’s diameter (such as for width in Fitts’ law studies). This means there is no need to orient targets in the selection task according to the movement direction. We also recommend using either a single-pixel pointer or a fixed-sized cursor across all tasks in a selection study. If a cursor is used, it’s size should be reported to allow correct calculation of errors (the method for determining errors should also be reported). We recommend defining errors as selections when the pointer is not completely inside the target object. With manipulation tasks, we recommend using color-coded cuboids or other polyhedrons that express the orientation unambiguously (e.g., tetrahedrons as in Wang and Lindeman [[81]](#81)). We also recommend using the same object shape both in the manipulated and target object (e.g., both cubes instead of placing a sphere in a cube [[43]](#43)). This helps to determine the required accuracy for a successful performance (e.g., if a successful translation or rotation is determined by docking an object of size *d* inside an object sized 1.5*d* [[47]](#47)).

### Aim for a wide and representative range of target sizes and distances

Soukoreff and McKenzie recommend using a wide and representative range of ID values for pointing device evaluation [[71]](#71). They suggested using ID values ranging from 2 to 8 bits. We recommend taking that as a guideline, but extending the general recommendation of a wide and representative range to target sizes and distances in general, and in both object selection and manipulation. We recommend using at least 6 levels of IDs (or at least 3 distances and 3 sizes). The studies with ISO tasks in our survey that used 6 to 9 levels of IDs, most commonly using three sizes and three distances. However, as mentioned above, the studies using ISO tapping tasks did not arrange targets across all three dimensions. None of the studies with "true" 3D target arrangement in the sample included 3&times;3 levels in their design. They either did not report distances (and had random targets), or varied those only at a maximum of three levels but did not vary the size. Therefore we maintain our recommendation at a modest minimum of three levels but with an ambition to include that for both distance and size variables. We recommend using euclidian distances for selection and translation tasks, and degrees for rotation tasks. We also recommend reporting these in SI units (such as meters) and angles in degrees or radians, and in both where possible (e.g., sizes and distances also as angular degrees of the visual field, such as in Tu et al. [[78]](#78)).

### Include a range of movement directions

We recommend placing targets across all three dimensions. The value of a selection or manipulation technique is hard to generalise from fixed, two-dimensional planes, because immersive virtual environments inherently are three-dimensional spaces, and therefore the objects of interest are likely located across the three dimensions. The performance in object selection and manipulation also varies across different directional motions: depth control is more difficult than lateral axis control (such as on a vertical plane). For example, performance in tapping two targets at different depths in front of the user is worse than tapping two targets with the same width and at the same distance on the sides [[44]](#44). Therefore, it is important for experimental comprehensiveness to include targets across all the three dimensions. The designs in our sample of studies also assimilate with the importance of this: over half (58.8%) of the studies that did not restrict themselves into the standard 2D ISO tapping task or involved typing on keyboards laid out targets across three dimensions.

### Control the physical setting in the study

We recommend using a fixed standing or sitting position in the physical space. Combining walking with object selection or manipulation adds a completely distinct task to the study. For example, LaViola et al. [[38]](#38) and many papers about interaction techniques for VR (e.g., [9–11,30,52])treat walking as a separate task.

### Control the virtual setting in the study

We recommend using a generic virtual environment, but with depth cues from shadows and from the surroundings, such as the ground or the walls. Depth cues are important, but realistic settings are difficult to compare with all possible distractors. Consider if your task is too specialised, if you feel a need to design a complex environment.

## References
{: .no_toc }

<a id="5">[[5]](#5)</a> Louise Barkhuus and Jennifer A Rode. 2007. From mice to men-24 years of evaluation in CHI. In *Proceedings of the SIGCHI Conference on Human Factors in Computing Systems*, Vol. 10. [https://doi.org/10.1145/1240624.2180963](https://doi.org/10.1145/1240624.2180963){:target="_blank"}

<a id="6">[[6]](#6)</a> Anil Ufuk Batmaz and Wolfgang Stuerzlinger. 2019. Effects of 3d rotational jitter and selection methods on 3d pointing tasks. *26th IEEE Conference on Virtual Reality and 3D User Interfaces, VR 2019 - Proceedings (2019)*, 1687–1692. [https://doi.org/10.1109/VR.2019.8798038](https://doi.org/10.1109/VR.2019.8798038){:target="_blank"}

<a id="9">[[9]](#9)</a> Doug Bowman, Ernst Kruijff, Joseph J LaViola Jr, and Ivan P Poupyrev. 2004. *3D user interfaces: Theory and Practice* (1 ed.). Addison-Wesley Professional.

<a id="10">[[10]](#10)</a> Doug A Bowman, Donald B Johnson, and Larry F Hodges. 2001. Testbed evaluation of virtual environment interaction techniques. *Presence: Teleoperators & Virtual Environments 10*, 1 (2001), 75–95.

<a id="11">[[11]](#11)</a> Doug A Bowman, Ernst Kruijff, Joseph J LaViola Jr, and Ivan Poupyrev. 2001. An introduction to 3-D user interface design. *Presence: Teleoperators & Virtual Environments 10*, 1 (2001), 96–108. 

<a id="15">[[15]](#15)</a> Kelly Caine. 2016. Local Standards for Sample Size at CHI. In *Proceedings of the 2016 CHI Conference on Human Factors in Computing Systems* (San Jose, California, USA) (CHI ’16). Association for Computing Machinery, New York, NY, USA, 981–992. [https://doi.org/10.1145/2858036.2858498](https://doi.org/10.1145/2858036.2858498){:target="_blank"}

<a id="30">[[30]](#30)</a> Chris Hand. 1997. A survey of 3D interaction techniques. In *Computer graphics forum*, Vol. 16. Wiley Online Library, 269–281. [https://doi.org/10.1111/1467-8659.00194](https://doi.org/10.1111/1467-8659.00194){:target="_blank"}

<a id="38">[[38]](#38)</a> Joseph J LaViola Jr, Ernst Kruijff, Ryan P McMahan, Doug Bowman, and Ivan Poupyrev. 2017. *3D user interfaces: theory and practice* (2 ed.). Addison-Wesley Professional.

<a id="39">[[39]](#39)</a> Jaeyeon Lee, Mike Sinclair, Mar Gonzalez-Franco, Eyal Ofek, and Christian Holz. 2019. TORC: A virtual reality controller for in-hand high-dexterity finger interaction. *Conference on Human Factors in Computing Systems - Proceedings* (2019), 1–13. [https://doi.org/10.1145/3290605.3300301](https://doi.org/10.1145/3290605.3300301){:target="_blank"}

<a id="43">[[43]](#43)</a> R. W. Lindeman, J. L. Sibert, and J. N. Templeman. 2001. The effect of 3D widget representation and simulated surface constraints on interaction in virtual environments. Proceedings - Virtual Reality Annual International Symposium (2001), 141–148. [https://doi.org/10.1109/vr.2001.913780](https://doi.org/10.1109/vr.2001.913780){:target="_blank"}

<a id="44">[[44]](#44)</a> Mayra Donaji Barrera Machuca and Wolfgang Stuerzlinger. 2019. The effect of stereo display deficiencies on virtual hand pointing. In *Conference on Human Factors in Computing Systems - Proceedings*. Association for Computing Machinery. [https://doi.org/10.1145/3290605.3300437](https://doi.org/10.1145/3290605.3300437){:target="_blank"}

<a id="47">[[47]](#47)</a> Diako Mardanbegi, Benedikt Mayer, Ken Pfeuffer, Shahram Jalaliniya, Hans Gellersen, and Alexander Perzl. 2019. EyeSeeThrough: Unifying tool selection and application in virtual environments. *26th IEEE Conference on Virtual Reality and 3D User Interfaces, VR 2019 - Proceedings* (2019), 474–483. [https://doi.org/10.1109/VR.2019.8797988](https://doi.org/10.1109/VR.2019.8797988){:target="_blank"}

<a id="48">[[48]](#48)</a> Alejandro Martin-Gomez, Ulrich Eck, and Nassir Navab. 2019. Visualization techniques for precise alignment in VR: A comparative study. *26th IEEE Conference on Virtual Reality and 3D User Interfaces, VR 2019 - Proceedings* (2019), 735–741. [https://doi.org/10.1109/VR.2019.8798135](https://doi.org/10.1109/VR.2019.8798135){:target="_blank"}

<a id="50">[[50]](#50)</a> Sven Mayer, Valentin Schwind, Robin Schweigert, and Niels Henze. 2018. The effect of offset correction and cursor on mid-air Pointing in real and virtual environments. *Conference on Human Factors in Computing Systems - Proceedings 2018-April* (2018), 1–13. [https://doi.org/10.1145/3173574.3174227](https://doi.org/10.1145/3173574.3174227){:target="_blank"}

<a id="52">[[52]](#52)</a> Daniel Mendes, Fabio Marco Caputo, Andrea Giachetti, Alfredo Ferreira, and J Jorge. 2019. A survey on 3D virtual object manipulation: From the desktop to immersive virtual environments. In *Computer graphics forum*, Vol. 38. Wiley Online Library, 21–45. [https://doi.org/10.1111/cgf.13390](https://doi.org/10.1111/cgf.13390){:target="_blank"}

<a id="69">[[69]](#69)</a> Ludwig Sidenmark and Hans Gellersen. 2019. Eye & Head: Synergetic eye and head movement for gaze pointing and selection. *UIST 2019 - Proceedings of the 32nd Annual ACM Symposium on User Interface Software and Technology* (2019), 1161–1174. [https://doi.org/10.1145/3332165.3347921](https://doi.org/10.1145/3332165.3347921){:target="_blank"}

<a id="71">[[71]](#71)</a> R. William Soukoreff and I. Scott MacKenzie. 2004. Towards a standard for pointing device evaluation, perspectives on 27 years of Fitts’ law research in HCI. *International journal of human-computer studies* 61, 6 (2004), 751–789. [https://doi.org/10.1016/j.ijhcs.2004.09.001](https://doi.org/10.1016/j.ijhcs.2004.09.001){:target="_blank"}

<a id="72">[[72]](#72)</a> Marco Speicher, Anna Maria Feit, Pascal Ziegler, and Antonio Krüger. 2018. Selection-based text entry In Virtual Reality. In *Conference on Human Factors in Computing Systems - Proceedings*, Vol. 2018-April. [https://doi.org/10.1145/3173574.3174221](https://doi.org/10.1145/3173574.3174221){:target="_blank"}

<a id="74">[[74]](#74)</a> Rasmus Stenholt. 2012. Efficient selection of multiple objects on a large scale. *Proceedings of the ACM Symposium on Virtual Reality Software and Technology, VRST* (2012), 105–112. [https://doi.org/10.1145/2407336.2407357](https://doi.org/10.1145/2407336.2407357){:target="_blank"} 

<a id="78">[[78]](#78)</a> Tanh Quang Tran, Hyun Ju Shin, Wolfgang Stuerzlinger, and Jung Hyun Han. 2017. Effects of virtual arm representations on interaction in virtual environments. *Proceedings of the ACM Symposium on Virtual Reality Software and Technology, VRST* (2017). [https://doi.org/10.1145/3139131.3139149](https://doi.org/10.1145/3139131.3139149){:target="_blank"}

<a id="79">[[79]](#79)</a> Huawei Tu, Susu Huang, Jiabin Yuan, Xiangshi Ren, and Feng Tian. 2019. Crossing-based selection with virtual reality head-mounted displays. In *Conference on Human Factors in Computing Systems - Proceedings (CHI ’19)*. Association for Computing Machinery, New York, NY, USA. [https://doi.org/10.1145/3290605.3300848](https://doi.org/10.1145/3290605.3300848){:target="_blank"}

<a id="81">[[81]](#81)</a> Keith Vertanen and Per Ola Kristensson. 2011. A versatile dataset for text entry evaluations based on genuine mobile emails. In *Proceedings of the 13th International Conference on Human Computer Interaction with Mobile Devices and Services*.
295–298. [https://doi.org/10.1145/2037373.2037418](https://doi.org/10.1145/2037373.2037418){:target="_blank"}

<a id="85">[[85]](#85)</a> Steve Whittaker, Loren Terveen, and Bonnie A Nardi. 2000. Let’s stop pushing the envelope and start addressing it: a reference task agenda for HCI. *Human–Computer Interaction* 15, 2-3 (2000), 75–106. [https://doi.org/10.1207/S15327051HCI1523_2](https://doi.org/10.1207/S15327051HCI1523_2){:target="_blank"}

<a id="88">[[88]](#88)</a> Bob G. Witmer and Michael J. Singer. 1998. Measuring Presence in Virtual Environments: A Presence Questionnaire. *Presence: Teleoperators and Virtual Environments 7*, 3 (1998), 225–240. [https://doi.org/10.1162/105474698565686](https://doi.org/10.1162/105474698565686){:target="_blank"}
