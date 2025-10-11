# Contributing to MapLibre

Hi, and thanks in advance for contributing to MapLibre. Here's how we work. Please follow these conventions when submitting an issue or pull request.

> [!IMPORTANT]
> **Do not violate Mapbox copyright!**
>
> In December 2020 Mapbox decided to publish future versions of mapbox-gl-js under a proprietary license.
> **You are not allowed to backport code from Mapbox projects which has been contributed under this new license**.
> Unauthorized backports are the biggest threat to the MapLibre project.
> If you are unsure about this issue, [please ask](https://github.com/maplibre/maplibre-gl-js/discussions)!

## Best Practices for Contributions

MapLibre welcomes contributions from community! This codebase is large and complex, and following these best practices will assist the maintainer team in reviewing your contribution. In general, the project values discussion and communication over process and documentation. However, due to the size and complexity of the code, below are some best practices that have aided contributors.

It is a good idea to discuss proposed changes before proceeding to an issue ticket or PR. The project team is active in the following forums:

* For informal chat discussions, visit the project's [Slack Channel](https://osmus.slack.com/archives/C01G3D28DAB).
* For discussions whose output and outcomes should not be ephemeral, consider starting a thread on [GitHub Discussions](https://github.com/maplibre/maplibre-gl-js/discussions). This makes it easier to find and reference the discussion in the future.

MapLibre software relies heavily on automated testing, and the project includes a suite of unit and integration tests. For both new features and bugfixes, contributions should update or add test cases to prevent regressions.

### New Features

For new features, it is usually a good idea to start with an issue ticket. If the feature requires changes to the style specification, an issue ticket should be created in the [style specification GitHub repository](https://github.com/maplibre/maplibre-gl-style-spec). Style specification changes are hard to change later, so there will be particularly close scrutiny on changes to the specification.

If possible, it is beneficial to demonstrate proposed new features and assess the performance implications of the proposed change. You can use `npm install <location-of-maplibre-source-code>` to test changes in an npm context, or `npm run build-prod` to build a .js package for this purpose.

For more complex proposed features that require deeper discussion, you should consider bringing it up in the [Technical Steering Committee](https://maplibre.org/categories/steering-committee/) meeting for a video discussion with the team about the proposed change. We find that sometimes it's easier to have a focused, face-to-face discussion for more consequential decisions.

The Technical Steering Committee meetings are open to anyone who wants to get involved in the technical direction of the project. These meetings offer a chance for discussion and collaboration on various technical topics. We welcome you to join the meetings if you're interested in getting involved.

### Bug Fixes

If you've identified a significant bug, or one that you don't intend to fix yourself, please write up an issue ticket describing the problem. For minor or straightforward bug fixes, feel free to proceed directly to a PR.

Some best practices for PRs for bugfixes are as follows:

1. Begin by writing a failing test which demonstrates how the current software fails to operate as expected. Commit and push the branch.
2. Create a draft PR which documents the incorrect behavior. This will show the failing test you've just written in the project's continuous integration and demonstrates the existence of the bug.
3. Fix the bug, and update the PR with any other notes needed to describe the change in the PR's description.
4. Don't forget to mark the PR as ready for review when you're satisfied with the code changes.

This is not intended to be a strict process but rather a guideline that will build confidence that your PR is addressing the problem.
