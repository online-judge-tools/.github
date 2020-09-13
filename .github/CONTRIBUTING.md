# Contribution Guide

## The first step

### If you found a bug / バグを見つけた場合

Please report by making an issue about the bug. / issue を立てて、バグについて報告してください。

Even when you are going to create the pull request, please make an issue first, because it makes easy to track bugs. Of course you can create a pull request without issues when the bugs are trivial (e.g. typo). / プルリクエストを書くつもりの場合も、まずは issue を立ててください。バグの管理がしやすくなるためです。もちろん typo のような重要でないバグについては issue なしでいきなりプルリクエストを作ってしまっても大丈夫です。


### If you want a new feature / ほしい機能がある場合

Please make an issue first and describe the feature. / まずは issue を立て、その機能について説明してください。

We don't recommend to try to create pull requests without issues. We should discuss the feature before you implement it, because such pull requests are sometimes difficult to implement and not always merged even if it's implemented. / issue なしでいきなりプルリクエストを作ろうとするのはおすすめしません。機能を追加するプルリクエストは実装が難しい場合があり、またもし実装できても常にマージされるとは限りません。なので、実装する前に機能について議論しておいた方がよいでしょう。


### If you're not in any trouble, but you want to help you anyway / なにか困っているわけではないが、できることがあれば手伝いたいという場合

You're welcome!

Please ask the maintainers what you can do via issues or other SNSs.
We will suggest you to contribute by doing:

-   Proposing features
-   Implementing code
-   Writing documents
-   Supporting other users directly
    -   on GitHub issues
    -   on other SNSs (e.g. Twitter)


## Making pull requests

### How to install the package from the source / ソースコードからインストールするには

Run `$ pip3 install -e .[dev]` on the root directly of the project.

### About tests / テストについて

We are running format checkers (`yapf` and `isort`), a linter (`pylint`), and many tests (`test/*.py`) in GitHub Actions.
They runs automatically when you make a pull request. Pull requests cannot be merged until all tests pass.
To run them locally, see the workflows of GitHub Actions (`.github/workflows/*.yml`).

By the way, the checks with `pylint` may be too strict. You can use `# pylint: disable=...` or edit `setup.cfg` if it's reasonable.

### How to pass the review / コードレビューについて

We review your pull request before merging to keep the quality of the product.
So you don't have to worry about your pull request breaking the product.

To pass the process:

-   You can read:
    -   other pull requests
    -   our [maintainers-guide.md](https://github.com/online-judge-tools/.github/blob/master/maintainers-guide.md)
    -   external resources like [How to write the perfect pull request - The GitHub Blog](https://github.blog/2015-01-21-how-to-write-the-perfect-pull-request/), or [The Change Author’s Guide](https://google.github.io/eng-practices/review/developer/) of [Google Engineering Practices Documentation](https://google.github.io/eng-practices/)
-   When you get some comments, please fix your code or logically persuade the reviewers.
