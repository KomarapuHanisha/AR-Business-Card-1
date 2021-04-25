# AR-Business-Card
Recruitment Project for 1st year
# AR-BUSINESS-CARD
A Simple business card might not have all the information related to you, but in an AR Business card, we get more detailed information with more reality and less paperwork.AR business card uses live image tracking technology, which is available for both ios and Android, the application can detect and track the card.

## PREREQUISITES:
1. Unity 3D
2. Unity package
3. Vuforia Engine
4. ARCore/AR Kit
5. AR Foundation
6. XR Plugin management Package

## FLOW CHART:
![](Flowchart.jpeg)
                          
## UNITY SETUP:
1. After installing Unity Hub and opening, we will click on “New,” then select “3D” as a template, name the project and select its location. Then we click on “Create.”
2. We have saved the given design package “Assembly.unitypackage” and open the file.
3. We click on Import.
4. On the left, under “Sample Scene,” we have to delete both “Main Camera” and ‘Directional Light” and Save.
5. We go to the “GameObject” tab and select “Vuforia Engine” and then “AR Camera.”
6. We left Click on “AR Camera” and then select “Vuforia Engine” and then select “Image.” We would notice that we have “Image Target: added underneath AR Camera. Then we save.
7. Now we have to add the database, so we go to https://developer.vuforia.com/vui/auth/register to register with your information, then we say “create an account,” and a link will be sent to the email address for verification. 
8. Now we login to https://developer.vuforia.com/vui/auth/login with the previously set email and password.
9. After getting logged in, we click “Get Development Key” and then proceed to “License Manager” where we will enter a License name and then check the box below and click “Confirm.”
10. Now that we have a license created, we click on it and copy the given license key.
11. We then close that window and select “AR Camera,” and on the right, we select “Open Vuforia Engine Configuration” and paste the License key we copied. Then we click “Add License.”
12. Now, we go back to Vuforia and select the “Target Manager” tab. We click on “Add Database”. We give it a name and check Type “ Device” then click “create”.
13. Now that we have created a database, we have to add targets. We click on it and then select “Add Target”.
14. We then Select Type “Single Image”. We browse to “AR Business card.jpg”. Then we say the width is “1” and select “Add”.
15. Then we add our 2nd Target following the same steps but choosing “Untitled.jpg” instead.
16. Then we add our 3rd Target by Selecting Type “3D Object” and browsing to “7gc.od” and then clicking “Add”.
17. Now that we have our database with our targets, we select “Download Database All” and then check “Unity Editor”. Then select “Download”.
18. We open the file we just downloaded and select “Import”.



## AR BUSINESS CARD DESIGN:  
Our AR business card would be designed in such a way that proper solid shapes and colors are used to make the image recognition possible. 
## AR DEVELOPMENT:
1. Under “AR Camera”, we create an “Image Target”.
2. We go to image Target and select the previously created database and “AR business card” as Target
3. Then we add 3D Object  Cylinder and scale it as x=1 and z=0.7.
4. Now we go to Business Card Folder and select a photo and drop it in the cylinder
5. Then we copy-paste five cylinders and paste their pictures inside.
6. Now we add 3D Object  Quad and then rotate it 90 degrees in the x-axis direction.
7. We then select the user avatar and drop it in the quad
8. Then we add 3D Object Text (Text Mesh Pro)
9. We go to Window  Text Mesh Pro and Import both “TMP Essential Resources” & “TMP Examples and Extras”.
10. We select Font size as “1.5” and Fill in User Details such as “Name” and “Address”
11. Now we go to the “Assets” folder and create a folder named “Scripts”. Then inside the folder, we create a “C# Script” and rename it according to what we want. For Example “LinkedIn”.
12. Then we open the script and delete methods “Start()” and “Update()”
13. Now, we add the method “OnMouseDown()” and add the line “Application.OpenURL();” where we paste the link of the wanted social media platform between the ().
14. Then we pick the script and drop it in “Add Component” for that object.
15. We repeat the same steps above for the rest of the social media links.
 
## IMAGE RECOGNITION USING VUFORIA:
Vuforia supports 2D as well as 3D object recognition. The required target will be scanned using the Object Scanner app provided by the Vuforia engine for Android. We need to add this target to the Targets database online, similar to how we added the image targets.
1. We select AR Camera ->Vuforia Engine ->3D Scan.
2. We make sure that the Target is 66.od.
3. Then, we include the controls from the business card under ObjectTarget.
4. Set the position of the objects to 0 so that they would be close to the object target. And adjust the placement according to the requirement.

## EXPORT INTO MOBILE APP:
1. We go to file  Build Settings
2. Then we select “Add Open Scenes.”
3. Then, we select the preferred platforms. In this case, it’s iOS or Android.
4. Now, we select “Switch Platform” and then select “Build and Run.”

## OTHER APPLICATION:
Apart from the A.R. business card, Auguemented reality concept can be used in other ways as well like:
1. As a poster: The popups from the card can be used as animations from the posters.
2. To showcase movie trailers and clips 
3. Can be modified into a Greeting card and postcard. Inclusion of pictures, popups, animations would help.
## WORK DONE SO FAR:
We have installed the unity hub and downloaded all the required packages like Vuforia engine, unity package,  AR foundation …. 
Since one of our team mates tested positive for covid-19 ,we couldn’t start the design work yet .But we make sure that we will complete the project in time .
## ISSUES FACED:
Initially we had a error while installing unity engine 2020 version as it didn’t have in built vuforia engine .So we are using the 2019 version for convenience
