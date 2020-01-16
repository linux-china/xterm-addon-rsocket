## xterm-addon-rsocket

An addon for [xterm.js](https://github.com/xtermjs/xterm.js) that enables attaching to a rsocket. This addon requires xterm.js v4+.

### Install

```bash
npm install --save xterm-addon-rsocket
```

### Usage

```ts
import { Terminal } from 'xterm';
import { RSocketAddon } from 'xterm-addon-rsocket';

const term = new Terminal();
const rsocketAddon = new RSocketAddon('ws://localhost:8080/rsocket');

// Attach the rsocket to term
term.loadAddon(rsocketAddon);
```

# References

* RSocket: http://rsocket.io
* Spring Boot RSocket: https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#boot-features-rsocket
