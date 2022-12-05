# review-assign-action-example

[review-assign-action](https://github.com/hkusu/review-assign-action) で Reviewers を設定できないケース

1. PR 作者が指定されている（ GitHub の制限）
2. チームが指定されている（ [GitHub Actions Toolkit](https://github.com/actions/toolkit) の制限と思われる）

チームが指定された場合のエラーログ

```
Error: GitHub API error (message: Request failed with status code 422). "github-token" or "reviewers" may not be correct. For "reviewers", specify accounts that have permission to access the repository.
```

指定したチームに対して当該リポジトリにアクセス権を設定していても 422 となる。
