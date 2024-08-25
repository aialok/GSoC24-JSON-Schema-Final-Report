![GSOCImage](https://github.com/user-attachments/assets/9aff2d4f-8f93-43cf-85d4-4d133a578866)

# GSoC'24 - Final Project Report

This report covers the work done in Google Summer of Code 2024. It includes results, possible improvements, and future plans. It's also the final project report with all contributions listed.

## Basic Info

- Name: Alok Gupta
- Email: alokgupta1560@gmail.com
- Github: aialok
- LinkedIn: https://www.linkedin.com/in/aialok/
- Twitter: https://x.com/ai_alok
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

## About the Project

<p align="center" style="background-color: #ffffff;">
  <img src="https://github.com/user-attachments/assets/0c2f2382-8881-434a-a2f5-8ad2f5f9e03d" alt="Brandmark-Blue" width="250" style="padding: 10px 0px; background: white;">
</p>

JSON Schema the project is located on GitHub under the organization name "json-schema-org". It is comprised of several git repositories used to track changes and enable collaboration on the specification and supporting resources.

The JSON Schema specification is made up of technical specification documents currently published canonically through the Internet Engineering Task Force (IETF) as a series of "personal drafts". A "personal draft" is the category given to documents published on the IETF which are from an IETF working group.

A JSON Schema document is written in JSON itself. Being written in JSON means that it can be read by almost every programming language, making it an interoperable validation solution. It can also be written using other formats which translate to JSON, or using code that can serialize to JSON.

My project was to set up the CI/CD pipeline and testing for the JSON Schema website.

## Project Goals

Currently the JSON Schema website have a very basic CI/CD workflow but we aim to provide a consistent way to securely add new features by improving the CI/CD workflow. The Project aims to stabilise & setup the CI/CD pipeline for the JSON Schema website project.

The second stage of this project will be create a minimal implementation of UI testing to be validated as part of the workflow so we can continue improve the tests over time.

The project implies:

1. Improving the CI/CD workflow using github actions and other tools to add features such as:

  - Lint.
  - Formatting.
  - Broken links check.
  - Unit Test.
  - Build.
  - UI Test.

2. Define and Implement the Unit Testing and UI Testing.
3. Review and consolidate the existing GitHub workflows approach what will be a mix of CI/CD and Community Ops.


<!-- ## Current Status of Project:
We are done with all the project Goals and go beyond the scope of project in some cases.
1. Setup Robust CI/CD pipeline consist of code quality checks like formatting, linting, typecheck etc, build, test, deployment, community operations etc.
2. Setup cypress testing libraries, and added Component Tests -->

## Goals Achieved:
- [ ] Setup Various CI/CD workflows for the JSON Schema website.
- [ ] Setup Linting, Formatting, Broken links check, Unit Test, Build, UI Test.
- [ ] Define and Implement the Unit Testing and UI Testing.
- [ ] Review and consolidate the existing GitHub workflows approach what will be a mix of CI/CD and Community Ops.

## Contributions


### Pull Request Summary

| PR Number | Title | URL | Status | Tag |
|-----------|-------|-----|--------|-----|
| **Website PRs** | | | | |
| 870 | testing(component-testing) : Add component test | [Link](https://github.com/json-schema-org/website/pull/870) | ✅ Merged | Feature |
| 869 | chore(github-actions): update contributor and project sync workflows | [Link](https://github.com/json-schema-org/website/pull/869) | ✅ Merged | Chore |
| 842 | chore(yarn) : migrated yarn to modern yarn berry | [Link](https://github.com/json-schema-org/website/pull/842) | ✅ Merged | Enhancement |
| 837 | Fix algolia search and removed duplicate dependencies | [Link](https://github.com/json-schema-org/website/pull/837) | ✅ Merged | Bug Fix |
| 829 | Set up Cypress and configure local test environment | [Link](https://github.com/json-schema-org/website/pull/829) | ✅ Merged | Feature |
| 797 | chore(documentation) : updated docs for setting up environment variables | [Link](https://github.com/json-schema-org/website/pull/797) | ✅ Merged | Chore |
| 789 | Chore(github-actions) : add CI/CD workflows guidelines and improve naming conventions | [Link](https://github.com/json-schema-org/website/pull/789) | ✅ Merged | Chore |
| 785 | [ github-actions ] : Add workflow to get preview from fork repository and deploy to cf pages | [Link](https://github.com/json-schema-org/website/pull/785) | ✅ Merged | Chore |
| 781 | Added two workflows for fetching contributor and project roadmap data | [Link](https://github.com/json-schema-org/website/pull/781) | ✅ Merged | Chore |
| 750 | chore(link.yml) : using github-app authentication and fixes failing link.yml workflow | [Link](https://github.com/json-schema-org/website/pull/750) | ✅ Merged | Chore |
| 748 | chore(unauthorized-file) : updated unauthorised file detection jobs | [Link](https://github.com/json-schema-org/website/pull/748) | ✅ Merged | Chore |
| 713 | Fixes: failing workflow pull-request-target-yml | [Link](https://github.com/json-schema-org/website/pull/713) | ✅ Merged | Bug Fix |
| 696 | Feat : Added job to detect changes in unauthorized files | [Link](https://github.com/json-schema-org/website/pull/696) | ✅ Merged | Feature |
| 695 | Enhancement : Merge both greet-on-first-pr and merge in pull-request-target-yml | [Link](https://github.com/json-schema-org/website/pull/695) | ✅ Merged | Enhancement |
| 693 | Feature: Added Issue-yml | [Link](https://github.com/json-schema-org/website/pull/693) | ✅ Merged | Feature |
| 690 | Feature : github-actions - Setup stale Issues and PRs workflow | [Link](https://github.com/json-schema-org/website/pull/690) | ✅ Merged | Feature |
| **Miscellaneous PRs** | | | | |
| 772 | chore(github-actions) : Fixes notify-failed-actions workflow | [Link](https://github.com/json-schema-org/community/pull/772) | ✅ Merged | Chore |
| 771 | chore(github-actions) : Fixes slack-ocwm-reminder.yml with office hour time and timezone. | [Link](https://github.com/json-schema-org/community/pull/771) | ✅ Merged | Chore |
| 9 | Add gitvote for automated voting process | [Link](https://github.com/json-schema-org/TSC/pull/9) | ✅ Merged | Feature |
| 738 | Feat : added stale issues and PR workflow | [Link](https://github.com/json-schema-org/community/pull/738) | ✅ Merged | Feature |
| 60 | Feat : added stale issue and PR workflow | [Link](https://github.com/json-schema-org/landscape/pull/60) | ✅ Merged | Feature |
