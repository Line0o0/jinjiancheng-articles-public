# AGENTS

## Archive Workflow

- All commits in this repository must use the GitHub identity `Line0o0 <37470807+Line0o0@users.noreply.github.com>` for both author and committer. Never use a real name or a corporate email address in commit metadata.
- This repository is the public-text companion to `Line0o0/jinjiancheng-articles`. Keep both repositories synchronized whenever articles are added or refreshed.
- Whenever any 金渐成 / jinjiancheng / 鸡哥 / 机哥 / 玑哥 / 天机 article is fetched, imported, refreshed, or otherwise added to the full archive, add or update its public copy here in the same task. Commit and push both repositories, then verify both remote default branches contain the new article files. The archival task is incomplete until both repositories are current.
- Use the full archive's canonical `search/content.txt` as the source, then apply this repository's public redaction and text-normalization conventions. Store the result as `YYYY/YYYY-MM-DD_HHMM_account_mid-idx.txt`, where `account` is `jinjiancheng`, `tianji-qitan`, or `shengjibobo`.
- Preserve the existing public file format exactly: article body, a blank line, `---- COMMENTS ----`, then public comments. Do not publish `raw/` files, session data, cookies, tokens, OpenID, UnionID, local paths, scripts, notes, Wiki content, or other non-public artifacts.
- Before syncing, compare article identity by `mid` and `idx` across the entire full archive and this repository so older gaps are not missed. Do not limit the comparison to only the newest date.
- After adding files, update the year counts in `README.md`, verify the table matches the actual `.txt` file count, and check that each new public file preserves its canonical article body and comments except for required redaction and normalization.
- Before changes, fetch `origin/main`. Fast-forward a clean checkout that is behind; do not pull across unrelated local changes.
- After verification, create an intentional commit, push it to `origin/main`, and confirm the remote branch points to the pushed commit unless the user explicitly asks not to commit or push.
