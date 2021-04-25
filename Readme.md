# Hi there! <img src="avatars/wave.gif" width="30px">

[My LinkedIn Profile](http://linkedin.com/in/sergei-tolmachev-21732a160)

## Autotests development

Creating scenarios that emulate human behavior to automatically test the product's performance.

<img src="avatars/Python.svg" alt="Python" width="46" height="46"> <img src="avatars/Pycharm.svg" alt="Pycharm" width="50" height="50"> <img src="avatars/Intelij_IDEA.svg" alt="IntelliJ IDEA" width="50" height="50"> <img src="avatars/Java.svg" alt="Java" width="50" height="50"> <img src="avatars/Selenium.svg" alt="Selenium" width="50" height="50"> <img src="avatars/Selenide.svg" alt="Selenide" width="50" height="50"> <img src="avatars/Gradle.svg" alt="Gradle" width="50" height="50"> <img src="avatars/JUnit5.svg" alt="JUnit5" width="50" height="50"> <img src="avatars/Rest-Assured.svg" alt="Rest-Assured" width="50" height="50"> <img src="avatars/Appium.svg" alt="Appium" width="50" height="50"> 

## Building infrastructure

Solving infrastructure problems for embedding the launch of autotests in CI / CD, containerization of browsers and mobile devices

<img src="avatars/Github.svg" alt="Github" width="50" height="50"> <img src="avatars/Jenkins.svg" alt="Jenkins" width="50" height="50"> <img src="avatars/Selenoid.svg" alt="Selenoid" width="50" height="50"> <img src="avatars/Browserstack.svg" alt="Browserstack" width="50" height="50"> 

## Visualization of test results

Generating reports that are understandable to the customer and setting up notifications to messengers about the status of tests

<img src="avatars/Allure_Report.svg" alt="Allure_report" width="50" height="50"> <img src="avatars/Slack.svg" alt="Slack" width="50" height="50"> <img src="avatars/Telegram.svg" alt="Telegram" width="50" height="50"> 

## Test management

Managing a large volume of tests in test management systems that support both manual and autotests, in conjunction with CI/CD tools and task trackers

<img src="avatars/Allure_EE.svg" alt="Allire_EE" width="50" height="50"> <img src="avatars/Jira.svg" alt="Jira" width="50" height="50"> 







<h1>Allure notifications :sun_with_face:</h1>
<h6>for telegram, slack, skype, email, mattermost</h6>

<h3>Languages:</h3>

![](readme_images/languages/United-Kingdom.png) ![](readme_images/languages/France.png) ![](readme_images/languages/Russia.png) ![](readme_images/languages/Ukraine.png)</h5>

| Telegram | Slack |
:-------------------------:|:-------------------------:
![shakal_screenshot](readme_images/telegram-en.png) | ![shakal_screenshot](readme_images/slack-en.png)
| **Skype** | **Email** |
`// todo` [#32](https://github.com/qa-guru/allure-notifications/issues/32) :nerd_face::computer: | ![shakal_screenshot](readme_images/email_en.png)

<h6>How to:</h6>

- [x] [Telegram config](https://github.com/qa-guru/allure-notifications/wiki/Telegram-configuration)
- [x] [Slack config](https://github.com/qa-guru/allure-notifications/wiki/Slack-configuration)
- [ ] [Email config](https://github.com/qa-guru/allure-notifications/wiki/Email-configuration)
- [ ] [Skype config](https://github.com/qa-guru/allure-notifications/wiki/Skype-configuration)
- [ ] [Mattermost config](https://github.com/qa-guru/allure-notifications/wiki/Skype-configuration)


<h6>CommandLine options</h6>
All keys should be used with `-D`: <br/>

| key | telegram | slack | email | mattermost | description |
:----:|:--------:|:-----:|:-----:|:----------:|:------------:
messenger            | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | telegram (default), slack, email, mattermost
bot.token            | :heavy_check_mark: | :heavy_check_mark: | :x:                | :heavy_check_mark: | Bot/app secret token
chat.id              | :heavy_check_mark: | :heavy_check_mark: | :x:                | :heavy_check_mark: | Chat/channel id
reply.to.message.id  | :heavy_check_mark: | // todo            | :x:                | :heavy_check_mark: | Message id for reply
mail.host            | :x:                | :x:                | :heavy_check_mark: | :x:                | Smtp server
mail.port            | :x:                | :x:                | :heavy_check_mark: | :x:                | Smtp port
mail.username        | :x:                | :x:                | :heavy_check_mark: | :x:                | From email username
mail.password        | :x:                | :x:                | :heavy_check_mark: | :x:                | From email password
mail.to              | :x:                | :x:                | :heavy_check_mark: | :x:                | To email list - a@a.a, b@b.b
mattermost.api.url   | :x:                | :x:                | :x:                | :heavy_check_mark: | Mattermost api url
project.name         | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | Project name
build.launch.name    | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | Build launch name
build.env            | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | Build environment
build.report.link    | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | Build report link
lang                 | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | Supported languages: en, fr, ru, ua
enable.chart         | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | Enable/disable PieChart diagram (false by default)
allure.report.folder | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | Set allure report folder

```
java  \
"-Dmessenger=${MESSENGER}" \
"-Dchat.id=${CHAT}" \
"-Dbot.token=${SECRET}" \
"-Dmail.host=${SMTP_SERVER}" \
"-Dmail.port=${SMTP_PORT}" \
"-Dmail.username=${EMAIL_USER}" \
"-Dmail.password=${EMAIL_PASSWORD}" \
"-Dmail.to=${EMAIL}" \
"-Dmattermost.api.url=${MATTERMOST_API_URL}" \
"-Dproject.name=${JOB_BASE_NAME}" \
"-Dbuild.launch.name=${SOME_LAUNCH_NAME}" \
"-Dbuild.env=${ENVIRONMENT}" \
"-Dbuild.report.link=${BUILD_URL}" \
"-Dlang=${LANGUAGE}" \
"-Denable.chart=${CHART}" \
"-Dallure.report.folder=./allure-report/" \
-jar allure-notifications-2.2.1.jar
```
