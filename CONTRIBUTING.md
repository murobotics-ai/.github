# Contributing to Mu Robotics

Thanks for helping make robot-learning data collection more accessible and reproducible. Mu Robotics welcomes focused contributions across hardware, capture software, documentation, validation, and new robot embodiments.

## Choose the right repository

- [`handumi-hw`](https://github.com/murobotics-ai/handumi-hw) — CAD, printable parts, electronics, the bill of materials, assembly, and gripper-tip designs.
- [`handumi-quest-app`](https://github.com/murobotics-ai/handumi-quest-app) — Meta Quest tracking compatibility and its Unity implementation.
- [`.github`](https://github.com/murobotics-ai/.github) — the organization profile and shared community files.

The main HandUMI capture software is still being prepared for public release. Until its repository is public, use `handumi-hw` for interface-wide questions and proposals.

For substantial changes, open an issue before investing significant time. Describe the problem, the proposed direction, and any hardware or dataset assumptions. This lets maintainers confirm scope and point you to relevant work.

## Development workflow

1. Fork the relevant repository and create a focused branch.
2. Read that repository's README and local contribution or test instructions.
3. Keep the change small enough to review and avoid unrelated formatting or generated-file churn.
4. Add or update tests and documentation when behavior changes.
5. Open a pull request with the motivation, implementation, validation evidence, and any hardware limitations.

## Hardware contributions

For a new or revised physical part, include:

- editable source files as well as export formats;
- the target printer, material, tolerances, and hardware revision;
- clear photos or renders of the assembled result;
- a bill-of-materials change when parts or costs differ;
- fit and motion-range notes, especially for a new gripper tip;
- enough measurements and test evidence for another person to reproduce the result.

Safety matters. Call out pinch points, sharp edges, electrical risks, heat, and any failure mode that could damage an operator, sensor, or robot.

## Software contributions

Follow the repository's documented setup and test commands. In the pull request, list the exact checks you ran. Changes that affect capture timing, transforms, calibration, schema, or quality gates should include regression tests and a short explanation of their effect on existing recordings.

Never commit credentials, private datasets, participant information, machine-local configuration, or large generated artifacts. Use synthetic or explicitly shareable samples in tests and documentation.

## Issues and pull requests

A strong issue is reproducible and specific: name the repository and revision, environment or hardware, expected behavior, actual behavior, minimal reproduction, and relevant logs. Remove personal data and secrets before attaching diagnostics.

A strong pull request explains why the change is needed, keeps one logical purpose, links its issue when applicable, and includes evidence that it works. Draft pull requests are welcome for early technical feedback.

By participating, you agree to keep collaboration technical, respectful, and constructive. Harassment, personal attacks, and discriminatory conduct are not welcome in Mu Robotics spaces.
