Contributing to OSRD
All contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome.

Check out our community's Code of Conduct and feel free to say hi on our #public-general:osrd.fr matrix channel if you'd like. It's a nice place to chat about OSRD development, ask questions, and get to know the other contributors and users in a less formal setting.

OSRD is a complex project currently in development phase. If you want to contribute and feel lost on the best way to do so, we will be happy to help you: please get in touch through contact@osrd.fr, via Matrix or ask a question on GitHub Discussions. You can also check out the currently open good first issues.

Getting oriented
The OSRD project has 2 primary repos:

osrd: This is where the simulator is developed.
osrd-website: Where the official website, blog, documentation, ... are hosted.
The osrd repo itself contains many smaller packages.

Some packages of interest (more details in packages' README.md):

core: The core engine of the simulation where physics, pathfinding and conflict detection are computed.
editoast: Service to retrieve data from the databases and make data available through http endpoints. It is also the place where edition of the infrastructure is computed.
front: GUI of OSRD.
tests: Package to run integration tests on services.
python/osrd_schemas: Definition of the railjson format.
What we are trying to build
OSRD is an open source web application for railway infrastructure design, capacity analysis, timetabling and simulation. Check out details on the website specific page.

OSRD also currently has the following "development process" goals:

Don't merge everything ... don't merge too early: Every feature we add increases maintenance burden and compile times. Only merge features that are "generally" useful. Don't merge major changes or new features unless we have relative consensus that the design is correct and that we have the developer capacity to support it.

Thoughtful public interfaces over maximal configurability: Symbols and apis should be private by default. Every public API should be thoughtfully and consistently designed. Don't expose unnecessary internal implementation details. Don't allow users to "shoot themselves in the foot". Favor one "happy path" api over multiple apis for different use cases.

Welcome new contributors: Invest in new contributors. Help them fill knowledge and skill gaps.

Civil discourse: We need to collectively discuss ideas and the best ideas should win. But conversations need to remain respectful at all times. Remember that we're all in this together. Always follow our Code of Conduct.

Test what you need to: Write useful tests. Don't write tests that aren't useful. We generally aren't strict about unit testing every line of code. We don't want you to waste your time. But at the same time:

Most new features should have at least one minimal integration test.
The more complex or "core" a feature is, the more strict we are about unit tests. Use your best judgement here. We will let you know if your pull request needs more tests.
The OSRD Team
The OSRD Team is the group of people responsible for stewarding the OSRD project. It handles things like merging pull requests, choosing project direction, managing bugs / issues / feature requests, running the OSRD website, controlling access to secrets, defining and enforcing best practices, etc.

Note that you do not need to be a member of the OSRD Team to contribute to OSRD. Community contributors (this means you) can freely open issues, submit pull requests, and review pull requests.

Click here to learn more about the project's governance.

Contribute code
To comply with the DCO, all commits must include a Signed-off-by line. You can find more information about this here

For more advice on how to contribute, follow that link: https://osrd.fr/en/docs/guides/contribute/contribute-code

Additional supported resources
In addition to obvious parts (CI, compile, tests, etc.), some resources are currently officially supported. These mostly aim at making the developer work easier on the project.

Official support
These should work for any commit.

kubernetes use (main deployment target)
documentation (.md files, OSRD website)
main software build and management tools for each component (uv, cargo, npm, gradle, ...)
./osrd-compose script (and the combinations of available flags)
all the .sh scripts of the repository (except pr-tests-compose.sh for now)
Nice-to-have tools
Any developer has a specific (customized) setup. Therefore, some tools are not officially supported, but efforts are mutualized by versioning resources into the repository.

