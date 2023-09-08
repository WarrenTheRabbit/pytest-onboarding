/prompts/raw_data/create_minimal_readmes.md

#### CONTEXT
Each top level directory should contain a `README.md` that at a minimum describes its purpose.

For example,
<hr>

| Directory  | Description | Motivation | 
| ---- | --- | --- |
|[domain](/domain/README.md)| I speculate about and suggest domain objects here.| thinking about design increases understanding |Domain-Driven Design |
should have
```markdown
#/domain/README.md
I speculate about and suggest domain objects here. 
```
<hr>
#### INPUT

directory name: prompts
description: I write prompts and prompt pipelines here.
motivation: automation frees up higher-level thinking


#### OUTPUT
```bash
mkdir -p prompts && echo "I write prompts and prompt pipelines here." > prompts/README.md
```

#### FORMATTING COMMANDS

```markdown
Order **bash scripts** by lexicographic order 
on the key in `mkdir - {key}`.
```
```markdown
Order **table rows** alphabetically.
```