/prompts/raw_data/update_directory_link.md

#### Context

Each row of top level directories in the table `DIRECTORY|DESCRIPTION|MOTIVATION|` should link to that directory's `README.md`.

> [!NOTE]
> A top level directory is `./top_level/`.

#### Input

| Directory    | Description                                | Motivation                                |
| ------------ | ------------------------------------------ | ----------------------------------------- | --- |
| case studies | I write up issues and pull requests here.  | examples and retrospection are teachers   |     |
| prompts      | I write prompts and prompt pipelines here. | automation frees up higher-level thinking |     |

#### Output

| Directory                               | Description                                | Motivation                                |
| --------------------------------------- | ------------------------------------------ | ----------------------------------------- | --- |
| [case studies](/case_studies/README.md) | I write up issues and pull requests here.  | examples and retrospection are teachers   |     |
| [prompts](/prompts/README.md)           | I write prompts and prompt pipelines here. | automation frees up higher-level thinking |     |
