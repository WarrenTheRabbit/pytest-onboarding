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

| Directory  | Description | Motivation | 
| ---- | --- | --- |
|[advice](/advice/README.md)| I write up advice I've received from pytest devs here.    | juniors can give back by documenting and scaling advice|
|[case studies](/case_studies/README.md)| I write up issues and pull requests here.    | examples and retrospection are teachers|
|[domain](/domain/README.md)| I speculate about and suggest domain objects here.    | thinking about design increases understanding |Domain-Driven Design |
|[functions](/functions/README.md)| I summarise and hypothesise about pytest functions here. | knowledge is data organised, memories are senses processed  |
|[objects](/objects/README.md)| I summarise and hypothesise about pytest objects here. | knowledge is data organised, memories are senses processed  |
|[packages](/packages/README.md)| I summarise and hypothesise about pytest packages here. | knowledge is data organised, memories are senses processed  |
|[prompts](/prompts/README.md)| I write prompts and prompt pipelines here.    | automation frees up higher-level thinking  | 
|[scripts](/scripts/README.md)| I keep scripts that help manage this repo here. | automation frees up higher-level thinking |


#### OUTPUT
```bash
mkdir -p advice && echo "I write up advice I've received from pytest devs here." > advice/README.md 
mkdir -p case_studies && echo "I write up issues and pull requests here." > case_studies/README.md 
mkdir -p domain && echo "I speculate about and suggest domain objects here." > domain/README.md 
mkdir -p functions && echo "I summarise and hypothesise about pytest functions here." > functions/README.md 
mkdir -p objects && echo "I summarise and hypothesise about pytest objects here." > objects/README.md 
mkdir -p packages && echo "I summarise and hypothesise about pytest packages here." > packages/README.md 
mkdir -p prompts && echo "I write prompts and prompt pipelines here." > prompts/README.md 
mkdir -p scripts && echo "I keep scripts that help manage this repo here." > scripts/README.md 
```

#### FORMATTING COMMANDS

```markdown
Order **bash scripts** by lexicographic order 
on the key in `mkdir - {key}`.
```
```markdown
Order **table rows** alphabetically.
```