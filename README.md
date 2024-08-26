![GSOCImage](https://github.com/user-attachments/assets/9aff2d4f-8f93-43cf-85d4-4d133a578866)

# GSoC'24 - Final Project Report

This report covers the work done in Google Summer of Code 2024. It includes results, possible improvements, and future plans. It's also the final project report with all contributions listed.

## Basic Info

- Name: Alok Gupta
- Email: alokgupta1560@gmail.com
- University: Indian Institute of Information Techonolgy Ranchi
- GSoC Organisation: [JSON Schema Org](https://github.com/json-schema-org)
- Project: Setting up the CI/CD Pipeline and Testing for the JSON Schema website
- Project Link: https://github.com/json-schema-org/community/issues/603
- Proposal Link: https://drive.google.com/file/d/1Hu7i1_twl9awkcXK_fac0YzqehNgYqGG/view?usp=sharing

## Background

My journey into open source began just a year ago, with my first contribution being a simple change to update the Twitter logo to X. That small step marked the beginning of an incredible adventure.
What I've come to appreciate most about open source is that it's not just about writing code. It's about how you write code, how you collaborate with others, how you help and learn from your peers, and ultimately, how you contribute to making the world a better place.

Open source has taught me invaluable lessons, from improving my coding skills to collaborating on projects that impact millions, if not billions, of people. Through this community, I've met amazing individuals from around the world, forming friendships and finding mentors who have been instrumental in guiding my journey.
At the end, I just want to say once you immerse yourself in the world of open source, there's no turning back. It becomes an addiction—one that you'll grow to love and cherish.

## Project: CI/CD Pipeline and Testing for JSON Schema Website


<p align="center" style="background-color: #ffffff;">
  <img src="https://github.com/user-attachments/assets/0c2f2382-8881-434a-a2f5-8ad2f5f9e03d" alt="Brandmark-Blue" width="250" style="padding: 10px 0px; background: white;">
</p>

The JSON Schema project, hosted on GitHub under the organization "json-schema-org", consists of multiple repositories for the specification and supporting resources. While the JSON Schema specification itself is published through the Internet Engineering Task Force (IETF) as a series of "personal drafts", our focus is on improving the development and deployment process for the JSON Schema website.

### Project Goals:

1. Enhance the existing CI/CD pipeline for the JSON Schema website using GitHub Actions to incorporate:
   - Linting
   - Code formatting
   - Broken link checking
   - Unit testing
   - Build processes
   - UI testing

2. Develop and integrate a foundational set of UI tests into the workflow, with the intention of expanding these tests over time.

4. Review and optimize existing GitHub workflows to balance CI/CD processes with community operations (Community Ops).

This project aims to improve code quality, ensure consistency, and facilitate secure feature additions to the JSON Schema website. By strengthening the CI/CD pipeline and introducing robust testing practices, we'll create a more reliable and maintainable development process for the JSON Schema community.

<!-- ## Current Status of Project:
We are done with all the project Goals and go beyond the scope of project in some cases.
1. Setup Robust CI/CD pipeline consist of code quality checks like formatting, linting, typecheck etc, build, test, deployment, community operations etc.
2. Setup cypress testing libraries, and added Component Tests -->


## Goals Achieved:

### CI/CD Pipeline

- **CI/CD Workflows for the JSON Schema Website**
  - [x] Setup linting, formatting, broken link checks, unit tests, build processes, UI tests, stale issue and PR detection, and unauthorized file detection.
  - [x] Migrated Cloudflare native deployment to GitHub Actions manual deployment workflow due to limitations with preview deployments from forked repositories.

- **JSON Schema Bot**
  - [x] Created the JSON Schema Bot for community operations and integrated its token into workflows.

### Testing

- **Unit and UI Testing**
  - [x] Configured Cypress for local test environment setup.
  - [x] Added Codecov for code coverage reporting and PR notifications.
  - [x] Implemented GitHub Actions workflow for running Cypress tests.
  - [x] Added component testing for the website.

### Community Operations

- **Community Operations and GitHub Workflows**
  - [x] Developed workflows for preview deployments from forked repositories and deployment to Cloudflare Pages.
  - [x] Created workflows for fetching contributor and project roadmap data.
  - [x] Implemented workflows for detecting unauthorized file changes.
  - [x] Added workflows for notifying failed actions and reminding office hours.

### Miscellaneous

- **Additional Contributions**
  - [x] Introduced GitVote for automated voting processes.
  - [x] Added stale issues and PR workflows for the community and landscape repositories.

<!-- - [ ] Setup Various CI/CD workflows for the JSON Schema website.
- [ ] Setup Linting, Formatting, Broken links check, Unit Test, Build, UI Test.
- [ ] Define and Implement the Unit Testing and UI Testing.
- [ ] Review and consolidate the existing GitHub workflows approach what will be a mix of CI/CD and Community Ops. -->

## Contributions


### Pull Request Summary

| PR Number | Title | URL | Status | Tag |
|-----------|-------|-----|--------|-----|
| **Website PRs** | | | | |
| 870 | testing(component-testing) : Add component test | [Link](https://github.com/json-schema-org/website/pull/870) | Merged | Feature |
| 869 | chore(github-actions): update contributor and project sync workflows | [Link](https://github.com/json-schema-org/website/pull/869) | ✅Merged | Chore |
| 842 | chore(yarn) : migrated yarn to modern yarn berry | [Link](https://github.com/json-schema-org/website/pull/842) | ✅Merged | Enhancement |
| 837 | Fix algolia search and removed duplicate dependencies | [Link](https://github.com/json-schema-org/website/pull/837) | ✅Merged | Bug Fix |
| 829 | Set up Cypress and configure local test environment | [Link](https://github.com/json-schema-org/website/pull/829) | ✅Merged | Feature |
| 797 | chore(documentation) : updated docs for setting up environment variables | [Link](https://github.com/json-schema-org/website/pull/797) | ✅Merged | Chore |
| 789 | Chore(github-actions) : add CI/CD workflows guidelines and improve naming conventions | [Link](https://github.com/json-schema-org/website/pull/789) | ✅Merged | Chore |
| 785 | Feat: Add workflow to get preview from fork repository and deploy to cf pages | [Link](https://github.com/json-schema-org/website/pull/785) | ✅Merged | Feature |
| 781 | Feat: Added two workflows for fetching contributor and project roadmap data | [Link](https://github.com/json-schema-org/website/pull/781) | ✅Merged | Feature |
| 750 | chore(link.yml) : using github-app authentication and fixes failing link.yml workflow | [Link](https://github.com/json-schema-org/website/pull/750) | ✅Merged | Chore |
| 748 | chore(unauthorized-file) : updated unauthorised file detection jobs | [Link](https://github.com/json-schema-org/website/pull/748) | ✅Merged | Chore |
| 713 | Fixes: failing workflow pull-request-target-yml | [Link](https://github.com/json-schema-org/website/pull/713) | ✅Merged | Bug Fix |
| 696 | Feat : Added job to detect changes in unauthorized files | [Link](https://github.com/json-schema-org/website/pull/696) | ✅Merged | Feature |
| 695 | Enhancement : Merge both greet-on-first-pr and merge in pull-request-target-yml | [Link](https://github.com/json-schema-org/website/pull/695) | ✅Merged | Enhancement |
| 693 | Feature: Added Issue-yml | [Link](https://github.com/json-schema-org/website/pull/693) | ✅Merged | Feature |
| 690 | Feature : github-actions - Setup stale Issues and PRs workflow | [Link](https://github.com/json-schema-org/website/pull/690) | ✅Merged | Feature |
| **Miscellaneous PRs** | | | | |
| 772 | chore(github-actions) : Fixes notify-failed-actions workflow | [Link](https://github.com/json-schema-org/community/pull/772) | ✅Merged | Chore |
| 771 | chore(github-actions) : Fixes slack-ocwm-reminder.yml with office hour time and timezone. | [Link](https://github.com/json-schema-org/community/pull/771) | ✅Merged | Chore |
| 9 | Add gitvote for automated voting process | [Link](https://github.com/json-schema-org/TSC/pull/9) | ✅Merged | Feature |
| 738 | Feat : added stale issues and PR workflow | [Link](https://github.com/json-schema-org/community/pull/738) | ✅Merged | Feature |
| 60 | Feat : added stale issue and PR workflow | [Link](https://github.com/json-schema-org/landscape/pull/60) | ✅Merged | Feature |

### Issues Summary
 All the issues related to the GSoC project are listed [here](https://github.com/json-schema-org/website/issues?q=is%3Aissue+author%3Aaialok+is%3Aclosed)

### Code Under Review

Code under review can be found [here](https://github.com/json-schema-org/website/pulls?q=is%3Aopen+is%3Apr+label%3AGSoC+author%3Aaialok)

 ### Problems Faced


- **Cypress Code Coverage Setup:** This is one of the interesting challenges I faced during the project. Setting up Cypress was easy, but the code coverage part took a good amount of time. The problem was that Cypress code coverage uses the Babel compiler for JS/TS, while Next.js uses the SWC compiler. When configuring Cypress code coverage with Istanbul (a tool for code coverage reporting), we needed to set up `.babelrc` files. Because of the `.babelrc` file, Next.js started using the Babel compiler instead of the SWC compiler, causing most of the Next.js parts to fail because they are compatible with the SWC compiler. After spending more than a day and going through 100+ tabs of blogs, GitHub issues, discussions, and the Cypress Discord, I could not find a good solution. This problem still exists.

  After lots of struggle, I found a little hacky solution. Basically, I found docs on babel documentation that if you use Babel in `package.json`, then Next.js will not be able to find the Babel config and will use the SWC compiler. And it worked!
  https://babeljs.io/docs/configuration#packagejson


 - **Cloudflare Pages Deployment:** The Cloudflare Pages Does not support the preview deployment from the forked repository. So, I have to create a manual deployment workflow for the preview deployment from the forked repository.


## Current Status of Project

During the GSoC period, I've successfully improved the JSON Schema website project by setting up a good CI/CD pipeline, implementing Cypress for UI testing, and adding component tests. I've also enhanced community operations and GitHub workflows, integrated GitVote for automated voting processes, and added workflows to manage stale issues and pull requests in both the community and landscape repositories. With all project goals now achieved, we've moved into the maintenance phase. I'll remain available to provide any necessary help or support to ensure these new systems and processes continue to run smoothly, thereby strengthening the JSON Schema website's development workflow, testing procedures, and community engagement for the future.

## Future Work

Since the project goals have been achieved, the focus now shifts to maintaining and improving the existing systems. Here are some areas for future work:

- The project goal is to setup minimal testing for the JSON Schema website. We can expand the test coverage by adding more component and E2E tests.
- We can add more GitHub workflows for automating community operations and enhancing the development process.

## My Learnings

Participating in GSoC has been rewarding both technically and non-technically. Here are the key lessons from my journey:

- Gained experience working with a large codebase and collaborating with a diverse team of developers.
- Learned how to set up CI/CD pipelines, write unit tests, and implement components tests.
- Improved communication skills with the community and learned to manage project requirements.
- Enhanced time management and task prioritization to meet deadlines.
- Developed skills in code review, documentation, and contributing to open-source projects.

## Note of Thanks

I would like to express my sincere gratitude to my mentor [Benjamin Granados](https://github.com/benjagm)  for his guidance, support, and encouragement throughout the GSoC program. His expertise, patience, and mentorship have been invaluable to me, and I am grateful for the opportunity to work with him on this project. I would also like to thank the JSON Schema community for their feedback, support, and collaboration during the GSoC program. Lastly, I would like to thank the GSoC program organizers for providing me with this opportunity to learn, grow, and contribute to open source projects. I am grateful for the experience and look forward to continuing my journey in the open source community.


