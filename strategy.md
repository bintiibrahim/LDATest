# Goal
1. Online - latest version only
2. Offline - all versions available on DownloadOffline.html
3. Want to be able to access older online versions

# Strategy
When a new version is ready...
1. ewfrees updates offline version in `DownloadOffline.html`
2. ewfrees commits changes to OpenActTexts (updates online version)
3. OpenActTexts creates release `v#.#` from master

If want to revert current online version to an older version (this will overwrite all changes)
 ```
git checkout master
git reset --hard v#.#
git push --force origin master
```
