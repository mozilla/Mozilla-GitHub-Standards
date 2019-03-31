# Mozilla Code of Conduct support

The scripts in this repository help repositories to be in compliance
with the [Mozilla GitHub Standards][mgs].

## check_CoC.py

This script checks repositories for compliance with the [Code of
Conduct][coc](CoC) requirement. It does the following, from an account
that should be dedicated to this purpose.

The process is:
- check a repository for a file of the correct name and contents,
- open an issue if it is missing or incorrect
- if the CoC is missing:
    - fork the repository (using the hash of the full name as the fork
      name - to avoid name space collisions)
    - commit the CoC file to the fork
    - create a pull request back to the source for the addition, linked
      to the issue.

The script can be rerun -- it will not create additional issues or PRs.


[mgs]: https://wiki.mozilla.org/GitHub/Repository_Requirements
[coc]: https://wiki.mozilla.org/GitHub/Repository_Requirements#Code_Of_Conduct
