/prompts/raw_data/create_function_readmes.md

#### CONTEXT

<hr>

#### INPUT

Functions
    pytest-approx
    pytest-fail
    pytest-skip
    pytest-importorskip
    pytest-xfail
    pytest-exit
    pytest-main
    pytest-param
    pytest-raises
    pytest-deprecated-call
    pytest-register-assert-rewrite
    pytest-warns
    pytest-freeze-includes

#### OUTPUT


Functions
```bash
mkdir -p functions/api/approx && echo '#### functions/api/approx/README.md' > functions/api/approx/README.md
mkdir -p functions/api/fail && echo '#### functions/api/fail/README.md' > functions/api/fail/README.md
mkdir -p functions/api/skip && echo '#### functions/api/skip/README.md' > functions/api/skip/README.md
mkdir -p functions/api/importorskip && echo '#### functions/api/importorskip/README.md' > functions/api/importorskip/README.md
mkdir -p functions/api/xfail && echo '#### functions/api/xfail/README.md' > functions/api/xfail/README.md
mkdir -p functions/api/exit && echo '#### functions/api/exit/README.md' > functions/api/exit/README.md
mkdir -p functions/api/main && echo '#### functions/api/main/README.md' > functions/api/main/README.md
mkdir -p functions/api/param && echo '#### functions/api/param/README.md' > functions/api/param/README.md
mkdir -p functions/api/raises && echo '#### functions/api/raises/README.md' > functions/api/raises/README.md
mkdir -p functions/api/deprecated_call && echo '#### functions/api/deprecated_call/README.md' > functions/api/deprecated_call/README.md
mkdir -p functions/api/register_assert_rewrite && echo '#### functions/api/register_assert_rewrite/README.md' > functions/api/register_assert_rewrite/README.md
mkdir -p functions/api/warns && echo '#### functions/api/warns/README.md' > functions/api/warns/README.md
mkdir -p functions/api/freeze_includes && echo '#### functions/api/freeze_includes/README.md' > functions/api/freeze_includes/README.md
```


#### FORMATTING COMMANDS

```markdown
Order **bash scripts** by lexicographic order 
on the key in `mkdir - {key}`.
```
```markdown
Order **table rows** alphabetically.
```