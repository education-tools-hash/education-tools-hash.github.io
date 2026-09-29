# Donomana Preview Environment

このrepositoryは [education-tools-hash/for-all-children-to-learn](https://github.com/education-tools-hash/for-all-children-to-learn)（どのまな／donomana.jp）の**Preview専用**環境です。

**Productionではありません。** donomana.jpとは完全に独立した別サイトです。

## 使い方

`Actions → preview-sync → Run workflow` から、`source_ref`にsource repoのcommit SHA（推奨）またはbranch名を指定して実行してください。source repoの指定checkpointを、このrepositoryのGitHub Pages（`https://education-tools-hash.github.io/`）へ、ファイルを加工せずそのまま配信します。

同期対象のアプリファイルやassetsはこのrepositoryのgit historyへは一切commitされません。すべてworkflow実行時にGitHub Actionsのartifactとしてのみ生成・deployされます（`.github/workflows/preview-sync.yml`参照）。

## 恒久ファイル

このrepositoryに恒久的に置かれるのは、この`README.md`と`.github/workflows/preview-sync.yml`のみです。
