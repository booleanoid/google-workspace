# Google Workspace 設定管理リポジトリ

このリポジトリは、Google Workspace の設定方法・運用手順を管理するためのドキュメントリポジトリです。

## 目的

- Google Workspace の各種設定を文書化し、チーム間で共有する
- 設定変更の履歴を Git で追跡する
- 新規管理者のオンボーディングを支援する

## ディレクトリ構成

```
google-workspace/
├── README.md          # このファイル
├── admin/             # 管理コンソール設定
├── gmail/             # Gmail 設定
├── drive/             # Google Drive 設定
├── meet/              # Google Meet 設定
├── calendar/          # Google カレンダー設定
└── security/          # セキュリティ・アクセス管理設定
```

## 管理対象の主な設定項目

### 管理コンソール (admin.google.com)
- ユーザー管理（追加・削除・権限変更）
- 組織部門 (OU) 構成
- グループ管理

### Gmail
- メールルーティング設定
- スパムフィルター設定
- メール署名テンプレート
- DKIM / SPF / DMARC 設定

### Google Drive
- 共有設定（社外共有の制限）
- 共有ドライブの作成・管理
- ストレージポリシー

### セキュリティ
- 2段階認証 (2FA) の強制設定
- OAuth アプリのアクセス制御
- セキュリティアラートの設定

## 設定変更の手順

1. このリポジトリをクローンする
   ```bash
   git clone git@github.com:booleanoid/google-workspace.git
   cd google-workspace
   ```

2. 設定変更内容をドキュメントに記述する

3. ブランチを作成してプルリクエストを出す
   ```bash
   git checkout -b feature/your-setting-name
   # ドキュメントを編集
   git add .
   git commit -m "設定変更の概要"
   git push origin feature/your-setting-name
   ```

4. レビューを受けて、承認後にマージする

## 参考リンク

- [Google Workspace 管理者ヘルプ](https://support.google.com/a)
- [Google Workspace 管理コンソール](https://admin.google.com)
