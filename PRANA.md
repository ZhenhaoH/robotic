# robotic with the RAI LGP Python extension

This public fork preserves the history of
[MarcToussaint/robotic](https://github.com/MarcToussaint/robotic), based on
`61647f20466786ebd7eca8c67b91e0939185d104`. The upstream MIT license and copyright
remain in `LICENSE`.

The `rai` submodule pins [ZhenhaoH/rai](https://github.com/ZhenhaoH/rai), including
the RobotPolicy LGP Python extension (`ROBOT_POLICY_LGP_API == 1`). The other four
submodules retain their upstream gitlinks and use absolute MarcToussaint URLs.
The committed URL and gitlink select the extension during normal recursive
submodule initialization; no local checkout override or patch application is needed.

The extension lives on `zhhuang/feat/robot-policy-public`; the upstream `master`
branch is retained. Use `origin` for ZhenhaoH/robotic and a read-only `upstream`
remote for MarcToussaint/robotic. After changing RAI, advance its gitlink here and then pin
both fork commits in the consuming project's source manifest.
Initialize submodules at their recorded commits; do not use `update --remote`.
Native build products and Python environments stay outside Git.

The initial integration has not been compiled or tested. GitHub Actions is
disabled to prevent imported build and documentation workflows from running
before runtime validation is authorized.
