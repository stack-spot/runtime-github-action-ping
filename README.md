# runtime-github-action-ping

[![Action test Ubuntu](https://github.com/stack-spot/runtime-github-action-ping/actions/workflows/action-test-ubuntu.yml/badge.svg)](https://github.com/stack-spot/runtime-github-action-ping/actions/workflows/action-test-ubuntu.yml) [![Action test MacOS](https://github.com/stack-spot/runtime-github-action-ping/actions/workflows/action-test-macos.yml/badge.svg)](https://github.com/stack-spot/runtime-github-action-ping/actions/workflows/action-test-macos.yml) [![Action test Windows](https://github.com/stack-spot/runtime-github-action-ping/actions/workflows/action-test-windows.yml/badge.svg)](https://github.com/stack-spot/runtime-github-action-ping/actions/workflows/action-test-windows.yml)

GitHub action to install StackSpot CLI :octocat:

_**Note**: This action is supported on all runners operating systems (`ubuntu`, `macos`, `windows`)_

## 📚 Usage

### Requirements

To get the account keys (`CLIENT_ID`, `CLIENT_KEY` and `CLIENT_REALM`), please login using a **ADMIN** user on the [StackSpot Portal](https://stackspot.com), and generate new keys at [https://stackspot.com/en/settings/access-token](https://stackspot.com/en/settings/access-token).

### Use Case

```yaml
    steps:
      - uses: stack-spot/runtime-github-action-ping@v1
        with:
          CLIENT_ID: ${{ secrets.CLIENT_ID }}
          CLIENT_KEY: ${{ secrets.CLIENT_KEY }}
          CLIENT_REALM: ${{ secrets.CLIENT_REALM }}
```

## License

[Apache License 2.0](https://github.com/stack-spot/runtime-github-action-ping/blob/main/LICENSE)