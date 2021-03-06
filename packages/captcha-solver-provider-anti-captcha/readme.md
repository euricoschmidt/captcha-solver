# captcha-solver-provider-anti-captcha

> Captcha solver provider for the [anti-captcha](https://anti-captcha.com) service.

[![NPM](https://img.shields.io/npm/v/captcha-solver-provider-anti-captcha.svg)](https://www.npmjs.com/package/captcha-solver-provider-anti-captcha) [![Build Status](https://travis-ci.com/transitive-bullshit/captcha-solver.svg?branch=master)](https://travis-ci.com/transitive-bullshit/captcha-solver) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

<p align="center">
  <a href="https://anti-captcha.com"><img src="https://anti-captcha.com/images/mainpage/herofront_nocape.png" alt="Anticaptcha Logo"></a>
</p>

## Install

This module requires `node >= 8`.

```bash
npm install --save captcha-solver-provider-anti-captcha
```

## API

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

#### Table of Contents

-   [CaptchaSolverProviderAntiCaptcha](#captchasolverprovideranticaptcha)
    -   [name](#name)
    -   [supportedTaskTypes](#supportedtasktypes)
    -   [createTask](#createtask)
    -   [getTaskResult](#gettaskresult)

### [CaptchaSolverProviderAntiCaptcha](https://github.com/transitive-bullshit/captcha-solver/blob/ec5e0649a40d0489264905d80a991f071703fce2/packages/captcha-solver-provider-anti-captcha/index.js#L28-L183)

**Extends: CaptchaSolverProvider**

Captcha solver provider for the anti-captcha service.

Type: `function (opts)`

-   `opts` **[object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object)** Options
    -   `opts.key` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** Client key.

* * *

#### [name](https://github.com/transitive-bullshit/captcha-solver/blob/ec5e0649a40d0489264905d80a991f071703fce2/packages/captcha-solver-provider-anti-captcha/index.js#L43-L45)

Provider name.

Type: [string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)

* * *

#### [supportedTaskTypes](https://github.com/transitive-bullshit/captcha-solver/blob/ec5e0649a40d0489264905d80a991f071703fce2/packages/captcha-solver-provider-anti-captcha/index.js#L52-L54)

Set containing task types supported by this provider.

Type: [Set](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Set)&lt;[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)>

* * *

#### [createTask](https://github.com/transitive-bullshit/captcha-solver/blob/ec5e0649a40d0489264905d80a991f071703fce2/packages/captcha-solver-provider-anti-captcha/index.js#L76-L154)

Creates a new captcha solving task.

Type: `function (opts)`

-   `opts` **[object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object)** Options
    -   `opts.type` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** Type of captcha to solve
    -   `opts.image` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)?** Captcha image to process encoded as a base64 string
    -   `opts.websiteURL` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)?** Website URL for nocaptcha, recaptcha, and funcaptcha
    -   `opts.websiteKey` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)?** Recaptcha website key
    -   `opts.websiteSToken` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)?** Secret token for old versions of Recaptcha
    -   `opts.websitePublicKey` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)?** Funcaptcha public key
    -   `opts.proxyType` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)?** Proxy type (http/socks4/socks5)
    -   `opts.proxyAddress` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)?** Proxy IP address (ipv4/ipv6)
    -   `opts.proxyPort` **([string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String) \| [number](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Number))?** Proxy port
    -   `opts.proxyLogin` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)?** Proxy login for basic auth
    -   `opts.proxyPassword` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)?** Proxy password
    -   `opts.userAgent` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)?** Browser's User-Agent to emulate
    -   `opts.cookies` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)?** Additional cookies to emulate

* * *

#### [getTaskResult](https://github.com/transitive-bullshit/captcha-solver/blob/ec5e0649a40d0489264905d80a991f071703fce2/packages/captcha-solver-provider-anti-captcha/index.js#L163-L182)

Fetches the result of a previously created captcha solving task.

Type: `function (taskId)`

-   `taskId` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** Unique task identifier

* * *

## Related

-   [captcha-solver](https://github.com/transitive-bullshit/captcha-solver) - Facilitates the automation of CAPTCHA verification.
-   [anti-captcha API docs](https://anticaptcha.atlassian.net/wiki/spaces/API/overview) - Anticaptcha v2 API docs.

## Disclaimer

Using this software to violate the terms and conditions of any third-party service is strictly against the intent of this software. By using this software, you are acknowledging this fact and absolving the author or any potential liability or wrongdoing it may cause. This software is meant for testing and experimental purposes only, so please act responsibly.

## License

MIT © [Travis Fischer](https://github.com/transitive-bullshit)
