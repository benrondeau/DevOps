# DevOps
Personal DevOps Notes for Ideal Process


### Raw Notes
- Code management with Git (duh)
- Issue tracking
- PRs
- Release/build tagging, [Semver](http://semver.org/) for versioning
- Continuous integration
- Templates for issues, PRs
- Joel test
- Single build script for everything
- Project management (Zenhub or the like)
- Proper API documentation, like [Swagger](http://swagger.io/)
- Code documentation (lots of source code, not text) in README, Wiki or with a tool like [GitBook](https://www.gitbook.com/)
- Document process for all this, not just how individual steps/components work
- Something about

#### Code
- Linting of styles, scripts
- Testing, both automated and manual (each PR should list any manual QA testing steps)
- Simplicity of complexity
- Progressive Web Apps
- Cross browser testing for scripts
- Testing on real devices
- Build script for dev, testing, production (deploy)
- Build it right the first time, don't be lazy.
- Checklist like http://a11yproject.com/checklist.html?

#### Testing
- Code styles (CSS & JS)
- Automated
- Security testing (basic testing to ensure obvious things are covered)

#### Process
1. Issue created
2. Issue triaged
3. Branch created from `master` with issue # in the branch name
4. Work done according to standards above
5. When code complete, PR created for `staging` branch (if exists) or `master`
6. Code review and manual testing by another dev (staging or their local machine), automated testing done by CI 
7. If everything passes muster, PR merged
8. Automated build occurs on merge, pushed to prod server
9. QA testing on prod.
10. Issue closed
11. Create release, if necessary based on change.



