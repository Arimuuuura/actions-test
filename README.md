# Git hub でCI/CD

CI / CD ツール
スクリプトテストを git push したときに自動で実行してくれる
% npm test を自動で走らせるワークフロー

1. Git hub にリポジトリを作成

2. コードエディターで
```
% git clone リポジトリURL
hello.js 作成
% npm init
% npm install
% npm test
```

3. Git hub で
- 該当のリポジトリに移動
- Actions
- Node.js の Set up workflow ボタンをクリック
- リポジトリ名/.github/workflow/node.js.yml というファイルができる
- 右上の Start commit ボタンをクリック
- Commit new file ボタンをクリック

4. テスト
コードエディターでファイルを編集したのち
```
% git push
```

5. Git hub で
- Actions を確認
- スクリプトテストが走っていることが確認できる
