# SDK Examples

## Setup
```shell
git clone https://github.com/IvanFarkas/mp_sdk_examples.git
cd mp_sdk_examples
yarn install
yarn install-bundle
```

## Set SDK key
Replace [SdkKey] to the SDK Key in: [/packages/common/src/index.ts](https://github.com/IvanFarkas/mp_sdk_examples/blob/main/packages/common/src/index.ts)

## Overview
- [SDK Examples](#sdk-examples)
  - [Setup](#setup)
  - [Set SDK key](#set-sdk-key)
  - [Overview](#overview)
  - [Prerequisites](#prerequisites)
  - [Setup packages](#setup-packages)
  - [Run the inspector app](#run-the-inspector-app)
  - [Run the virtual staging app](#run-the-virtual-staging-app)
  - [Run the magical bunny app](#run-the-magical-bunny-app)
  - [Run the remote control app](#run-the-remote-control-app)
  - [Clean packages](#clean-packages)
  - [Packages](#packages)
    - [vs-app](#vs-app)
    - [rc-app](#rc-app)
    - [inspector](#inspector)
    - [easter](#easter)
    - [common](#common)
    - [core](#core)
    - [bundle](#bundle)
  - [Useful Links](#useful-links)

## Prerequisites
Your development environment will need node.js and yarn installed.

See <https://nodejs.org/en/> and <https://classic.yarnpkg.com/en/docs/install> for installation instructions specific to your environment.

## Setup packages
Call this to install or update the package dependencies. It also links local packages together.
```shell
yarn bootstrap
```

## Run the inspector app
```shell
yarn inspector
```

## Run the virtual staging app
```shell
yarn vs-app
```

## Run the magical bunny app
```shell
yarn easter
```

## Run the remote control app
```shell
yarn rc-app
```

## Clean packages
You will need to bootstrap after cleaning.
```shell
yarn clean
```

## Packages
The repository is a [Lerna](https://lerna.js.org/) monorepo with the following local packages:

### vs-app
frameworks: [Reactjs](https://reactjs.org/) + [SDK Bundle](https://matterport.github.io/showcase-sdk/sdkbundle_home.html)
- virtual staging
- local webcam
- canvas
- security camera

### rc-app
frameworks: [Reactjs](https://reactjs.org/) + [Photon SDK](https://www.photonengine.com/sdks#sdkrealtimejavascript) + [SDK Embed](https://matterport.github.io/showcase-sdk/sdk_home.html)
- an example that shows how to build a remote controlled showcase

### inspector
frameworks: [Reactjs](https://reactjs.org/) + [RxJS](https://rxjs.dev/) + [SDK Bundle](https://matterport.github.io/showcase-sdk/sdkbundle_home.html)
- object placement using sdk scene files

### easter
frameworks: [Reactjs](https://reactjs.org/) + [Phaser](https://phaser.io/) + [SDK Bundle](https://matterport.github.io/showcase-sdk/sdkbundle_home.html)
  - minigame

### common
- reusable sdk bundle components

### core
- matterport observable library

### bundle
- showcase sdk bundle

## Useful Links

- [SDK Overview](https://matterport.github.io/showcase-sdk/sdkbundle_home.html)
- [Tutorial](https://matterport.github.io/showcase-sdk/sdkbundle_tutorials_setup.html)
- [Examples](https://matterport.github.io/showcase-sdk/sdkbundle_examples_summary.html)
- [Reference](https://matterport.github.io/showcase-sdk/docs/sdkbundle/reference/current/index.html)
- [Scene](https://matterport.github.io/showcase-sdk/docs/sdkbundle/reference/current/modules/scene.html)
