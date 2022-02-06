![Typescript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
<br />
![npm](https://badges.aleen42.com/src/npm.svg)
<br />
<br />
![Continuous Deployment](https://github.com/noahvarghese/logger/actions/workflows/cd.yaml/badge.svg)
<br />
![Continuous Integration](https://github.com/noahvarghese/logger/actions/workflows/ci.yaml/badge.svg)
<br />
<br />
![Statements](https://img.shields.io/badge/statements-96.77%25-brightgreen.svg?style=flat)
<br/>
![Lines](https://img.shields.io/badge/lines-98.18%25-brightgreen.svg?style=flat)
<br/>
![Functions](https://img.shields.io/badge/functions-100%25-brightgreen.svg?style=flat)
<br/>
![Branches](https://img.shields.io/badge/branches-89.28%25-yellow.svg?style=flat)
<br/>
<br/>
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
<br />
<br />

<img src="assets/log.png" width="100" alt="log" />

# Logger

Javascript/Typescript logger. Basic right now, just used to share implementation across projects. At some point may be able to store logs instead of just outputting to std{err,out}.

## Usage

```typescript
import Logger from "@noahvarghese/logger";

// Typically set in a .env file, on deployment, or within CI
process.env["LOG_LEVEL"] = 1;

/**
 * Environment variable options that enable at most the preceding and current corresponding functions
 * for the values starting at 0 increasing by 1 each time
 *
 * enum LogLevels {
 * ERROR,
 * TEST,
 * WARN,
 * DEBUG,
 * LOG,
 * CMD,
 * SQL
 * }
 *
 */

// Can override environment and turn off all logs by passing true to the init function
const disableLogs = false;

// Required to load environment variable into class
Logs.init(disableLogs);
```

## Development - Getting Started

```bash
git clone https://github.com/noahvarghese/logger
cd ./logger
npm i
npm run init
```
