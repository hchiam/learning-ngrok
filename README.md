# Learning ngrok

Just one of the things I'm learning. https://github.com/hchiam/learning

Exposes your localhost to the web with a random URL. Consider using it only for projects where the project and data are already open-sourced. Otherwise consider [USB-connected port forwarding](https://developer.chrome.com/docs/devtools/remote-debugging/local-server/#port-forwarding) to do [remote debugging](https://developer.chrome.com/docs/devtools/remote-debugging/).

https://ngrok.com/

https://github.com/bubenshchykov/ngrok

it's now closed-source and commercial: https://dashboard.ngrok.com/get-started/setup
- (note to self: update to be able to use now)

```sh
npm install ngrok --global
```

or with [`yarn`](https://github.com/hchiam/learning-yarn):

```sh
yarn global add ngrok
```

then: create and account and copy the command that looks like `ngrok config add-authtoken .......`

then:

```sh
ngrok http 3000
# or #### for whatever port your localhost:#### is
```

## demo

You'll need an account set up.

```sh
yarn; yarn global add ngrok parcel-bundler; parcel index.html --open;
```

```sh
cd learning-ngrok; ngrok http 1234
# copy the "Forwarding" HTTPS URL
```

## more

https://ngrok.com/docs/start

for example:

- https://ngrok.com/docs/traffic-policy/actions/oauth
- https://dashboard.ngrok.com/traffic-inspector
- https://ngrok.com/docs/agent/web-inspection-interface
- https://dashboard.ngrok.com/log-exporting for observability
