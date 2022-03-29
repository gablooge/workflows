
# GitHub Workflows


[![Tests](https://github.com/20c/workflows/workflows/ci/badge.svg)](https://github.com/20c/workflows/actions/workflows/ci.yaml)


## poetry

Action to install and cache poetry and the virtualenv it installs to.

```yaml
inputs:
  python-version:
    required: false
    default: 3.x
    type: string
outputs:
  venv-path:
    description: "virtualenv path"
    value: ${{ steps.get-venv-path.outputs.venv-path }}
```

## Release

```sh
git tag -a -m "bump v1" v1
git push --follow-tags
```

## License

Copyright 2016-2021 20C, LLC

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this software except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
