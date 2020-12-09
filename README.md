# Visual crowding in ANN

**Aim**
Visual crowding refers to a phenomenon in which identification of a target stimulus is severely impaired when it is surrounded by other objects. Psychophysical studies have shown that crowding occurs with various kinds of visual stimuli and that 'critical spacing' for crowding is proportional to target eccentricity. These results suggest that multiple cortical areas are involved in this phenomenon. However, very few neurophysiological experiments have been conducted measuring crowding effects. Here, I will examine how outputs from intermediate layers of ANNs are affected by various target-distractor relationships.

**Stimulus**

100 animal icons (H: 32 pix, V: 32 pix) are used for target or surround stimuli. Each icon is differently characterized by contour (and color). I will be testing the following target-distractor relationships.[ ](https://)
  * Target alone vs. Target + Distractor
  * Number of distractors : 2, 4, or 6 near distractors 
  * Target-Distractor distance: near, middle, or far distractors
  * Target saliency (e.g., color target + line distractor)

**Target network and layers**

I will look into intermediate convolutional layers (RF size > 50x50 pix) in AlexNet, VGG16, and Resnet50.

**Analysis**

1. Response selectivity: Correlation between 'Target alone' and 'Target+Distractor'
2. Response modulation: 'Target alone' vs. Target+Distractor' vs. 'Target alone + Distractor alone'
3. How #1 & #2 are different depending on layers (& networks)
4. Visualization of representative units. 

**Prediction**

Visual crowding will be stronger in higher layers as RF size gets larger. 
Contour processing units and color processing units will be differently affected in target saliency conditions. 

**Reference**

Whitney, D., & Levi, D. M. (2011). Visual crowding: A fundamental limit on conscious perception and object recognition. Trends in cognitive sciences, 15(4), 160-168.
