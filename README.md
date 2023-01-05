# Fastlane Firebase App Distribution CI/CD using Github Actions

Hi all  I have implement GitHub action pipelines with fastLane for app distribution 

GitHub action will trigger on every push or on pull request 

After trigger GitHub action it will get the branch name 

and get the last commit from it. 

The purpose of getting last commit from branch if your commit contains message like (build apk for firebase)  the action will be continue else the action will be not continue .

The purpose of getting branch name is to take a decision to create a dev build or to create a live build
For example if your branch is master it will create a release build and distribute it on firebase with the help of fast lane.


Or if the branch name is Stage or Development  it will create a debug apk


