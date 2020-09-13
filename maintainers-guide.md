# Notes for maintainers

## Reviewing guideline

-   Reject pull requests to add bad features
-   Don't merge commits including bugs
-   Don't request too much about coding styles
    -   Use linters if you want to forbid something.
    -   It's often faster to fix code yourself. Educational comments are important, but you should not leave too many.
-   Be tolerant for beginners


## Checklist to review pull requests

-   [ ] UX: The behavior is appropriate.
    -   [ ] It has benefits for users.
    -   [ ] It is consistent with the responsibility of the project.
-   [ ] Architecture: The design of code is acceptable.
    -   [ ] It is reasonably maintainable.
-   [ ] Implementation: The code is properly written.
    -   [ ] It passes CI.
    -   [ ] It has tests.
    -   [ ] It is enough readable.


## Labels in issues

-   `priority:high`: The issue affects many users and is important. It should be fixed at most in a month.
-   `priority:medium`: otherwise
-   `priority:low`: The issue affects only few users and is ignorable.
-   `difficulty:high`: It's impossible to assign others because the issue is too difficult. If you feel that the issue is tedious and you don't want to do it, use this.
-   `difficulty:medium`: otherwise
-   `difficulty:low`: It's trivial. If you feel that the issue enough easy and you want to assign it to anyone, use this. 


## How to bump the version

1.  Update the version number in `setup.py` (or in a file like `__about__.py`)
    -   Use [Semantic Versioning](https://semver.org/)
1.  Update the `CHANGELOG.md` if it exists
    -   Read the [keep a changelog](https://keepachangelog.com/) page
1.  Create a [GitHub Release](https://help.github.com/en/github/administering-a-repository/managing-releases-in-a-repository)
    -   Use tag names like `v1.2.3`
    -   Describe what are changed in the Description field. You can copy and paste this from `CHANGELOG.md`.
    -   This kicks a GitHub Action to upload the package to [PyPI](https://pypi.org/)


## Contacts

Currently [@kmyk](https://github.com/kmyk) is the main maitainer of this organization.
Some repositories have additional maintainers.

Also, as a backup, [@yosupo06](https://github.com/yosupo06) has the admin permission of this organization. If [@kmyk](https://github.com/kmyk) is gone, please contact to [@yosupo06](https://github.com/yosupo06).
