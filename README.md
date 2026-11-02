# 非営利学生団体GUILD 公式サイト（GitHub Pages版）

旧サイト https://nposub-guild.amebaownd.com/ （Ameba Ownd）から移転するために、
GitHub Organization `nposub-guild` 向けにローカルで構築した静的サイトです。

**公開中： https://nposub-guild.github.io/**
（2026-11-03に Organization `nposub-guild` のリポジトリ `nposub-guild.github.io` へ push して公開）

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

## 更新方法

1. このリポジトリのファイルを編集して main ブランチへ push すると、数分で自動的にサイトへ反映されます
2. 旧サイト・SNS（X @SUBNPO_G / Instagram @subnpo_g）のリンクは、順次新URLへ差し替えてください
