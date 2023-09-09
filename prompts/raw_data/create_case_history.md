/prompts/raw_data/create_case_history.md

#### Context

Each case study should have a table that summarises its associated history of issues and pull requests.

See [this case study](https://github.com/WarrenTheRabbit/pytest-onboarding/blob/main/case_studies/11345/README.md) for an example of how the output is used.

#### Input
type-error

https://github.com/pytest-dev/pytest/issues/11343
WarrenTheRabbit
2023-08-23
identifies two `[attr-defined]` errors


https://github.com/pytest-dev/pytest/pull/11345
WarrenTheRabbit
2023-08-07
fixes two `[attr-defined]` type errors


#### Output
mkdir -p ./case_studies/type-error
cat > ./case_studies/type-error/README.md << 'EOF'
| Event                                                             | Date       | Author                                                | Summary                                |
| ----------------------------------------------------------------- | ---------- | ----------------------------------------------------- | -------------------------------------- |
| [Issue #11343](https://github.com/pytest-dev/pytest/issues/11343) | 2023-08-23 | [WarrenTheRabbit](https://github.com/WarrenTheRabbit) | identifies two `[attr-defined]` errors |
| [PR #11345](https://github.com/pytest-dev/pytest/pull/11345)      | 2023-08-07 | [WarrenTheRabbit](https://github.com/WarrenTheRabbit) | fixes two `[attr-defined]` type errors |
EOF