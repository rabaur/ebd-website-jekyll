---
layout: exercise
title: Exercise 3
date:   2024-02-14 15:48:01 +0100
categories: jekyll update
publish: true
---

# Exercise 3: Comparing Users’ Wayfinding across Hospital Typologies

## Submission Details 
- **Group size**: Up to 4 students
- **Submission date**: 27.11.2024, 17:59 CET
- **Presentation date**: 27.11.2024
- **Submission materials**:
  - For all the following materials, use the naming convention of your group member's last name delimited by `_`. Example: If your group consists of _A. Einstein_, _M. Curie_ → `einstein_curie` with the appropriate file extension.
  - The `fbx` models of the **two** hospital typologies. [Upload link](https://polybox.ethz.ch/index.php/s/s8njKELCd8qdEMC)
  - A presentation on this exercise (max. 10 slides, max. 5 minutes, exceeding this will result in grade penalty). [Upload link](https://polybox.ethz.ch/index.php/s/xpkGTZnJRRnANe2)
  - The `zip` compressed Unity project folder. [Upload link](https://polybox.ethz.ch/index.php/s/Ak4kazIVtngM8Jc)

## Overview

This exercise is a continuation of exercise 2.
In exercise 2, you have performed an intervention to a floorplan and evaluated it with the help of analytics.
In this exercise, you will test how that intervention will affect human behavior in a 3D virtual walkthrough of the typologies.
As a general guide for the exercise, please refer to the tutorial given in lecture 8.

## 1 Choosing Your Groups and Typologies
- Form groups of 3 to 4 people using [this sheet](https://docs.google.com/spreadsheets/d/1zr8fpB73u7Xav52ACkJfbUrC0qmHQpRzlGYIsKvUeiU/edit?usp=sharing). Smaller groups will only be allowed by the course team in exceptional circumstances.
- Choose 1 layout (and its corresponding intervention) from your group that you will focus on.


## 2 Creating 3D Geometry from Line Drawings
- Take a screenshot of the base layout and the intervention layout in [arxitect](https://arxitect.ivia.ch/home).
- Retrace the line drawings in your favourite 3D software. Note that we will only be able to assist you if you use [Rhino 7](https://www.rhino3d.com/download/archive/rhino/7/latest/)
  - If you decide to use Rhino 7, we can provide you with a license. Please send an email to [bopanb@student.ethz.ch](bopanb@student.ethz.ch) with the email that is associated with your Rhino account such that we can invite you to the license pool.
- Follow the approach shown in [the lecture](https://ethz.zoom.us/rec/share/HYDx-BdTlpGVI22vkQlLpduRA_Pof-JPmg7bz_Fu4Au8xlzTCISdEmCG_Zvru1hY.uUD1DtbZ3ugkVtMZ) to properly scale your reference image, trace the lines, and create 3D walls from them.
- After this is done, follow the approach in the lecture to make sure that your walls are double-sided (adding thickness)
- Finally, export your geometry to fbx

## 3 Importing Your 3D Geometry into Unity
- Follow [the lecture](https://ethz.zoom.us/rec/share/HYDx-BdTlpGVI22vkQlLpduRA_Pof-JPmg7bz_Fu4Au8xlzTCISdEmCG_Zvru1hY.uUD1DtbZ3ugkVtMZ) and or [this tutorial](https://github.com/rabaur/EBD-Toolkit/tree/main) to obtain **GitHub Desktop**, **Unity 2022.3.XXX**, and the **Unity Project**.
- Familiarize with the functionalities of the tool through [the lecture](https://ethz.zoom.us/rec/share/HYDx-BdTlpGVI22vkQlLpduRA_Pof-JPmg7bz_Fu4Au8xlzTCISdEmCG_Zvru1hY.uUD1DtbZ3ugkVtMZ).
- Make sure that you are able to collect and visualize some data in the reference scene `VirtualWalkthrough`.
- For more in-depth information, follow [this tutorial](https://github.com/rabaur/EBD-Toolkit/blob/main/docs/virtual_walkthrough.md)
- Go through this checklist before continuing with your next steps:
  - Have I imported my two layouts (the fbx files generated in step 2) into a new scene each (not the reference scene)?
  - Is my geometry up to scale?
  - Have I pressed "Calculate colliders" and applied the changes when importing the geometry?
  - Have I made all items static by clicking the "static" checkbox?
  - Have I assigned all objects to the relevant layers or created new layers if needed?
  - Have I rebuilt and visualized the NavMesh?

## 4 Coming Up With an Experiment
- For this exercise, you will be recruiting at least 3 participants to perform the virtual walkthrough.
- These participants can be anyone except your group members themselves. They could also be colleagues from other EBD groups.
- Familiarize yourself with the outputs that the tool provides. What would be an interesting research question to ask in your layout? Consult [the lecture](https://ethz.zoom.us/rec/share/HYDx-BdTlpGVI22vkQlLpduRA_Pof-JPmg7bz_Fu4Au8xlzTCISdEmCG_Zvru1hY.uUD1DtbZ3ugkVtMZ) to check what the properties of a good research question are.
- Your will perform a [within-subject](https://www.scribbr.com/methodology/within-subjects-design/) study, meaning all your participants will see both layouts. Randomize the order of experiments to combat learning effects.
- Define a role and a task for your participant. Example:
  - Role: A new assistant doctor on the search for a patient.
  - Task: Start at the nurse station. The doctor needs to perform an undirected search, since it is their first working day.
- Come up with a hypothesis regarding some measure related to your task. Example:
  - Hypothesis: The doctors will on average take longer to find the patient room in layout 1 since the network efficiency is lower
- Think about how you can **measure** your outcome using the tool. Example:
  - We will use the path length and the walkthrough duration
- **Important**: Before beginning with the experiments, send an email to *raphael.baur@ai.ethz.ch* to submit your research question / hypothesis, your role, task, and how you will measure whether your hypothesis holds or not
- Go through this checklist before continuing with the experiments:
  - I have recruited at least 3 participants
  - I have received a feedback regarding my experimental design

## 5 Analyzing and Visualizing the Outcomes
- Use the various visualization tools of the toolkit to visualize "visual attention" patterns and trajectories (at least one, both only if applicable to your hypothesis)
- Perform a statistical test on your collected outcomes. Google Sheets supports simple (and complex) statistical tests like a [t-Test](https://support.google.com/docs/answer/6055837?hl=en)
- Feel free to use more involved statistical tests or methods if applicable
- Summarize your findings in a presentation (10 slides, 5 minutes max).