# Jest Unit Test

## Pre environment
Need to install `jest` first

## Install
1. Create a folder name `.arc-extensions` under the root directory of project
2. Put `arc-jest` into `.arc-extensions`

## arcconfig example
```json
{
  "load": [
    ".arc-extensions/arc-jest"
  ],
  "unit.engine": "JestUnitTestEngine",
  "unit.engine.jest.command": "NODE_ENV=test node scripts/test.js --env=jsdom --config jest.config.json"
}
```

## Usage
```bash
  arc unit
```


## Source
Forked from [jest-phabricator](https://github.com/facebook/jest/tree/master/packages/jest-phabricator) and customized by Cagen