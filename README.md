# LeapMotion_BrainConnectivityLeap

Hello, my name is Filipe Rodrigues and I'm a Biomedical Engineering student from Lisbon, Portugal. I've been working with the Leap Motion Controller for my Master’s Thesis and It's been great!
Brain Connectivity Leap is a by-product of that work. Essentially, it’s an app in which you can interact with a 3D Reconstruction of an actual human Brain and its underlying Network of Connectivity Graphs. You can “disturb” the human Connectome either as a whole, or as a set of structural and functional segments. It was developed by Filipe Rodrigues (lead developer), Ricardo Ribeiro and Hugo Alexandre Ferreira at the Institute of Biophysics and Biomedical Engineering (IBEB), Faculty of Sciences of the University of Lisbon (FCUL) in the scope of a research project financed by Fundação para a Ciência e Tecnologia (FCT) and Ministério da Ciência e Educação (MCE) of Portugal (PIDDAC) under grant PTDC/SAU-ENB/120718/2010.

KEY FEATURES:
- Actual Reconstructions: Both the Brain mesh and the Network of Connectivity Graphs were calculated using real medical images and the [Multimodal Brain Connectivity Analysis (MIBCA)](http://www.mibca.com) toolbox. The brain model was reconstructed from Magnetic Resonance Images processed using MIBCA-pipelined [Freesurfer](http://surfer.nmr.mgh.harvard.edu/) and the graphs were computed from Diffusion Tensor Imaging based tractography data processed using MIBCA-pipelined [Diffusion Toolkit / Trackvis](http://www.trackvis.org/dtk/) and [Brain Connectivity Toolbox](https://sites.google.com/site/bctnet/);
- Gesture Recognition: Allows for a pretty reliable recognition of the Trigger (thumb tip touching index base while index is extended) and Pinch (thumb tip touching index tip while middle and ring finger are extended);
- Widgets: Sliders & Scrollers from the standard core assets. Can be hidden / displayed at run time;
- Leap Interaction: One & Two Handed Interaction;
- Custom made Affordances for most of the implemented features;
- VR Support: Though this is not as tested as the non-VR version;

WHAT'S NEW:
- Fixed an error that caused an incorrect reading of the connectivity files. Kudos if you noticed that the connectivity network looks a bit different now:) 
- Added comprehensive text Instructions that pop up at launch;
- Added must-have features like the "ESC" to quit keyboard command & the leap motion disconnection notice. This should have been there in the 1st place!;
- It is now possible to interact with individual brain segments, meaning that you can select, translate & rotate them. Each hand has its own set of selections, which can be distinguished by the Hand Model's signature color;
- Removed the 2 buttons that were in the previous version. I came to the conclusion that the segment coloring was rather useless & that a slider would give the user more control over the network’s coloring. Instead, we now have 2 sliders that control the color code applied to the graphs. One adjusts the type of color coding & the other its intensity;
- Added 2 Scrollers that list the currently segments (one for each hand);
- Added a feature that compares the currently observed connectivity matrix with a Health Reference Matrix (computed from data acquired from several healthy subjects). It then colors each graph according to said comparison. If it has a weaker connection than it "should" have, we paint it red (deficit). If in turn it has an excessive connection strength, we paint it yellow;
- Added a collection of custom made affordances / pseudo-widgets. Whereas the 1st version had only a scale-beam that showed up when the user was in scaling mode, the present one has this sort of visual cues for most of the available interaction tools (point, select, deselect, hover, scale, left & right hand gesture indicator, left & right hand finger counter);
- Made some optimizations to the brain mesh (reduced its poly count from 1.8M to 500k);

Like I said, the new version displays text instructions at launch but if you're feeling lazy, you can always watch the new Brain Connectivity Leap [YouTube Video](https://www.youtube.com/watch?v=bSz0j2-K_3Y) to get the general idea of how everything works:)

WHAT'S TO COME:
- Haptic Feedback! As part of my Thesis, I'm designing a glove (hardware & software) that will provide tactile feedback in this & other Unity apps. We already have a working prototype, just need to dress it up a bit:p
- Electrophysiological Feedback! Another feature of the aforementioned glove:) The user's ECG, EDA & EMG signals will be acquired at run time & used to modulate the scene (provided he's wearing the glove);
- Dynamic Tutorial. I know that the current text instruction are a bit lengthy & that that's no fun. I'll try to tackle this in the upcoming versions & make a step-by-step interactive tutorial;
- Matrix selection at run time. As it is now, you're stuck looking at the matrix I had selected when the build was made. We want to change this;
- Support for new Segmentation Atlases. The current version uses the AAL - Automated Anatomical Labeling - Atlas to parcellate the brain into 116 segments. Support for 4 or 5 other atlases is in the making;
- Suggestions?:) Any feedback is good feedback!

That's pretty much it:) Hope someone enjoys it. Thanks and cheers!
