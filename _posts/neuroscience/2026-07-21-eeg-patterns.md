---
title: "5 EEG Patterns"
categories: neuroscience
subcategories: eeg-101
description: "Overview of well-known patterns that can be encountered in EEG recordings, and considering their meaning."
link_title: eeg-patterns
reading_time: 7
layout: post
title_image: yes
home_page_invisible: true

---

# What are EEG patterns?

EEG consists of electrodes, each recording the relative strength of neural signal at a different point on top of the skull. The recordings look like a number of "squiggly lines", each line representing one electrode.

<img src="/assets/posts/{{page.categories}}/{{page.link_title}}/images/eeg_recording.png" alt="Example of EEG recording" class="image-centre">

<div class="image-description">An example of EEG recording. Image source: Wang Q, Yang J, Yu C, Deng Y, Wen Q, Yang H, Liu H and Luo R, licensed under the <a href="https://en.wikipedia.org/wiki/en:Creative_Commons">Creative Commons</a> <a href="https://creativecommons.org/licenses/by/4.0/deed.en">Attribution 4.0</a> International license.</div>


These lines are often related to each other, as they all represent the signal from various regions of the brain that may overlap and influence other regions. Therefore, certain patterns often emerge, where a subset of the lines all create particular "shapes" caused by a strong signal spreading across several brain regions.

Each line represents the relative strength of neural signal recorded at each electrode. The arrangement of electrodes and their names is standardised as follows:
- Electrodes at the front of the brain: Names begin with "F" (for frontal lobe)
- Electrodes at the back: Names begin with "O" (for occipital lobe)
- Electrodes on the sides: "T" (temporal lobe)
- Electrodes on the very centre of the top: "C" 
- Other electrodes on top/back: "P" (parietal lobe)

Many EEG patterns are only visible on particular electrodes. For example, the blink artifact is only visible on "F" electrodes, as they are the closest to the eyes.

<img src="/assets/posts/neuroscience/{{page.link_title}}/images/eeg_electrodes.png" alt="Common arrangement of EEG electrodes" class="image-centre">

<div class="image-description">Left: Standard arrangement and naming convention of electrodes when 64 electrodes are used. Top right: Brain regions corresponding to electrode groups.</div>

# What causes the patterns?

## Sources inside the brain

In their purest form, the patterns are caused by one or more active regions inside the brain. As an example, the alpha rhythm (see "2. Alpha rhythm") occurs likely due to rhythmic cellular interactions between the neurons on top of the head, at the back of the head, and in the thalamus (in the deep parts of the brain). 

The patterns can occur due to one region being active, or due to multiple independent regions emitting signals that superimpose.

The physical source of the patterns is not easy to identify, as EEG on its own can't detect the location of the signal - it only measures the relative strength of the signal(s) which can have multiple possible origins. Other methods such as fMRI or MEG are often used to find the physical source.

## Artifacts - sources outside the brain

Some of the patterns are "artifacts" - byproducts of some other activity that didn't originate in the brain. EEG detects voltage on the scalp, but it's unable to tell the voltage source. Therefore, the EEG recording can become contaminated by other sources that disturb the electric field. Examples include: 

