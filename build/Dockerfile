FROM circleci/android:api-28-alpha

###################
# GitHub Action description
###################
LABEL "com.github.actions.name"="Android Build"
LABEL "com.github.actions.description"="Build Android projects"
LABEL "com.github.actions.icon"="box"
LABEL "com.github.actions.color"="green"

LABEL "repository"="https://github.com/vgaidarji/android-github-actions/build"
LABEL "homepage"="https://github.com/vgaidarji/android-github-actions"
LABEL "maintainer"="Veaceslav Gaidarji <veaceslav.gaidarji@gmail.com>"

RUN sudo apt-get update
RUN sudo apt-get install ruby ruby-dev ruby-build
RUN sudo gem install fastlane

COPY entrypoint.sh /
ENTRYPOINT ["/entrypoint.sh"]
