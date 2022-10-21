# k6-playground

## Setup

```bash
brew install k6
```

## Usage

<https://k6.io/docs/getting-started/running-k6/>

```bash
k6 run --vus 10 --duration 30s --out csv=test_results.gz script.js
```

## Dashboard

Note: half working

```bash
# setup
go install go.k6.io/xk6/cmd/xk6@latest
xk6 build --with github.com/szkiba/xk6-dashboard@latest

# run
./k6 run --vus 10 --duration 30s --out dashboard script.js # http://127.0.0.1:5665
```
