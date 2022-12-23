# I have (Unofficially) taken over this project because I wish to use this for my game development.
### This fork is for me to make changes and port to Blender 3.2.1
This fork is not meant to take over the original, but the original repo has been abandoned for almost 2 years.<br>
The reason for the fork detachment is because i wish to see those green squares on my profile for dopamine.<br>
Original repo: [@specoolar/Blender-BakeLab2](https://github.com/specoolar/Blender-BakeLab2)

# Small guide to export models with textures to FBX
###### You can't imagine how much effort I have put into export with textures (There are NO concrete guides). I have spent WEEKS on figuring it out.
### Select your object, which you wish to export:
<img src="https://user-images.githubusercontent.com/44818698/208796516-b65b8a17-9e58-4827-b5e2-39653d561be1.png" width=400/>

### Select bake mode
![image](https://user-images.githubusercontent.com/44818698/209251117-b3218991-af75-4f0d-a722-6cbd231c3144.png)
Note: "All To One Image" is used for exporting to FBX

### Open BakeLab tab on the right menu:
<img src="https://user-images.githubusercontent.com/44818698/208796603-f23e3a32-40c5-44d7-b92a-ca3471ca1a67.png" height=400/>

### CLick "Unwrap" and choose your unwrapping prefences and click "OK":
<img src="https://user-images.githubusercontent.com/44818698/208796704-3f0eb6bc-7fbb-472c-9182-cdedfa51648a.png" width=400/>

### Add your texture types, that you want to bake:
<img src="https://user-images.githubusercontent.com/44818698/208796897-2201cf6a-8c39-425e-9756-07713b048e2f.png" height=400/>

### !IMPORTANT! Choose "Output" to "Save" and choose your location for your baked textures:
<img src="https://user-images.githubusercontent.com/44818698/208797034-95b8edb5-f641-421c-99d0-5af4a326ef0d.png" width=400/>

### !IMPORTANT! Check if your objects has more than one UV mapping:
<img src="https://user-images.githubusercontent.com/44818698/208797191-cd628410-30f6-4e65-ac34-078a8fed9d96.png" width=400/><br>
If you have more than one then delete the unused one. If you don't know which one is unused then just clear UVs and re-Unwrap:<br>
<img src="https://user-images.githubusercontent.com/44818698/208797379-10f34c45-1efc-4b5c-b9f7-b83bcfaa5ea2.png" width=400/>

### TIME TO BAKE!!!
<img src="https://user-images.githubusercontent.com/44818698/208797414-d1b4a175-1e26-4bb0-bbce-e47e40b53b2e.png" width=400/><br>
You just have to click the big button called "Bake" 🤦🏻‍♂️

### Now press "Generate Materials"
<img src="https://user-images.githubusercontent.com/44818698/208797580-cd2ea0a9-5f3d-4bbc-a64e-315c4eae93be.png" height=400/>

### Next to the export part:
<img src="https://user-images.githubusercontent.com/44818698/208797749-2da3241d-65bb-46d4-a5b5-c7f08b49ea01.png" width=400/>

### Choose the correct export settings
<img src="https://user-images.githubusercontent.com/44818698/208797899-3f69fe18-b6a1-4f3c-b752-0e7e685ca015.png" width=400/><br>
Path mode: Auto ==> Copy<br>
Click the small button to the right: <img src="https://user-images.githubusercontent.com/44818698/208800361-74784af8-023e-4d61-afb5-4dc7cf2baf98.png" width=40/>
<br>
Object types: * ==> Mesh

### Finally! Press export!!
And here we go!!!<br>
<img src="https://user-images.githubusercontent.com/44818698/208798164-185c6213-5e5b-4a6e-b989-5fbfdf970c90.png" width=400/><br>
###### This object was opened in Paint 3D

# Import FBX with texture into Unity
### Go back and bake a smoothness map instead of roughness
![image](https://user-images.githubusercontent.com/44818698/209249522-633b5d34-3b90-4592-94b0-d6d4c2a1992c.png)<br>
![image](https://user-images.githubusercontent.com/44818698/209249534-d2ad9241-d636-4793-a8c3-23afaede8991.png)<br>
Enable this checkbox, then rebake and export.
## Import into Unity
<img src="https://user-images.githubusercontent.com/44818698/208798522-87788bba-9b02-4147-ac01-61cbb4d23ce8.gif" width=400/><br>
Notice that this isn't showing textures.<br>
#### Extract textures from FBX
Just select the object in Unity and in the inspector, extract the textures<br>
<img src="https://user-images.githubusercontent.com/44818698/208798775-ccd433d9-9a5f-4622-b87e-66b0087f3cd3.png" width=400/>

#### Profit?
<img src="https://user-images.githubusercontent.com/44818698/208798899-b867f538-69e2-4dac-b0a1-c5abf3bff145.png" width=400/>
<br>
<br>
<br>

TODO: Move this guide to Wiki or create Youtube video instead (Minimum 24 minutes for some reason)
###### I probably won't do this but it's still a TODO

<br>
<br>
<br>
<br>
<br>
<br>
<br>

# This is the original README (I don't know what to do with this and i decided to just keep it here)
## Blender-BakeLab2
![Thumbnail](bakelab_thumbnail_text_logo_small.jpg)
BakeLab - A blender addon for baking images.<br>
For blender version 2.79 go to [here](https://github.com/Shahzod114/Bakelab-Blender-addon)

Main Features:
* Automatically create images, setup materials, bake objects and save/pack images in one click;
* Automatically generating materials;
* Anti-Aliased baking;
* Baking cycles displacement to real geometry;
* Bake any PBR attributes of your material by its name (Metallic, Roughness, Specular and etc);
* Adaptive image size by object's surface size;
* Unwrap and Bake Multiple Objects into one image;

video:
https://youtu.be/XmXek3TPZLk

![Screen](bakelab_screen.png)
