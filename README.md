# MouseVR
Repository holding Bonsai workflows and Godot project for MouseVR


The Game folder holds the Godot project, which can be imported once you open your Godot program. Beware it uses ZeroMQ to interface with Bonsai, so it has to be the .NET version of Godot.

The Bonsai_workflows folder holds a couple of existing bonsai workflows.

- VR_Godot holds the version of the Godot integrated script prior to the Bonsai workshop.
- StimulusactivationButtonTest holds a script that allows testing of the custom made electronics made for the MouseVR setup. This allows activation of the electronics components upon pressing left/right/up.
- VR_Godot_basler_FullVideo_5sVideos holds a script compiled at the end of the Bonsai workshop in March 2024. TODO write down the full functionalities of the script. 
- - One thing to be aware of in the video saving is that currently it saves both a full video (in the CompleteVideos folder that is created), in the main script, and under the SelectMany it also individually saves a video upon stimulus interaction it saves a video for each interaction with a stim cube, and saaves in a folder of the corresponding stim cube, and the time and date info (NOT as DD/MM/YYYY since the / will create subfolders, and it impairs the video saving i.e. the video is not saved correctly).
- - what happens in the video is saved in an Output folder in a excel file. this logs different parameters of movement from Godot, when the mouse is in proximity with one type of the 3 types of stim cubes (logs '1' for being in proximity of the cube until a certain amount of time after leaving the cube). It also logs when it starts and saves certain videos for individual stimuli and save them as e.g. Circle/Circle_6_16_3_39.avi, and logs this until a new video is being logged e.g. Diagonal/Diagonal_6_16_3_43.avi
- -  TODO fix the time stamping, currently logs day, hour, minute, second.
- - TODO investiate how long time delay there is form cube proximity entry to stimulus is elcited and video recording starts. Currently seems to be quite a delay.
