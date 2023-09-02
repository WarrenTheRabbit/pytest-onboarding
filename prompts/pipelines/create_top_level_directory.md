#### The Pipeline
Create a top level directory, its readme and an entry in the table of contents.
```mermaid
graph LR
    subgraph input
        data[- directory name <br> - description <br> - motivation]
    end
    subgraph root[Add an entry to the /README.md table]
        contents[create_content_page_entry] --> links[update_directory_links]
    end
    subgraph readmes[Create the dir and its readme]
        create_minimal_readmes
    end
    readmes --> root
    input --> readmes
```

#### Overview

Given

- a top level directory `name`
- a `description` of that directory's purpose
- the `motivation` for having that purpose

the creation of a top level directory should include the following steps:

1. Create the directory and a minimal readme file.
2. Add an entry for it to the `/README.md` table of contents.



#### Example
##### Inputs
`directory name`: prompts
`description`: I write prompts and prompt pipelines here.
`motivation`: automation frees up higher-level thinking

##### Outputs
Creates the `prompts` directory and a minimal readme file:

```markdown
# /prompts/README.md

I write prompts and prompt pipelines here.
```

Adds an entry for it to the `/README.md` table of contents:

```markdown
# /README.md

| DIRECTORY                     | DESCRIPTION                                | MOTIVATION                                |
| ----------------------------- | ------------------------------------------ | ----------------------------------------- |
| [prompts](/prompts/README.md) | I write prompts and prompt pipelines here. | automation frees up higher-level thinking |
```