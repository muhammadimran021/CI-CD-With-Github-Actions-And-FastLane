# Fastlane Firebase App Distribution CI/CD using Github Actions

GitHub action pipelines with fastLane for app distribution 

GitHub action will trigger on every push or on pull request 

<img width="258" alt="Screen Shot 2023-01-05 at 11 50 41 AM" src="https://user-images.githubusercontent.com/16763500/210719156-22b416c0-9a68-45e4-814a-706ed201f728.png">

After trigger GitHub action it will get the branch name 

<img width="579" alt="Screen Shot 2023-01-05 at 11 36 16 AM" src="https://user-images.githubusercontent.com/16763500/210719328-7ca5387c-a217-4f74-bfdd-3a5825323583.png">

and get the last commit from it. 

<img width="573" alt="Screen Shot 2023-01-05 at 11 37 50 AM" src="https://user-images.githubusercontent.com/16763500/210719448-29c245e2-66f0-4a52-9a6f-715f4e9e19bd.png">

The purpose of getting last commit from branch if your commit contains message like (build apk for firebase)  the action will be continue the Gradle Build process else the action will be not continue .

<img width="465" alt="Screen Shot 2023-01-05 at 11 39 35 AM" src="https://user-images.githubusercontent.com/16763500/210720023-a10c37e6-d03e-4ec6-bb6e-7be4a69a2762.png">

The purpose of getting branch name is to take a decision to create a debug build or to create a live build
For example if your branch is master it will create a release build and distribute it on firebase with the help of fast lane.

<img width="708" alt="Screen Shot 2023-01-05 at 11 58 15 AM" src="https://user-images.githubusercontent.com/16763500/210720457-fd657442-f82d-4754-9a57-aae51af20b12.png">


Or if the branch name is like Stage or Development it will create a debug apk

<img width="576" alt="Screen Shot 2023-01-05 at 12 00 16 PM" src="https://user-images.githubusercontent.com/16763500/210720784-0928f363-4ff7-4c00-ac53-cc06b42568a6.png">

NOTE: I create this actions according to my project need you can just modify it according to your project development lifecycle 
