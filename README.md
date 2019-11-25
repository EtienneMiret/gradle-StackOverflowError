This is a [MCVE][1] to demonstrate [gradle/gradle#11466][2].

In order to reproduce this StackOverflowError:

 1. Check-out this project.
 2. Make sure your `~/.gradle/gradle.properties` DO NOT contain any
    gradle publish secret
    (you don’t want to publish this dummy plugin by accident)
    (you just need to comment out the line with your secret if you have one).
 3. Run ./gradlew publishPlugins.

[1]: https://meta.stackoverflow.com/questions/366988/what-does-mcve-mean
[2]: https://github.com/gradle/gradle/issues/11466
