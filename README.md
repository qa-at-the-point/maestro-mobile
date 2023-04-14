# Mobile Automation using Maestro

Maestro is a tool for Mobile Automation that uses YAML files for its tests.

## Setup

> ⚠️ You must create a free Maestro account for this repo to work!

Using Gitpod, a lot of the setup is already done for you 🎉

1. Open a Terminal and login to Maestro

    ```bash
    maestro login
    ```

    > 📧 This sends an email to authenticate. Click `Sign In` in that email and return to the Terminal

2. Run some flows on the cloud

    ```bash
    maestro cloud wiki-ios-app.zip .maestro/ios --format junit --include-tags=ios
    ```

    Things to note:

    - `maestro cloud` - the command to run Flows in the cloud
    - `wiki-ios-app.zip` - the iOS Wikipedia App to test
    - `.maestro/ios` - the folder to look for Flows to run
    - `--format junit` - have Maestro generate a JUnit XML that can be used in reporting tools like JIRA
    - `--include-tags=ios` - include all Flows that have this tag(s)

3. Once complete, open the `Uploads` page of your Maestro Cloud account to see the results!

## Documentation

There's a lot more you can do, so make sure to visit their docs for more details and advanced usages:

> 🔗 [Maestro Documentation](https://maestro.mobile.dev/)
