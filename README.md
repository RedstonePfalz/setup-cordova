## setup-cordova


Setup your GitHub Actions workflow with Apache Cordova.

**Note: Since this runs in a Linux-based Docker image, Xcode is not available for iOS builds.**

## Example

```yaml
- name: Use RedstonePfalz/setup-cordova
  uses: RedstonePfalz/setup-cordova@0.0.4
  with:
    exec: |
      cordova platform add android && \
      cordova build --no-telemetry && \
      cp "$(find . -name '*.apk')" .
```

## Acknowledgement

Initially based on [coturiv/setup-ionic](https://github.com/coturiv/setup-ionic).

## License

SPDX-License-Identifier: [MIT](LICENSE)

## Reference

- [Hello world docker action](https://github.com/actions/hello-world-docker-action)

## See Also

- [Setup Leiningen](https://github.com/oxr463/setup-leiningen)
