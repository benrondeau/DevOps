# DevOps
Personal DevOps Notes for Ideal Process


### Raw Notes
- Code management with Git (duh)
- Issue tracking
- PRs
- Release/build tagging with changelog ([example](https://github.com/angular/angular/blob/master/CHANGELOG.md)), [Semver](http://semver.org/) for versioning.
- Continuous integration
- Templates for issues, PRs
- Follows applicable principles of [Joel test](https://myers.io/2017/04/04/the-joel-test-for-2017/)
- Follows [12 Factor App](https://12factor.net/) principles
- Single build script for everything
- Project management (Zenhub or the like)
- Proper API documentation, like [Swagger](http://swagger.io/)
- Code documentation (lots of source code, not text) in README, Wiki or with a tool like [GitBook](https://www.gitbook.com/)
- Document process for all this, not just how individual steps/components work
- Create style guide for app, even if just super basic.
- Accessibility standards, even if just basic.
- Proper licensing of assets (code, images, etc.)
- Use [GitFlow branching model](http://nvie.com/posts/a-successful-git-branching-model/)
- DON'T GO CRAZY GOING FOR PERFECTION ON EVERY FRONT. EVEN THE WORLD'S BEST APPS HAVE ISSUES (Facebook's mobile website is an example [Page can't load, try again error])

### Tracking/Analytics
- Add analytics to project (like GA)
- Add frontend bug tracking (ex. Sentry), analytics (ex. GA) and performance tracking (ex. New Relic Browser)
- Add server side bug tracking (ex. Sentry), logging (ex. Papertrail), performance tracking (New Relic)

### Code
- Linting of styles, scripts
- Validated using these tools (https://w3c.github.io/developers/tools/)
- Testing, both automated and manual (each PR should list any manual QA testing steps)
- Simplicity of complexity
- Progressive Web Apps
- Cross browser testing for scripts
- Testing on real devices
- Build script for dev, testing, production (deploy)
- Build it right the first time, don't be lazy.
- Checklist like http://a11yproject.com/checklist.html?
- Create spec for what will be supported and not (browsers, devices, accessibility, etc.)



### Front End Process
1. Create branch for issue from `master`
2. Setup dev environment 
- Launch VM's, open actual device browsers to URL
3. Write code
4. Add tests as I go
5. Refer to PR checklist to ensure everything is being done correctly
6. Create PR

### Testing
- Code styles (CSS & JS)
- Automated
- Security testing (basic testing to ensure obvious things are covered)
- Add frontend bug tracking (Sentry), backend tracking (New Relic)
- Lighthouse score
- Chrome lens (accesibility)

### Security
- HTTPS on server, all connections in apps use it
- Plan for handling security breach?
- Service for tracking vulnerabilities in dependencies (like Synk)
- Directions for users how to submit security issues (same as issues?)

### Problems
- Plans for restores and rollbacks on backend components (db's, etc.)
- Back everything up (databases, etc.)
- Way to be alerted if there is a critical problem

# Distilled Notes

### Initial Planning
- Create standards for project, including:
  - [ ] Design standards
  - [ ] Code standards

### Code Creation
1. Issue created
2. Issue triaged
3. Branch created from `develop` with issue # in the branch name (ex. `132-description-of-branch`)
4. Work done according to standards above
5. When code complete, PR created for `staging` branch (if exists) or `master`
6. Code review and manual testing by another dev (staging or their local machine), automated testing done by CI 
7. If everything passes muster, PR merged
8. Automated build occurs on merge, pushed to prod server
9. QA testing on prod.
10. Issue closed
11. Create release, if necessary based on change.

### Ongoing Maintenance
TBD


