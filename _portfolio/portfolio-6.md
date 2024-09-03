---
title: "Skin Track"
excerpt: "Project architecture which enables continuous touch-tracking for detection of gestures so as to send commands to the wearable watch.<br/><img src='/images/Skin_Track.jpg'>"
collection: project
---

SkinTrack is a wearable system that enables continuous touch tracking on the skin. It consists of a ring, which emits a continuous high frequency AC signal, and a sensing wristband with multiple 
electrodes. Due to the phase delay inherent in a high-frequency AC signal propagating through the body, a phase difference can be observed between pairs of electrodes. SkinTrack measures 
these phase differences to compute a 2D finger touch coordinate. Our approach can segment touch events at 99% accuracy, and resolve the 2D location of touches with a mean error of 7.6mm. 
As our approach is compact, non-invasive, low-cost and lowpowered, we envision the technology being integrated into future smartwatches, supporting rich touch interactions beyond the 
confines of the small touchscreen. We deployed the methodology using IoT and machine learning algorithm with SVM classifier with an accuracy of 85%. Presented as one of the Top 5 projects from IIT Kanpur at the Engineer’s Conclave held at IIT Bombay.
[Code](https://github.com/eclub-iitk/skintrack)
