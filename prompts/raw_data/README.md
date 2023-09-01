## Raw Prompt Data
This directory contains files of *raw prompt data*. 

[Raw Prompt Files](#contents)
[Explanation](#explanation)


### Contents
| PROMPT BEHAVIOUR | 
| --- | 
| [prompt(readme): update directory column with links](/prompts/raw_data/update_directory_links.md)| 
| [prompt(cases): tabulate a history](/prompts/raw_data/create_case_history.md)
| [prompt(readme): create minimal top level READMEs](/prompts/raw_data/create_minimal_readmes.md)|
| [prompt(prompt): create a link to a prompt](/prompts/raw_data/create_prompt_row.md)|

### Explanation

##### Motivation
*raw prompt data* provides the building blocks for one-shot and few-shot prompts. If these building blocks are collected, it is easier to automate manual input-to-output processes at a later stage.

##### Process
Whenever I change text from one form to another and anticipate it would be helpful if that process were highly efficient in the future, I add a *raw prompt data* file to this directory. 

##### Expected Structure
A *raw prompt data* file should contain the following:

```markdown
#### Context
(comments)
(links to useful external files/resources)

#### Input
(the original text)

#### Output
(the text after the input has been processed)

#### Formatting Commands {Optional}
(subprompts for formatting input or output text)
```





