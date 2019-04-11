# Technical challenge 1

Create web application which shows in real-time files and directories of some server-side directory (preferred either
temp or home directory) including real-time changes.
Server-side should-t keep directories in memory - need to iterate through root folder and send them to the web application
Server-side need to observe folder / files changes to send those changes as well.

Key language learning points: iterables (to convert tree to flat iterable),
reactivity (to convert structure changes to stream items and send through Websockets).
<br /><br />


**Prerequisites**
- Java 8
- Maven
- IntelliJ Community Edition
- Lombok
- Github
<br /><br />

**Key points**
- Application should use Spring Boot (with Websockets)
- The directory tree should be presented as iterable
- Application should be fully covered with unit and integration tests
- Whenever a new file or directory is added web page contents also should be updated (make use of ReactiveX to handle changes)
<br /><br />

**Check points**
- [Pre work](checkpoints/stepZero.md)
- [Step1](checkpoints/stepOne.md)
- [Step2](checkpoints/stepTwo.md)
- [Step3](checkpoints/stepThree.md)
- [Step4](checkpoints/stepFour.md)
<br /><br />

**Verification**
- Download application from Docker Hub
- Open application in two browsers
- Check if both provides list of files located in some server-side folder
- Invoke http://(docker-instance-address)/addFile?name=1/2/3.txt
- Check if both browsers are updated with just created file named 3.txt and located in 1/2 folder