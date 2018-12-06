# UnityML

This code is the bare necessity needed to connect to a UnityML agent.

This tutorial uses an older version of Unity ML-Agents. These steps may not work with the most recent version of ML-Agents. For that, it is recommended that you use the version in the repository. It is also recommended that you create a virtual environment for this project. This will give you a clean slate for the installing the packages. If you do not use a virtual environment and you have already installed a version of unityagents, it may not work with tutorial.

The meat of the repository is the <a href="ml-agents-master/python/test1.py">test1.py</a> file located in the ml-agents-master/python/ folder. If you're just interested in how python interacts with Unity in the simplest of examples, check out this file. Else, continue with the setup process to get everything up and running. Keep in mind, this python script will not work alone.

<br/>

# Setup

<b>Install</b>

1. Clone this repository.
2. If you're using a virtual environment, activate it now.
3. In the terminal, navigate to the python/ folder located in the ml-agents-master/ folder.
4. Once inside the python/ folder, run the command 'pip3 install .' (don't forget the period) to install everything you need for this tutorial.

<br/>

<b>Unity</b>

5. Now that the installs are complete, open the Unity editor and create a new project.
6. Once open, go to Edit -> Project Settings -> Player. Then, in the inspector, under 'Other Settings', make sure that Scripting Runtime Version is set to '.NET 4.x Equivalent'.
7. This should prompt you to restart the Unity editor. Do so and continue.
8. In your file explorer (or terminal), locate the ML-Agents/ folder in the ml-agents-master/unity-environment/Assets/ folder. Once found, copy the ML-Agents/ folder to the Assets/ folder of your new Untiy project.
9. In the Unity editor (REMEMBER, this is now in the Unity editor, not your terminal or file explorer), navigate to the 3DBall/ folder located in the Assets/ML-Agents/Examples/ folder. Once in the 3DBall/ folder, double click the 3DBall.unity object to the open the 3DBall environment in the hierarchy.

10. In the project Hierarchy, select the Ball3DBrain object within the Ball3DAcademy object.
11. Now, in the inspector, make sure Brain Type is set to 'External'. This is important for your python script to interact with the Unity brain.
12. Finally, go to File -> Build Settings. Select the intended Platform (most likely PC, Mac & Linux Standalone) and select a Taget Platform and Architecture in the dropdown menus. Then hit Build, give it a name, and set the location to the same python/ folder from above, located in the ml-agents-master/ folder. The location is important so make sure this step is done correctly.

<br/>

<b>Run</b>

13. Once the build is successful, navigate back to the python/ folder, again, located in the ml-agents-master/ folder.
14. There you will find a python file named <a href="ml-agents-master/python/test1.py">test1.py</a>. This is the script that contains the bare-necessities needed to connect your python AI with Unity. Open the <a href="ml-agents-master/python/test1.py">test1.py</a> file in any text editor.
15. The first line should say something like 'env_name = "unity_executable"'. Replace the 'unity_executable' within the double quotes with the name of the Unity executable you just built. Note, you do NOT need the include the .extention with the name.
16. Also note that, if you were following along correctly, the <a href="ml-agents-master/python/test1.py">test1.py</a> and the Unity executable you just built, are in the same folder. This is important or the script will not be able to find the Unity executable. (unless you specify the correct path youreslf)
17. Last but not least, while still in the python/ folder, again, located in the ml-agents-master/ folder, run 'python3 test1.py' in the terminal.

<br/>

# That's it!

A small window should open and run the Unity environment for 20 episodes and close. The terminal will show a few details as well.


<b>More details explaining the python code within the script itself are soon to come...</b>