- Power line noise (50 Hz in Europe): caused by AC power lines and wiring.
- Eyes blinking: caused by the cornea being positively charged and the retina negatively charged. During closing of the eyes, the eyeballs rotate upwards (Bell's phenomenon), causing a disturbance in the electric field.
- Pulse artifact: caused by an electrode being placed on top of a pulsating blood vessel.

Many of the artifacts can be filtered out. For example to filter power line noise, a filter of 50 Hz (in Europe) is sufficient. 

Other artifacts are more difficult to filter out algorithmically, but are easy to filter out visually - for example, the pulse artifact manifests as waves of the same frequency as the heartbeats.

<img src="/assets/posts/{{page.categories}}/{{page.link_title}}/images/pulse_artifact.png" alt="Pulse artifact" class="image-centre">

<div class="image-description">Example of a pulse artifact. Notice that the frequency corresponds to the heartbeat frequency (the red line). Source: eegpedia.org</div>


# What's the point of identifying the patterns?

The first clinical application of EEG after it was first developed in 1920s was detecting epilepsy. In the modern days, this is still one of its most prevalent uses, as there's particular EEG patterns that are strongly indicative of epilepsy and are used as part of diagnosis.

Other EEG patterns help to detect the mental state - for example, there's EEG patterns that indicate drowsiness or being drugged, patterns that indicate the phase of sleep, and patterns that indicate alertness or focus. EEG signals can also be used to give the prognosis for patients in coma, as different patterns indicate different levels of remaining mental activity.

<img src="/assets/posts/{{page.categories}}/{{page.link_title}}/images/seizure_eeg.png" alt="Seizure visible in EEG" class="image-centre">

<div class="image-description">EEG recording during a seizure. Source: eegpedia.org</div>

Now, onto the list of 5 EEG patterns:

# 1. Spike and slow wave 

This pattern is indicative of epilepsy. 

An important note to interpret EEG recordings is that, by convention, **positive brain activity is represented by the lines on the graph going down**, and **negative brain activity is represened by the lines going up.**

This pattern begins with a sudden strong burst of electric activity (the spike), often starting in a hyper-excitable area of the cerebral cortex. This excitation then triggers an inhibitory response to "shut down" the firing - the slow wave. This inhibitory response it thought to be done by neurons in the thalamus (a deep part of the brain) releasing GABA (the brain's primary inhibitory chemical) back onto the cortex and other parts of the thalamus.

This can then become a repeating pattern, as when the inhibition fades, this triggers a rebound burst of firing. The brain can then become "stuck in a loop", resulting in a spike-and-wave seizure.

<img src="/assets/posts/{{page.categories}}/{{page.link_title}}/images/spike_slow_wave.png" alt="Spike and slow wave" class="image-centre">

<div class="image-description">Example of spike and slow wave patterns. Source: eegpedia.org</div>


# 2. Alpha rhythm

Alpha rhythm was the first EEG pattern identified in humans in 1929 by Hans Berger. That's likely because it's a commonly present and easily identifiable rhythm in humans due to its characteristic wave shape.

It's defined as a wave 8-13 Hz that's present at the back head regions (electrodes "P" and "T") in people who are relaxed but awake and have their eyes closed. 

It disappears when people open their eyes, unless the environment has no light or the person is not focused on anything visually. Therefore, the alpha rhythm might be related to a readiness to see something. It's usually absent or severely reduced in people who have been blind from birth. For people who became blind later in life, they often retain some alpha activity that then reduces over the years following the loss of sight.

The alpha rhythm also disappears with drowsiness or concentration. Therefore a present alpha rhythm indicates that the person is (1) awake, (2) relaxed, and (3) not drowsy.

<img src="/assets/posts/{{page.categories}}/{{page.link_title}}/images/alpha_rhythm.png" alt="Alpha rhythm" class="image-centre">

<div class="image-description">Alpha rhythm visible across "P" and "T" electrodes. Source: eegpedia.org</div>


# 3. Blink artifact

This artifact (a pattern created by a source outside of the brain) is caused by the eye's cornea being positively charged and the retina negatively charged. 

<img src="/assets/posts/{{page.categories}}/{{page.link_title}}/images/eye_structure.png" alt="Eye structure" class="image-centre">

<div class="image-description">Eye structure, with the cornea visible at the front and retina at the back. Image source: www.scientificanimations.com, licensed under the <a href="https://en.wikipedia.org/wiki/en:Creative_Commons">Creative Commons</a> <a href="https://creativecommons.org/licenses/by-sa/4.0/deed.en">Attribution-Share Alike 4.0 International</a> license.</div>

During closing of the eyes, the eyeballs rotate slightly upwards (Bell's phenomenon), and the moving difference in charge results in a disturbance in the electric field. 

This artifact is generally only seen in the electrodes on the front of the head (electrode names beginning with F). The closer the electrode is to the eyes, the stronger the artifact.

<img src="/assets/posts/{{page.categories}}/{{page.link_title}}/images/blink_artifact.png" alt="Blink artifact" class="image-centre">

<div class="image-description">Blink artifact, seen 5 times across most of the F electrodes. Source: eegpedia.org</div>


# 4. Sleep spindles

Sleep spindles are a burst of rhythmic activity that occurs during sleep - specifically, during stages 2 and 3 of NREM (non-rapid eye movement) sleep. Those sleep stages are when the body moves from light (stage 2) into deep sleep (stage 3).

Sleep spindles are normal, healthy activity. They have a role in memory consolidation: a study from 2007 by Schabus et al. showed that some sleep spindles activate the hippocampus (responsible for forming new memories) and parts of the frontal cortex resposible for combining new memories with established knowledge.

Sleep spindles can sometimes still be visible for people in a coma. When that is the case, it's usually a sign of a better prognosis than a coma without sleep spindles.

<img src="/assets/posts/{{page.categories}}/{{page.link_title}}/images/sleep_spindle.png" alt="Sleep spindle vs K complex" class="image-centre">

<div class="image-description">Sleep spindle compared with a K-Complex (another common EEG pattern in sleep).</div>

<img src="/assets/posts/{{page.categories}}/{{page.link_title}}/images/sleep_spindles.png" alt="Sleep spindles" class="image-centre">

<div class="image-description">Sleep spindles visible across "C" and "O" electrodes.</div>


# 5. Beta rhythm

Beta rhythm was the second pattern identified by Hans Berger in 1929 alongside the alpha rhythm.

 It's defined as activity with frequency of 13 Hz or greater. The only faster rhythm is gamma activity, though gamma activity (30+ Hz) is not commonly used in clinical EEG due to its overlap with muscle artifacts.

When beta rhythm is localised to the front and centre of the brain, it's associated with drowsiness or sleep onset, and sometimes it's linked to anxiety and vigilance.

When beta rhythm is spread across the larger portion of the brain, it's linked to sedative medications and certain drugs such as cocaine and amphetamine.

<img src="/assets/posts/{{page.categories}}/{{page.link_title}}/images/beta_rhythm.png" alt="Beta rhythm" class="image-centre">

<div class="image-description">Beta rhythm visible in "F" and "C" electrodes, indicative of drowsiness and sleep onset. Source: eegpedia.org</div>

<img src="/assets/posts/{{page.categories}}/{{page.link_title}}/images/brainwaves.png" alt="Comparison of beta rhythm with other common rhythms" class="image-centre">

<div class="image-description">Comparison of Beta rhythm with other common rhythms.</div>


# Further Reading

- "Atlas of EEG Patterns" by John. M. Stern and Jerome Engel - the best explanation of a large number of EEG patterns. Expensive book to buy, but can be found in other places online.
- www.eegpedia.org - list of EEG patterns and a summary their features. It's a good quick reference, but it doesn't include comprehensive explanations like "Atlas of EEG Patterns".

# Other Sources

- Spike and slow wave: https://pmc.ncbi.nlm.nih.gov/articles/PMC3168114/
- Images: wikimedia.org