# Child Mind Institute - Detect Sleep States
'Detect sleep onset and wake from wrist-worn accelerometer data'

## Overview
Your work will improve researchers' ability to analyze accelerometer data for sleep monitoring and enable them to conduct large-scale studies of sleep. Ultimately, the work of this competition could improve awareness and guidance surrounding the importance of sleep. The valuable insights into how environmental factors impact sleep, mood, and behavior can inform the development of personalized interventions and support systems tailored to the unique needs of each child.
<p align="center">
<img src = 'https://github.com/SehyunPark/Competitions/assets/28240330/69d33cf2-9ac1-4c62-9d42-8dd097da4860' width="500" height="200" align="center">
</p>

## Description
### Goal of the Competition
The goal of this competition is to <b>detect sleep onset and wake</b>. You will develop a model trained on wrist-worn accelerometer data in order to determine a person's sleep state.

Your work could make it possible for researchers to conduct more reliable, larger-scale sleep studies across a range of populations and contexts. The results of such studies could provide even more information about sleep.

The successful outcome of this competition can also have significant implications for children and youth, especially those with mood and behavior difficulties. Sleep is crucial in regulating mood, emotions, and behavior in individuals of all ages, particularly children. By accurately detecting periods of sleep and wakefulness from wrist-worn accelerometer data, researchers can gain a deeper understanding of sleep patterns and better understand disturbances in children.

### Context
The “Zzzs” you catch each night are crucial for your overall health. Sleep affects everything from your development to cognitive functioning. Even so, research into sleep has proved challenging, due to the lack of naturalistic data capture alongside accurate annotation. If data science could help researchers better analyze wrist-worn accelerometer data for sleep monitoring, sleep experts could more easily conduct large-scale studies of sleep, thus improving the understanding of sleep's importance and function.

Current approaches for annotating sleep data include sleep logs, which are the gold standard for detecting the onset of sleep. However, they are impractical for many participants to use reliably, and fail to capture the nuanced difference between heading to bed and falling asleep (or, conversely, waking up and getting out of bed). Heuristic-based software is another solution that attempts to identify sleep windows, though these rely on human-engineered features of sleep (i.e. arm angle) that vary across individuals and don’t accurately summarize the sleep windows that experts can visually detect from their data. With improved tools to analyze sleep data on a large scale, researchers can explore the relationship between sleep and mood/behavioral difficulties. This knowledge can lead to more targeted interventions and treatment strategies.

Competition host Child Mind Institute (CMI) transforms the lives of children and families struggling with mental health and learning disorders by giving them the help they need. CMI has become the leading independent nonprofit in children’s mental health by providing gold-standard evidence-based care, delivering educational resources to millions of families each year, training educators in underserved communities, and developing tomorrow’s breakthrough treatments.

Established with a foundational grant from the Stavros Niarchos Foundation (SNF), the SNF Global Center for Child and Adolescent Mental Health at the Child Mind Institute works to accelerate global collaboration on under-researched areas of children’s mental health and expand worldwide access to culturally appropriate trainings, resources, and treatment. A major goal of the SNF Global Center is to expand innovations in clinical assessment and intervention, to include building, testing, and deploying new technologies to augment mental health care and research, including mobile apps, sensors, and analytical tools.

Your work will improve researchers' ability to analyze accelerometer data for sleep monitoring and enable them to conduct large-scale studies of sleep. Ultimately, the work of this competition could improve awareness and guidance surrounding the importance of sleep. The valuable insights into how environmental factors impact sleep, mood, and behavior can inform the development of personalized interventions and support systems tailored to the unique needs of each child.

### Acknowledgements
The data used for this competition was provided by the Healthy Brain Network, a landmark mental health study based in New York City that will help children around the world. In the Healthy Brain Network, families, community leaders, and supporters are partnering with the Child Mind Institute to unlock the secrets of the developing brain. In addition to generous support provided by the Kaggle team, financial support has been provided by the Stavros Niarchos Foundation (SNF) as part of its Global Health Initiative (GHI) through the SNF Global Center for Child and Adolescent Mental Health at the Child Mind Institute

### Evaluation

Submissions are evaluated on the [average precision](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.average_precision_score.html) of detected events, averaged over timestamp error tolerance thresholds, averaged over event classes.

Detections are matched to ground-truth events within error tolerances, with ambiguities resolved in order of decreasing confidence. For both event classes, we use error tolerance thresholds of 1, 3, 5, 7.5, 10, 12.5, 15, 20, 25, 30 in minutes, or 12, 36, 60, 90, 120, 150, 180, 240, 300, 360 in steps.

You may find Python code for this metric here: [Event Detection AP](https://www.kaggle.com/code/metric/event-detection-ap/notebook).

















