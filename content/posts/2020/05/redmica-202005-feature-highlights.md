---
title: "RedMica 1.1 主な新機能"
date: 2020-05-08T15:32:43+09:00
---

今月リリース予定のRedMica 1.1の新機能をいくつかピックアップ。

なお、Redmineにおいてはこれらの機能はRedmine 4.2（リリース時期不明）に含まれる。

## Accounts / authentication

* [Feature #3369: Allowed/Disallowed email domains settings to restrict users' email addresses](https://www.redmine.org/issues/3369): ユーザーアカウントで使用できるメールアドレスのドメインを制限するための設定「許可するメールアドレスのドメイン」「禁止するメールアドレスのドメイン」を追加。例えばユーザーが勝手に組織外のメールアドレスを設定するのを防ぐ（情報流出防止）ようにできる
* [Feature #33126: Support custom fields when exporting users to CSV](https://www.redmine.org/issues/33126): ユーザーのCSVエクスポートがカスタムフィールドに対応
* [Feature #33347: Include updated_on and passwd_changed_on columns when exporting users to CSV](https://www.redmine.org/issues/33347): ユーザーのCSVエクスポートで得られるCSVに「更新日」「パスワード最終更新日」を追加

## Attachments

* [Feature #7056: Download all attachments at once](https://www.redmine.org/issues/7056): 特定のチケットやWikiページに添付されている添付ファイルをまとめてZIP形式でアーカイブしてダウンロード

## Email notifications

* [Patch #32628: Notify users about high issues (only)](https://www.redmine.org/issues/32628): 「個人設定」内のメール通知に、優先度がデフォルトよりも高いチケットについても通知を行うオプションを追加。例えば通知対象を「ウォッチ中または自分が関係しているもの」としている場合も、優先度が高いチケットについては必ずメール通知を行うようにできる

 ## Importers

* [Feature #28198: Support issue relations when importing issues](https://www.redmine.org/issues/28198): チケットをCSVファイルからインポートするときに「関連するチケット」の情報もインポート
* [Patch #22913: Auto-select fields mapping in Importing](https://www.redmine.org/issues/22913): CSVインポートを行うとき、これまで手作業で一つ一つ設定していた「フィールドの対応関係」がCSVファイルの列名をもとに自動で設定

##  Issues

* [Feature #4511: Allow adding user groups as watchers for issues](https://www.redmine.org/issues/4511): グループをチケットのウォッチャーに追加。これまではユーザーしか追加できなかった
* [Feature #33254: Show open/closed badge on issue page](https://www.redmine.org/issues/33254): チケット表示画面に「完了」「未完了」のバッジを表示

## Projects

* [Feature #32818: Add a system settings for default results display format of project query](https://www.redmine.org/issues/32818): プロジェクト画面の表示形式のデフォルト値を定義する設定を「管理」→「設定」→「プロジェクト」に追加

## Text formatting

* [Feature #1575: Toolbar button to insert a table](https://www.redmine.org/issues/1575): Wikiツールバーにテーブルを挿入するためのボタンを追加
* [Feature #32528: Make languages in Highlighted code button in toolbar customizable](https://www.redmine.org/issues/32528): Wikiツールバーのシンタックスハイライトボタンで使用する言語を定義できる設定「ツールバーのコードハイライトボタンで使用する言語」を「個人設定」に追加

## Time tracking

* [Patch #32436: Add support for grouping by issue on timelog view](https://www.redmine.org/issues/32436): 作業時間の一覧で利用できるグループ条件に「チケット」を追加。作業時間の明細をチケットごとに見ることができるようになる

##  UI

* [Feature #31589: Show warning and the reason when the issue cannot be closed because of open subtasks or blocking open issue(s)](https://www.redmine.org/issues/31589): 未完了の子チケットやブロックしているチケットが原因でチケットをクローズできないときに理由を表示
* [Patch #29285: Add &quot;Assign to me&quot; shortcut to issue edit form](https://www.redmine.org/issues/29285): チケットの編集画面に「自分に割り当て」リンクを追加
