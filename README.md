# you-plus

AI に丸ごと任せれば、形にはなる。ただ、自分の理解が置いていかれる——you-plus はそこを埋めるスキル群である。AI が代わりに考えるのではなく、問いに答えるうちに自分の考えが言葉になり、構造になり、足りなかった定石が埋まっていく。対話が終わったとき、手元には自分の言葉で書かれた文書と、次は一人で考えられる引き出しが残る。

English version follows the Japanese section.

## スキル一覧

| スキル | 用途 |
|---|---|
| [shape-your-feature](skills/shape-your-feature/SKILL.md) | 作りたいものが決まっている人が、作り始める前に使う。既に持っているものと知っていることを問いで取り出し、足りない分は調べ方ごと渡し、AI に渡せる計画書に着地させる |

## 導入方法

同一のスキル一式が、以下のすべての経路で利用できる。

### npx skills 対応エージェント

コマンドラインで次を実行する。Claude Code を含む、対応するエージェントすべてで使える。

```sh
npx skills add saita08/you-plus
```

### Claude Code

Claude Code だけに入れる場合は、コマンドラインで次を実行する。`.agents/` を作らず、`.claude/skills/` へ直接入る。

```sh
npx skills add saita08/you-plus --agent claude-code
```

マーケットプレイスとして登録する場合は、Claude Code 内で次を実行する。スキルは一つずつ独立したプラグインなので、使うものだけ選んで入れられる。

```
/plugin marketplace add saita08/you-plus
/plugin install shape-your-feature@you-plus
```

### Codex と ChatGPT

Codex だけに入れる場合は、コマンドラインで次を実行する。Codex が直接読む `.agents/skills/` へ入る。

```sh
npx skills add saita08/you-plus --agent codex
```

マーケットプレイスとして登録する場合は、Codex 内で次を実行する。

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
| [shape-your-feature](skills/shape-your-feature/SKILL.md) | For someone who already knows what they want to build, used before they start. Draws out what you already have and already know through questions, hands over how to search for the rest, and lands everything in a plan you can hand to an AI |

## Installation

The same set of skills works through every route below.

### Agents that support npx skills

Run the following from the command line. It works for every supported agent, Claude Code included.

```sh
npx skills add saita08/you-plus
```

### Claude Code

To install for Claude Code only, run the following from the command line. Skills go directly into `.claude/skills/`, without creating `.agents/`.

```sh
npx skills add saita08/you-plus --agent claude-code
```

To register the repository as a marketplace, run the following inside Claude Code. Each skill is its own plugin, so you can install only the ones you need.

```
/plugin marketplace add saita08/you-plus
/plugin install shape-your-feature@you-plus
```

### Codex and ChatGPT

To install for Codex only, run the following from the command line. Skills go into `.agents/skills/`, which Codex reads directly.

```sh
npx skills add saita08/you-plus --agent codex
```

To register the repository as a marketplace, run the following inside Codex.

```
/plugin marketplace add saita08/you-plus
/plugin install you-plus@you-plus
```

In the ChatGPT desktop app, add this marketplace in the Plugins Directory and install from there.

### Claude.ai

1. Download a .skill file from [Releases](../../releases)
2. Open Settings > Customize > Skills and upload it
3. The skill activates automatically when a relevant conversation begins

## License

[MIT](LICENSE)
