# Meet Cryptfire

We are providing a Transak-driven CEX and Swap for Bitcoin, Ethereum, Lyra and Utopia. We run a Blockchain network executing WASM compiled smart contracts as well as Serverless functions and JSLinux Virtual Machines.

💵 See [Wiki](https://github.com/cryptfire/.github/wiki/Cryptfire-Pricing) for Pricing. 

✅ Utilize our open source code base for highest expectations and great design. [Github](https://github.com/cryptfire/cryptfire)

❗ [Commerical API](https://github.com/cryptfire/.github/wiki/Commerical-API) currently under active developmemt. 

## 🚀 Install CLI

```
npm install @cryptfire/cli -g
cryptfire --health;
```

## 🚀 Join

In order to build with us, you'll need a free API Key:

```
cryptfire --register --email your@email.com;
cryptfire --confirm;
```

Or

```
curl -X POST \
     -H "Content-Type: application/json" \
     -d '{"phone": "[YOUR_PHONE]"}' \
     https://api.cryptfire.io/keygen/phone
```

Or simply for an interactive shell

`curl https://install.cryptfire.io | sh` 

 🔥 Once it was granted, export it on shell
`export CRYPTFIRE_API=...` ⬇️

<br />

![logo](https://github.com/cryptfire/.github/assets/114028070/f3f3cdb9-268d-478a-b716-c232446ed5e1)

## Deploy your first Infrastructure

In order to set up your Cryptfire Capsules for testing and later production scaling, you only need one line.
This will set up multiple cost-effective cloud servers for development purposes. You need a domain to get started.
We recommend Namecheap.

The development capsules shouldn't be used for production, as they aren't performant, nor are they clean for security
after playing around for while. Set up a fresh, optimized, production cluster:

```
curl -X POST \
     -H "Content-Type: application/json" \
     -d '{"api_key": "[YOUR_API_KEY]", "type": "dev", "domain": "[YOUR_DOMAIN]}' \
     https://api.cryptfire.io/deploy/compute
```

## Deploy from staging to production 

Let's scale up to Bare Metal:

```
curl -X POST \
     -H "Content-Type: application/json" \
     -d '{"api_key": "[YOUR_API_KEY]", "type": "prod", "domain": "[YOUR_DOMAIN]}' \
     https://api.cryptfire.io/deploy/compute
```

This will spawn a Bare Metal server and set DNS entries for domain.

Or simply for an interactive shell

```
curl https://api.cryptfire.io/deploy | sh
```

## Premium

Everything you have seen so far is provided free, given that you're paying for domain and cloud servers / bare metal yourself.
If you *prefer* to host with us however, you can do that too.

```
curl -X POST \
     -H "Content-Type: application/json" \
     -d '{"api_key": "[YOUR_API_KEY]"}' \
     https://api.cryptfire.io/premium/upgrade

# wait for email

curl -X POST \
     -H "Content-Type: application/json" \
     -d '{"api_key": "[YOUR_API_KEY]", "code": "[CONFIRM_CODE]"}' \
     https://api.cryptfire.io/premium/verify
```

### Fund your wallet

In order to deploy, you need at least one month worth of dev compute in your wallet. Your wallet address was posted to you
upon API key retrieval, but you can always fetch it

```
curl -X POST \
     -H "Content-Type: application/json" \
     -d '{"api_key": "[YOUR_API_KEY]"}' \
     https://api.cryptfire.io/wallet
```

As soon as one confirmation on Ethereum mainnet was mined, please trigger manually or wait until our cron job fetches it.

```
curl -X POST \
     -H "Content-Type: application/json" \
     -d '{"api_key": "[YOUR_API_KEY]", "type": "dev"}' \
     https://api.cryptfire.io/wallet/signal
```

It is increasingly hard to obtain a [Transak](https://transak.com/) API Key so if you need a way to buy Ethereum with your
Credit card or Bank account, [MoonPay](https://www.moonpay.com/en-gb/buy) is very reasonable these days.

## Maintainers

Cryptfire is maintained and is being operated by [@zdanl](https://github.com/zdanl)

## Copyright

The code base is licensed under the GNU v3 General Public License.
