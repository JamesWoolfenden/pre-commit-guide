# Pre-commit Usage

## Install

Pre-commit requires three things to work:

- install the tool

```shell
pip3 install pre-commit
Pre-commit install
```

- create the hooks config
  In the root of repository is the config **.pre-commit-config.yaml**, this contains the config of which hooks, version and how they should be run. Below is a link to an example.

  <https://raw.githubusercontent.com/bridgecrewio/terraform-aws-bridgecrew-remediation/main/.pre-commit-config.yaml>
- install the config/hooks for the local repository

  ```shell
  pre-commit install
  ```

![install pre-commit](https://gist.githubusercontent.com/JamesWoolfenden/cc23ee81879f21deef8580dde8f25c5a/raw/b7704edb429c902ed07465aba0264b9bb0cbc620/termtosvg_uy8yp1qr.svg)

## Running a scan

You can run all hooks, or specify or only run them on commit.

![Run a Scan](https://gist.githubusercontent.com/JamesWoolfenden/e61e007e1c59738fab5981cb835cc57e/raw/e3073a2d1ea388dcf760268d005d826d84f5ea96/termtosvg_r8pao6de.svg)

Some of the hooks fix the violations, in this case it required the developer to edit.

## Commit to git

Now that the markdown has been edited you can commit the changes - the test will be run on commit.

![commit](https://gist.githubusercontent.com/JamesWoolfenden/d269229f7c0ed5b16b1ed6c31a295816/raw/964edc9ccec51b982a40d2a6839433a4b28c5f2b/termtosvg_aehmh7cl.svg)

### Created using

<https://github.com/nbedos/termtosvg>

<https://cli.github.com/>

```shell
$termtosvg
<do something>
$gh gist create <local svg file> -d install -f -P
```
