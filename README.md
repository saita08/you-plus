# you-plus

AI に丸ごと任せれば、形にはなる。ただ、自分の理解が置いていかれる——you-plus はそこを埋めるスキル群である。AI が代わりに考えるのではなく、問いに答えるうちに自分の考えが言葉になり、構造になり、足りなかった定石が埋まっていく。対話が終わったとき、手元には自分の言葉で書かれた文書と、次は一人で考えられる引き出しが残る。

English version follows the Japanese section.

## スキル一覧

| スキル | 用途 |
|---|---|
| [shape-your-feature](skills/shape-your-feature/SKILL.md) | 何かを作り始める前に使う。構想を問いで引き出し、構造化し、不足している定石を補い、AI に渡せる計画書にまとめる |

## 導入方法

同一のスキル一式が、以下のすべての経路で利用できる。

### npx skills 対応エージェント

コマンドラインで次を実行する。Claude Code を含む、対応するエージェントすべてで使える。

```sh
npx skills add saita08/you-plus
```

### Claude Code

マーケットプレイスとして登録する場合は、Claude Code 内で次を実行する。

```
/plugin marketplace add saita08/you-plus
/plugin install you-plus@you-plus
```

### Codex と ChatGPT

Codex 内で次を実行し、マーケットプレイスとして登録する。

```
/plugin marketplace add saita08/you-plus
/plugin install you-plus@you-plus
```

ChatGPT デスクトップアプリでは、Plugins Directory にこのマーケットプレイスを追加してインストールする。

### Claude.ai

1. [Releases](../../releases) から .skill ファイルをダウンロードする
2. 設定から カスタマイズ > スキル を開き、アップロードする
3. 該当する話題を始めると、スキルが自動で適用される

## ライセンス

[MIT](LICENSE)

---

# you-plus (English)

Hand everything to AI and you get something that works — while your own understanding falls behind. you-plus is a set of skills that closes that gap. Instead of the AI thinking for you, you answer questions until your idea takes words, then shape, and the standard practices you were missing fall into place. When the dialogue ends, you are left with a document written in your own words — and thinking you can reuse on your own next time.

## Skills

| Skill | Purpose |
|---|---|
| [shape-your-feature](skills/shape-your-feature/SKILL.md) | Use before starting to build something. Draws out your idea through questions, structures it, supplies missing standard practices, and lands everything in a plan you can hand to an AI |

## Installation

The same set of skills works through every route below.

### Agents that support npx skills

Run the following from the command line. It works for every supported agent, Claude Code included.

```sh
npx skills add saita08/you-plus
```

### Claude Code

To register the repository as a marketplace, run the following inside Claude Code.

```
/plugin marketplace add saita08/you-plus
/plugin install you-plus@you-plus
```

### Codex and ChatGPT

Run the following inside Codex to register the repository as a marketplace.

```
/plugin marketplace add saita08/you-plus
/plugin install you-plus@you-plus
```

In the ChatGPT desktop app, add this marketplace in the Plugins Directory and install from there.

### Claude.ai

1. Download a .skill file from [Releases](../../releases)
2. Open Settings > Capabilities > Skills and upload it
3. The skill activates automatically when a relevant conversation begins

## License

[MIT](LICENSE)
