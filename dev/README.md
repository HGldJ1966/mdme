MdMe Developer Notes
=====================

This document contains notes that may be useful to the developers of
MdMe.


Release Checklist
-----------------

Perform the following tasks for every release:

  - Update version in README.md.
  - Update version in package.json.
  - Update version in Makefile.
  - Update copyright notice in LICENSE.md.
  - Update copyright notice in mdme.js.
  - Update CHANGES.md.
  - Update minified script.

        npm run min

  - Commit changes.

        git status
        git add .
        git commit

  - Tag the release.

        git tag <VERSION> -m "MdMe <VERSION>"
        git push
        git push origin <VERSION>

  - Publish package.

        npm login
        npm publish

  - Publish documentation and examples.

        make pushdocs
