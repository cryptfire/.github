# Meet Cryptfire

We are a providing the self-hosted infrastructure and enrich the code base of superior self-hosted Backend as a Service platforms, your corresponding Frontends, and a Capsule for Benchmarking & Browser Automation Testing, scaling massively. Our goal is to provide web3- & crypto readyness, and serve the needs of traditional web2 apps too. 
Features like Auth (now including SIWE), Databases, Realtime, Mailgun, Twilio, 2FA, etc. are included. Our included Serverless stack is excellent. Most importantly, you do not need to develop locally anymore, but can do it public/live for cheap, then, scale up to production. __You have root access to your infrastructure at all teams__

Utilize our open source code base for highest expectations and great design. [Github](https://github.com/cryptfire/cryptfire)

## 🚀 Join

In order to build with us, you'll need a free API Key:

```
curl -X POST \
     -H "Content-Type: application/json" \
     -d '{"email": "[YOUR_EMAIL]"}' \
     https://install.cryptfire.io/keygen
```

Or simply

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
     -d '{"api_key": "[YOUR_API_KEY]", "type": "dev"}' \
     https://install.cryptfire.io/deploy/compute
```

Or simply for an interactive shell

```
curl https://install.cryptfire.io/deploy | sh
```

## Premium

Everything you have seen so far is provided free, given that you're payig for domain and cloud servers / bare metal yourself.
If you *prefer* to host with us however, you can do that too.

```
curl -X POST \
     -H "Content-Type: application/json" \
     -d '{"api_key": "[YOUR_API_KEY]"}' \
     https://install.cryptfire.io/premium/upgrade

# wait for email

curl -X POST \
     -H "Content-Type: application/json" \
     -d '{"api_key": "[YOUR_API_KEY]", "code": "[CONFIRM_CODE]"}' \
     https://install.cryptfire.io/premium/verify
```

## Maintainers

Cryptfire is maintained and is being operated by [@zdanl](https://github.com/zdanl)

## Copyright

The code base is licensed under the GNU v3 General Public License.
