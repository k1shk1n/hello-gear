# hello-gear
This Gears contains `.gitlab-ci.yml` that outputs a greeting.

This Gear is an example of git-system-follower Gear 
which uses default package api for `init.py`, `delete.py`.

## Extra parameters

| Name   | Description                                         | Default  | Example             |
|--------|-----------------------------------------------------|----------|---------------------|
| `name` | The name of the person being greeted                | `World`  | `Vladislav`, `Ivan` |
| `tags` | Runner tags on which to run the `.gitlab-ci.yml` on | `defalt` | `docker`, `linux`   |

## Using
1. Configure your repository: [git-system-follower: Complete repository prerequisites](https://github.com/Netcracker/qubership-git-system-follower/blob/main/docs/getting_started/quickstart.md#complete-repository-prerequisites)
2. Export the `GSF_GIT_TOKEN` variable
    ```bash
    export GSF_GIT_TOKEN=<your access token>
    ```
3. Run installation Hello-World Gear using git-system-follower
    ```bash
    gsf install --repo <your repository> \
                --branch <your branch> \
                --extra name <your name> no-masked \
                --extra tags <your tags> no-masked \
                <TBD Gear after release>
    ```
