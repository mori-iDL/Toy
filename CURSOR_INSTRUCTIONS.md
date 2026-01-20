# Cursorへの指示：GitHubリポジトリ作成とプッシュ

以下のコマンドを順番に実行してください。

## 1. このフォルダに移動
```bash
cd [このフォルダのパス]
```

## 2. Git設定（未設定の場合）
```bash
git config user.name "あなたの名前"
git config user.email "あなたのメール"
```

## 3. 初回コミット
```bash
git add -A
git commit -m "Initial commit: 手描きパターンデザイナー v1.0

- 9種類の手描きパターンを実装
- パラメータ調整機能（有機的な揺らぎ、線の太さ、密度、スケール、回転）
- シード値による再現性
- SVG/PNG出力機能"
```

## 4. GitHubリポジトリ作成とプッシュ
```bash
gh repo create tegaki-pattern-designer --public --source=. --remote=origin --push
```

または、プライベートリポジトリの場合：
```bash
gh repo create tegaki-pattern-designer --private --source=. --remote=origin --push
```

## 5. 確認
```bash
gh repo view --web
```

---

## 今後のバージョン管理

変更があった場合：
```bash
git add -A
git commit -m "変更内容の説明"
git push
```
