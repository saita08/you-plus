# you-plus

AI に丸ごと任せれば、形にはなる。ただ、自分の理解が置いていかれる——you-plus はそこを埋めるスキル群である。AI が代わりに考えるのではなく、問いに答えるうちに自分の考えが言葉になり、パターンとして見え、足りなかった定石が埋まっていく。対話が終わったとき、手元には自分の言葉で書かれた文書と、次は一人で考えられる引き出しが残る。

English version follows the Japanese section.

## スキル一覧

| スキル | 用途 |
|---|---|
| [shape-your-feature](skills/shape-your-feature/SKILL.md) | 作りたいものが決まっている人が、作り始める前に使う。既に持っているものと知っていることを問いで取り出し、足りない分は調べ方ごと渡し、AI に渡せる計画書に着地させる |

## 導入

同じスキル一式が、どの経路からも入る。

### コマンドラインから

| 対象 | コマンド |
|---|---|
| npx skills 対応エージェント | `npx skills add saita08/you-plus` |
| gh skill 対応エージェント | `gh skill install saita08/you-plus` |
| Claude Code のみ | `npx skills add saita08/you-plus --agent claude-code` |
| Codex のみ | `npx skills add saita08/you-plus --agent codex` |

### マーケットプレイスから

Claude Code 内で実行する。スキルごとに一つのプラグインなので、使うものだけ入れる。

```
/plugin marketplace add saita08/you-plus
/plugin install shape-your-feature@you-plus
```

Codex 内で実行する。ChatGPT デスクトップアプリは Plugins Directory に同じマーケットプレイスを追加する。

```
/plugin marketplace add saita08/you-plus
/plugin install you-plus@you-plus
```

### Claude.ai

1. [Releases](https://github.com/saita08/you-plus/releases) からスキルの zip をダウンロードする
2. 設定 > カスタマイズ > スキル からアップロードする

## ライセンス

[MIT](LICENSE)

---

# you-plus (English)

Hand everything to AI and you get something that works — while your own understanding falls behind. you-plus is a set of skills that closes that gap. Instead of the AI thinking for you, you answer questions until your idea takes words, then shows itself as a known pattern, and the standard practices you were missing fall into place. When the dialogue ends, you are left with a document written in your own words — and thinking you can reuse on your own next time.

## Skills

| Skill | Purpose |
|---|---|
| [shape-your-feature](skills/shape-your-feature/SKILL.md) | For someone who already knows what they want to build, used before they start. Draws out what you already have and already know through questions, hands over how to search for the rest, and lands everything in a plan you can hand to an AI |

## Installation

The same set of skills installs through any of these routes.

### From the command line

| Target | Command |
|---|---|
| Agents that support npx skills | `npx skills add saita08/you-plus` |
| Agents that support gh skill | `gh skill install saita08/you-plus` |
| Claude Code only | `npx skills add saita08/you-plus --agent claude-code` |
| Codex only | `npx skills add saita08/you-plus --agent codex` |

### From a marketplace

Run inside Claude Code. Each skill is its own plugin, so install only the ones you need.

```
/plugin marketplace add saita08/you-plus
/plugin install shape-your-feature@you-plus
```

Run inside Codex. In the ChatGPT desktop app, add the same marketplace in the Plugins Directory.

```
/plugin marketplace add saita08/you-plus
/plugin install you-plus@you-plus
```

### Claude.ai

1. Download the skill's zip from [Releases](https://github.com/saita08/you-plus/releases)
2. Upload it under Settings > Customize > Skills

## License

[MIT](LICENSE)
