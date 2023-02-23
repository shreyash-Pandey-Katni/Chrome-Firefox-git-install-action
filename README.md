# Github Action: Install Chrome, Firefox and Git on OS

This is a Github Action that installs Chrome, Firefox and Git on the OS. This action works on both Linux and Windows systems.

### Inputs

This action has the following inputs:
* `chrome`: A boolean input that indicates whether Chrome should be installed or not. Default value is false.
* `firefox`: A boolean input that indicates whether Firefox should be installed or not. Default value is false.
* `git`: A boolean input that indicates whether Git should be installed or not. Default value is false.
* `isWindows`: A boolean input that indicates whether the OS is Windows or not. Default value is true if the runner's OS is Windows, otherwise false. It is not required to set this input as it detects OS automatically.

### Outputs

This action does not have any outputs.

### Example Usage

```
name: Example Workflow

on: [push]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
    - name: Install Chrome, Firefox and Git on OS
      uses: username/repo-name@v1
      with:
        chrome: true
        firefox: true
        git: true
```

### License

This action is licensed under the [MIT License](LICENSE).
