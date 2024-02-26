# git-overview

A Bash script (`git-overview`) for recursively scanning directories to find Git repositories and providing a detailed overview of their state. It highlights the current branch, pending changes, and remote synchronization status for each repository found.

## Features

- Recursively identifies Git repositories from the starting directory.
- Displays the current branch for each found repository.
- Indicates pending changes with a `*` symbol next to the branch name.
- Lists remote repositories and their synchronization status with the local branch.

## Usage

1. Clone this repository or download `git-overview` directly.
2. Make the script executable: `chmod +x git-overview`.
3. Execute the script in a directory to analyze Git repositories within: `./git-overview`.

## Output Format

The script outputs a neatly formatted table with columns for:

- Repository Name
- Current Branch (marked with `*` if there are pending changes)
- Remote Synchronization Status

### Example Output

```
project-alpha                 master   beta[ahead 126, behind 0] origin[up to date] production[ahead 2782, behind 0]
widget-factory-client         master   beta[ahead 840, behind 13] origin[up to date] production[ahead 815, behind 0]
cloud-gatekeeper              main*    origin[ahead 0, behind 1]
data-hub-api                  master*  origin[up to date]
enterprise-connector          master*  beta[ahead 4251, behind 90] origin[up to date] production[ahead 3450, behind 0]
devops-pipeline-tools         main     origin[ahead 0, behind 31]
backoffice-framework          beta     beta[branch not present] origin[up to date] production[branch not present]
marketing-dashboard-client    master   beta[ahead 136, behind 0] origin[ahead 0, behind 6]
analytics-backend-service     master   origin[up to date]
utility-library               main*    origin[up to date]
customer-engagement-platform  master   beta[ahead 7, behind 0] origin[up to date]
infrastructure-as-code        main     origin[ahead 0, behind 39]

```

- A `*` next to the branch name denotes pending changes.
- The synchronization status details how the local branch compares to its remote counterparts.

## Requirements

- Bash/Zsh
- Git

## Contributing

Feel free to fork this repository and submit pull requests to enhance the script's functionality.

## License

This project is licensed under the [MIT License](LICENSE).
