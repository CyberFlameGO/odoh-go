# odoh-go

[![Coverage Status](https://coveralls.io/repos/github/cloudflare/odoh-go/badge.svg?branch=master)](https://coveralls.io/github/cloudflare/odoh-go?branch=master)
[![GoDoc](https://godoc.org/github.com/cloudflare/odoh-go?status.svg)](https://godoc.org/github.com/cloudflare/odoh-go)

This library implements version 0x0001 of [Oblivious DoH](https://tfpauly.github.io/draft-pauly-adaptive-dns-privacy/draft-pauly-dprive-oblivious-doh.html). It is based on the original implementation [available here](https://github.com/chris-wood/odoh).

![protocol overview](odoh-flow.png)

## Test vector generation

To generate test vectors, run:

```
$ ODOH_TEST_VECTORS_OUT=test-vectors.json go test -v -run TestVectorGenerate
```

To check test vectors, run:

```
$ ODOH_TEST_VECTORS_IN=test-vectors.json go test -v -run TestVectorVerify
```
