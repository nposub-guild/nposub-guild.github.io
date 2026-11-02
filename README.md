# 非営利学生団体GUILD 公式サイト（GitHub Pages版・ローカル構築中）

旧サイト https://nposub-guild.amebaownd.com/ （Ameba Ownd）から移転するために、
GitHub Organization `nposub-guild` 向けにローカルで構築した静的サイトです。

**現在の状態：ローカルのみ。まだ公開（push）はしていません。**
公開先の想定URL： https://nposub-guild.github.io/
（リポジトリ名 `nposub-guild.github.io` で作成し、この中身をそのまま push する想定）

## 構成

| ファイル | 内容 |
|---|---|
| `index.html` | トップ（ヒーロー／PROJECT 子どもプログラミング教室／公式SNS／NEWS最新3件） |
| `work.html` | WORK：私たちのやれること①〜③ |
| `about.html` | ABOUT：団体紹介＋メンバー紹介（6名） |
| `news.html` | NEWS一覧（全5件） |
| `news/*.html` | 記事ページ（旧サイトの原文＋画像をそのまま移行） |
| `assets/css/style.css` | 共通スタイル（ライト／ダーク自動切替） |
| `assets/images/` | 旧サイトから取得し軽量化した画像 |

記事と旧サイトの対応：
- `news/programming-class-1.html` ← 第一回 子どもプログラミング教室（2026.06.28公開）
- `news/programming-class-2.html` ← 第二回 子どもプログラミング教室（2026.07.09公開）
- `news/setagaya-funding.html` ← せたがや若者ファンディング採択！（2026.07.09公開）
- `news/programming-class-3.html` ← 第三回 子どもプログラミング教室（2026.07.12公開）
- `news/programming-class-4.html` ← 第四回 子どもプログラミング教室（2026.07.26公開）

## ローカルで確認する方法

```bash
cd nposub-guild-site
python3 -m http.server 8000
# ブラウザで http://localhost:8000/ を開く
```

## 公開する時の手順（まだ未実施）

1. Organization `nposub-guild` に Public リポジトリ `nposub-guild.github.io` を作成
2. このディレクトリの中身を push
3. リポジトリ Settings → Pages で公開を確認（`*.github.io` リポジトリは自動で有効）
4. 公開後に旧サイト・SNS（X @SUBNPO_G / Instagram @subnpo_g）のリンクを新URLへ差し替え
