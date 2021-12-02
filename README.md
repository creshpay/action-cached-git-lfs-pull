# Action-cached-git-fls-pull

This action is used to do git pull LFS leveraging github action cache

## Requirement

Your have to checkout your project containing the Dockerfile before running the action. Be sure to set lfs to false.

## Usage

See [action.yml](action.yml)

Basic:

```yaml
steps:
- name: Checkout repository
  uses: actions/checkout@v2
  with:
      token: ${{ secrets.GITHUB_TOKEN }}

- name: Pull LFS
  uses: cresh-io/action-cached-git-lfs-pull@v1
```

## Thanks

This composite is inspired of the great works of : [action-cached-lfs-checkout](https://github.com/nschloe/action-cached-lfs-checkout)

## License

The scripts and documentation in this project are released under the [MIT License](LICENSE)
