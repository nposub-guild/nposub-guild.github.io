# 非営利学生団体GUILD 公式サイト（GitHub Pages版）

旧サイト https://nposub-guild.amebaownd.com/ （Ameba Ownd）から移転するために、
GitHub Organization `nposub-guild` 向けにローカルで構築した静的サイトです。

**公開中： https://nposub-guild.github.io/**
（2026-11-03に Organization `nposub-guild` のリポジトリ `nposub-guild.github.io` へ push して公開）

## 構成

2026-11-03に、サブカル研究会GUILD公式サイト（https://guild3cha.github.io/）と同じ形式へ全面リニューアル。
共通CSS／JS・ヘッダー／フッター・セクション見出し・お知らせ行リスト・活動実績カード・テーマ切替
（ライト／ダーク、localStorageキー `guild-theme`）などの仕組みを同サイトと共通化した。
ページのURL・本文・画像は従来どおり維持している。

| ファイル | 内容 |
|---|---|
| `index.html` | トップ（額装ヒーロー／お知らせ最新3件／活動実績カード／PROJECT 子どもプログラミング教室／GUILDについて／公式SNS・お問い合わせ） |
| `work.html` | WORK：私たちのやれること①〜③ |
| `about.html` | ABOUT：団体紹介＋メンバー紹介（6名） |
| `news.html` | NEWS一覧（全5件、行リスト形式） |
| `news/*.html` | 記事ページ（旧サイトの原文＋画像をそのまま移行） |
| `assets/style.css` | 共通スタイル（guild3cha版と共通形式。NPOSUB用の追加分は末尾に明記） |
| `assets/site.js` | モバイルメニュー／テーマ切替／トップへ戻るボタン |
| `assets/images/` | 旧サイトから取得し軽量化した画像＋ロゴ透過版（`emblem-mark*.png`／`logo-horizontal*.png`） |

お知らせの追加方法：`news/` の既存記事を複製して日付・タイトル・本文・写真を差し替え、
`news.html` の一覧とトップの該当行／カードのリンクを更新する（guild3cha版と同じ運用）。

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
