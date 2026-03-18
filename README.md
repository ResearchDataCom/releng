# Release Engineering

Simplify project maintenance with shared GitHub Actions workflows that
enable privilege separation, facilitate reproducible builds, and
support matrix strategies.

> [!NOTE]
>
> Workflows in other private repositories in this organization
> **MUST** be able to access this repository.  For more information,
> refer to
> [Sharing actions and workflows from your private repository](https://docs.github.com/en/actions/how-tos/reuse-automations/share-across-private-repositories).

[_Good DevOps Practice_](https://github.com/ResearchDataCom/good-devops-practice)
describes the underlying methodology and recommended tooling in
greater detail.  For an example of how to use these workflows, refer
to the
[Python project template's CI workflow](https://github.com/ResearchDataCom/good-devops-practice/blob/main/python-template/%7B%7B%20cookiecutter.package_slug%20%7D%7D/.github/workflows/ci.yml).

## Available Workflows

Workflows are listed in alphabetical order.  Refer to the linked
workflow definitions for additional details.

<dl>

<dt><a href="cz-bump/action.yml">cz-bump</a></dt>
<dd>Determines the next version number, updates project metadata, and
tags the new release; requires <code>contents: write</code>
permissions.</dd>

<dt><a href="publish-github/action.yaml">publish-github</a></dt>
<dd>Retrieves build artifacts and uploads them to the corresponding
GitHub release; requires <code>contents: write</code>
permissions.</dd>

<dt><a href="python-lint/action.yml">python-lint</a></dt>
<dd>Checks Python code syntax/style using the configured pre-commit
hooks and generates dependency pins.</dd>

<dt><a href="python-test/action.yml">python-test</a></dt>
<dd>Runs pytest via GNU Make.</dd>

<dt><a href="python-build/action.yml">python-build</a></dt>
<dd>Builds a Python distribution via GNU Make and stores the results
in a workflow artifact.</dd>

</dl>

## References

[The Right Way to Handle Permissions in GitHub Actions](https://shreyapohekar.com/blogs/the-right-way-to-handle-permissions-in-github-actions-a-practical-guide-to-staying-secure/)

[Securing GitHub Actions Workflows](https://wellarchitected.github.com/library/application-security/recommendations/actions-security/)

[Running variations of jobs in a workflow](https://docs.github.com/en/actions/how-tos/write-workflows/choose-what-workflows-do/run-job-variations)
