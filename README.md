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
repo-name master* origin[up to date]
another-repo feature origin[ahead 1, behind 2] upstream[branch not present]
```

- A `*` next to the branch name denotes pending changes.
- The synchronization status details how the local branch compares to its remote counterparts.

## Requirements

- Bash
- Git

## Contributing

Feel free to fork this repository and submit pull requests to enhance the script's functionality.

## License

This project is licensed under the [MIT License](LICENSE).
