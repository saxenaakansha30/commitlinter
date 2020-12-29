# CommitLinter

CommitLinter enables to validate commit message against simple five rules. If the message not satisfies the rule it throws respective errors.
1. Separate subject from body with a blank line (Work in progress)
2. Limit the commit subject line to 50 characters.
3. Capitalize the subject line
4. Do not end the subject line with a period
5. Use the imperative mood in the subject line (Work in progress)


## Installation

1. Requires python, for more info install python from https://www.python.org/downloads/
2. Change directory to the root of your project.
```bash
 cd project_name
```
3. Go to the git hook directory.
```bash
 cd .git/hook
```
4. Copy the commit-msg file to this directory. The file path should look like  ``.git/hooks/commit-msg``
5. Make the file executable
```bash
 chmod +x commit-msg
```
## Usage

Commit as usual you do like ``git commit -m "This is test message." <files>``. If your commit doesn't meet the above specified 5 rules the linter will throw error like for this example it should throw ``Err: Do not end the commit subject line with a period`` without fixing the reported error you would not be able to commit successful

```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
[MIT](https://choosealicense.com/licenses/mit/)
