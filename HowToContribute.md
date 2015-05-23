# Start #

To get you a little overview over the internal flows of the library I started with an Architecture description. Please give me feedback about it!
To start coding, follow the steps in IDESetup.

# Contribute #

Every contribution is always welcome. To help me keep the library clean and maintainable please try to follow these rules:

  * Send me patches to the latest version in GIT. See https://www.kernel.org/pub/software/scm/git/docs/git-diff.html command for an example
  * Every supported device / eep should have an Unit Test that tests its parsing functionality. See SingleInputContactTest as an example. For each number there should be method with the two boundaries (min, max) and one in between. The TemperaturSensorTest can be used as an example. The supporting methods for the tests are still being improved, my goal is it to make it as easy as possible to write an unit test.
  * If possible send me the descriptions for the wiki as well (examples are coming soon)