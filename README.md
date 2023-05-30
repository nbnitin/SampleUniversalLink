# SampleUniversalLink

Add domain name under plist, entitlement, Project Settings > Info > URL Types
<img width="830" alt="Screenshot 2023-05-30 at 9 24 43 AM" src="https://github.com/nbnitin/SampleUniversalLink/assets/5785670/063f2435-2902-414d-a346-98164a6df5de">
<img width="968" alt="Screenshot 2023-05-30 at 9 24 53 AM" src="https://github.com/nbnitin/SampleUniversalLink/assets/5785670/9c8effe1-2da5-43c6-8cef-0440a55db071">
<img width="977" alt="Screenshot 2023-05-30 at 9 25 12 AM" src="https://github.com/nbnitin/SampleUniversalLink/assets/5785670/4b2c14ca-ef01-484f-b115-49ed63e60919">


Turn on Associate Domains from apple developer account for your app

Come under project settings, signing & capabilities add capabilities Associated Domains add domain

<img width="815" alt="Screenshot 2023-05-30 at 9 32 46 AM" src="https://github.com/nbnitin/SampleUniversalLink/assets/5785670/05c9962e-5b2d-4cd6-9d53-c552ccbeaa29">


If entitlement file not get added automatically create new from 
File menu > New File...
Select iOS > Resource > Property List
Name the new file "targetname.entitlements" (typically, "targetname" is the target name)
Don't forget to set your target's CODE_SIGN_ENTITLEMENTS build setting to be the path to entitlements file you just added.

<img width="960" alt="Screenshot 2023-05-30 at 9 35 32 AM" src="https://github.com/nbnitin/SampleUniversalLink/assets/5785670/f8684daf-77fd-4ada-a1e9-69b801141396">

Create a JSON file without extension with named 
apple-app-site-association

add below code to that json
{"applinks":{"apps":[],"details":[{"appID":"TEAM_ID.BUNDLE_IDENTIFIER","paths":["*","/"]}]}}

e.x.
{"applinks":{"apps":[],"details":[{"appID":"KKKKKKKKKK.com.xyz","paths":["*","/"]}]}}
