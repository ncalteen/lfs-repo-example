# Git LFS Example

This repository is used to demonstrate configuring Git LFS on GitHub.

For instructions, see
[About large files on GitHub](https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-large-files-on-github).

## Git LFS Commands

| Command           | Description                                                                      |
| ----------------- | -------------------------------------------------------------------------------- |
| git lfs checkout  | Populate working copy with real content from Git LFS files                       |
| git lfs dedup     | De-duplicate Git LFS files                                                       |
| git lfs env       | Display the Git LFS environment                                                  |
| git lfs ext       | Display Git LFS extension details                                                |
| git lfs fetch     | Download Git LFS files from a remote                                             |
| git lfs fsck      | Check Git LFS files for consistency                                              |
| git lfs install   | Install Git LFS configuration                                                    |
| git lfs lock      | Set a file as "locked" on the Git LFS server                                     |
| git lfs locks     | List currently "locked" files from the Git LFS server                            |
| git lfs logs      | Show errors from the Git LFS command                                             |
| git lfs ls-files  | Show information about Git LFS files in the index and working tree               |
| git lfs migrate   | Migrate history to or from Git LFS                                               |
| git lfs prune     | Delete old Git LFS files from local storage                                      |
| git lfs pull      | Fetch Git LFS changes from the remote & checkout any required working tree files |
| git lfs push      | Push queued large files to the Git LFS endpoint                                  |
| git lfs status    | Show the status of Git LFS files in the working tree                             |
| git lfs track     | View or add Git LFS paths to Git attributes                                      |
| git lfs uninstall | Uninstall Git LFS by removing hooks and smudge/clean filter configuration        |
| git lfs unlock    | Remove "locked" setting for a file on the Git LFS server                         |
| git lfs untrack   | Remove Git LFS paths from Git attributes                                         |
| git lfs update    | Update Git hooks for the current Git repository                                  |

## Examples

To get started with Git LFS, the following commands can be used.

- Setup Git LFS on your system. You only have to do this once per user account:

  ```bash
  git lfs install
  ```

- Choose the type of files you want to track, for examples all ISO images, with
  git lfs track:

  ```bash
  git lfs track "*.iso"
  ```

  The above stores this information in the `.gitattributes` file, so that file
  needs to be added to the repository.
