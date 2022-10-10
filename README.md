# action-install-pact
Reusable action to install Pact standalone 

## Usage

```yaml
jobs:
  make-tests:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: replicatedhq/action-install-pact@v1
      - name: make pact-test
```

## Inputs
### version
The version of the standalone tools to use, without a leading _v_. **Default:** 1.91.0

### shasum
The SHA checksum of the x86_64 release tarball, as found in the release checksum file. **Default:** 9b745949f5f795d690941d6bf85444af325f248b