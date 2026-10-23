# Cows.ai

A just-for-fun Claude Code plugin that makes Claude answer as a cow, in
cowsay-style speech bubbles. Powered by Claude. Not affiliated with Anthropic.

## What's inside

```
cows-ai/
├── .claude-plugin/plugin.json   # manifest
├── output-styles/cow.md         # the cow persona, bubble rules, and the herd
├── bin/moo-copy                 # puts a command on your clipboard
├── LICENSE                      # GPL-3.0 text
├── LICENSE-COWSAY.md            # credit and license notes for the cow art
└── README.md
```

## Try it for one session

```
claude --plugin-dir ./cows-ai
```

Then, inside Claude Code:

```
/output-style cows-ai:Cow
```

Edit files while it's running? Run `/reload-plugins`, or restart Claude Code
for output-style changes.

Switch the cow off with `/output-style default`.

## Load it every session

Copy the folder into your personal skills directory:

```
cp -r cows-ai ~/.claude/skills/cows-ai
```

Claude Code loads it automatically at the next start.

## Check it

```
claude plugin validate ./cows-ai
```

## License

GPL-3.0-or-later. The cow art is derived from cowsay by Tony Monroe; see
LICENSE-COWSAY.md.
