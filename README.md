# Eunomia

TBD

## Getting Started

TBD

## Contributing

To contribute to this repository, you should:

- Sign the [Developer Certificate of Origin](https://developercertificate.org) (DCO) by adding a `Signed-off-by` line to your commit messages, which can automatically be done by passing a `-s` or `--signoff` option when commit your changes.
This certifies that you wrote or have the right to submit the code you are contributing to the project, do note that you might need to add a signing key on Github to have a `verified` status on your commit, detailed information will be listed below.
- Choose an issue to work on. Issues labeled `good first issue` are suitable for newcomers. You can also look for issues marked `help wanted`.
- Fork the eunomia repository and create a branch for your changes.
- Make your changes and commit them with a clear commit message.
- Push your changes to GitHub and open a pull request.
- Respond to any feedback on your pull request. The eunomia maintainers will review your changes and may request modifications before merging.
- Once your pull request is merged, you will be listed as a contributor in the project repository and documentation.

### Add signing keys

In order to mark your commit as `verified`, you have to first [*add a gpg key to Github*](https://docs.github.com/en/enterprise-cloud@latest/authentication/managing-commit-signature-verification/adding-a-gpg-key-to-your-github-account). Alternatively, you can use your existing SSH key for signing if you are using
Git 2.34 or later. More information could be found at [*Telling Git about your signing key*](https://docs.github.com/en/enterprise-cloud@latest/authentication/managing-commit-signature-verification/telling-git-about-your-signing-key).

### Commit sign-off

Contributors sign-off that they adhere to these requirements by adding a Signed-off-by line to commit messages.

```bash
This is my commit message

Signed-off-by: Random J Developer <random@developer.example.org>
```

Git even has a -s command line option to append this automatically to your commit message:

```bash
$ git commit -s -m 'This is my commit message'
```

### Rebase the branch

If you have a local git environment and meet the criteria below, one option is to rebase the branch and add your Signed-off-by lines in the new commits. Please note that if others have already begun work based upon the commits in this branch, this solution will rewrite history and may cause serious issues for collaborators (described in the git documentation under “The Perils of Rebasing”).

You should only do this if:

- You are the only author of the commits in this branch
- You are absolutely certain nobody else is doing any work based upon this branch
- There are no empty commits in the branch (for example, a DCO Remediation Commit which was added using `-allow-empty`)

To add your Signed-off-by line to every commit in this branch:

- Ensure you have a local copy of your branch by checking out the pull request locally via command line.
- In your local branch, run: `git rebase HEAD~1 --signoff`
- Force push your changes to overwrite the branch: `git push --force-with-lease origin main`

## License

Eunomia is licensed under this Licensed:

- MIT LICENSE ( [LICENSE-MIT](LICENSE-MIT) or https://opensource.org/licenses/MIT)
- Apache License, Version 2.0 ([LICENSE-APACHE](LICENSE-APACHE) or https://www.apache.org/licenses/LICENSE-2.0)
