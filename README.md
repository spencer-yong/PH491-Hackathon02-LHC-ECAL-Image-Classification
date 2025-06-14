# PH491-Hackathon02-LHC-ECAL-Image-Classification
<a target="_blank" href="https://colab.research.google.com/github/spencer-yong/PH491-Hackathon02-LHC-ECAL-Image-Classification/blob/main/PH491_Hackathon_2_group1_Kodatt_Rollins_Young.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

Image classification project using dataset from the Electromagnetic Calorimeter (ECAL) in the Large Hadron Collider (LHC) megaproject. A calorimeter measures the energy of an interaction. Each pixel in the image corresponds to a detector cell, while the intensity of the pixel corresponds to how much energy is measured in that cell. Timing of the energy deposits are also available, though this may or may not be relevant. The dataset contains 32x32 Images of the energy hits and their timing (channel 1: hit energy and channel 2: its timing) in each calorimeter cell (one cell = one pixel) for the two classes of particles: Electrons and Photons. The dataset contains around four hundred thousand images for electrons and photons.


A series of convolutional neural network (CNN) architectures were tested on a limited sample of the dataset for performance reasons. The final architecture, VGG16, first used by the Visual Geometry Group at University of Oxford, was trained on 80% of the data, tuned on 10% of the data, and finally tested for ROC/AUC performance on the remaining 10% of the data.
