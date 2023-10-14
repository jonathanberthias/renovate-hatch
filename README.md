# renovate-hatch

Minimal reproduction repository for https://github.com/renovatebot/renovate/discussions/24956 to enable updates to hatch environments' dependencies.

There is a minimal [`pyproject.toml`](https://github.com/jonathanberthias/renovate-hatch/blob/main/pyproject.toml) file created with `hatch new --init`, to which I removed the unrelated sections.

It contains a standard PEP621 dependency `requests` which is outdated, as well as 2 hatch environments, each with their own set of outdated dependencies, using various specifiers.

In the [onboarding PR](https://github.com/jonathanberthias/renovate-hatch/pull/1), only `requests` is detected.
