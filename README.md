# Nymbots Final Degree Project
I did my final degree project in collaboration with another student in the robotics lab of Prof. Gal A. Kaminka, as a part of his research within the ISF Smart Swarms Center – a collaborative large-scale research project.  
For more information about the ISF Smart Swarms Center: https://u.cs.biu.ac.il/~kaminkg/research/smart-swarms/
  
Our project laid the groundwork for utilizing robots (in our case, small robots called "nymbots") to better understand the behavior patterns of locusts and locust swarms.

A significant part of the project was creating a robotic sensor which enables the nymbots to detect obstacles and other nymbots in their vicinity.  
Other nymbots can be detected via four possible vision models, which simulate the four assumed ways locust interprets seeing other locusts inside its field of view:
1. X Ray - The nymbot sees all nymbots inside its FOV, even if they are hidden behind other nymbots (imaginary situation).
2. Ignore Partially Hidden – The nymbot ignores nymbots that are completely or partially hidden behind other nymbots. 
3. Ignore Completely Hidden - The nymbot ignores nymbots that are completely hidden behind other nymbots. 
4. Partially Hidden Is Small Nymbot – when nymbots are partially hidden behind other nymbots, the nymbot interprets each part it sees as a small nymbot.

A short video demonstrating the sensor in action:


https://user-images.githubusercontent.com/73775638/203353761-4d22d0f9-1731-4f2b-abfc-36eed3f7a590.mp4  


Using the sensor's detection ability, we implemented a collective motion model. In each frame, each nymbot moves in the headings average of the nymbots in its vicinity. A convergence of the nymbots can be observed a while after the program starts running.
The implementation includes obstacle avoidance and managing nymbots collisions. 


https://user-images.githubusercontent.com/73775638/203353877-193e0d0e-25f6-431b-b2b8-a0ff768fdc19.mp4


