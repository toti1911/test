

# Welcome to the Javascript Team <img width="40" height="40" src="https://github.com/toti1911/test/blob/master/js.png">

Welcome to Bcn Javascript Team! :raised_hands: You‘re about to become part of a world-class team of software engineering experts.
Innovation lies at the heart of our culture and we need your talent and expertise to stay ahead of the curve.
We would like this to be a zone of sharing and consulting where all the collaborators can solve their doubts about
how we are working as a team and some knowledge about the different projects that we are working on.

Also we would like to share knowledge through **code examples** and **best practises** so everyone can improve.

1. [ Dev tools :wrench: ](#desc)
2. [ Code Style guide :pencil:](#style)
3. [ Commits & Branchs :eyes:](#commits)
4. [ Proxy :gun:](#proxy)
5. [ OpenPaaS :rocket:](#openpaas)
6
. [ Collaborators :muscle: ](#collaborators)

<a name="desc"></a>
## Getting started
<img src="https://media.giphy.com/media/oS8pRFxbD0d44/giphy.gif" width="200" height="150" />

:one: The first thing you should do is consult the section [Accounts](./docs/accounts.md) to be sure that you will have all the permissions that you need to continue.

### Development tools and workstation setup :wrench:

- :heavy_check_mark: Install **Nose.js** [Download](https://nodejs.org/en/download/)
- :heavy_check_mark: Install **NVM** [Download](https://github.com/creationix/nvm) in order to be able to switch between NodeJS versions.
- :heavy_check_mark: Configure **NPM** Private repository access: [Guide](https://google.com)

#### Test environment:

```bash
git clone https://github.com/test-commons-node.git
cd amf-commons-node.git
npm install
```

+ Install **MongoDB** [Guide](https://docs.mongodb.com/v3.2/administration/install-community/)
+ Setup **Windows 10 for Modern/Hipster Development** [Guide](https://github.com/felixrieseberg/windows-development-environment)

### Allowed tools :hammer:

#### IDEs
+ **Visual Studio Code** [Download](https://code.visualstudio.com/)

Any other tool is not allowed (for example Sublime text)

Alternative:
+ Webstorm: Javascript IDE (we have licenses, please ask for it) [Download](https://www.jetbrains.com/webstorm/download/)(ask for your license to Service Desk)


### Communication :speech_balloon:

+ **Slack** [Download] (https://slack.com/downloads/osx)
+ **Lync**

### other recommended tools :top:

+ **SourceTree**: Git client [Download](https://www.sourcetreeapp.com/)
+ Configure **eslint** hook. [Guide](https://google.com)
+ **conEmu**:  Windows console emulator with tabs [Download](https://sourceforge.net/projects/conemu/)
+ **Robomongo**: Native and cross-platform MongoDB manager [Download](https://robomongo.org/download)

<a name="style"></a>
### Code guide style

<img src="https://media.giphy.com/media/3o7qE1YN7aBOFPRw8E/giphy.gif" width="200" height="150" />

:star: [Eslint](http://eslint.org/)

:star: [javascript airbnb styleguide](https://github.com/airbnb/javascript)

:star: [Tslint](https://palantir.github.io/tslint/)

:star: [typescript airbnb styleguide](https://www.npmjs.com/package/tslint-config-airbnb)

**Want more?** :blue_book: --> More details about why we should lint our javascript code and our styleguide specs can be found [here](./docs/style.md).

Also, you can see the [Style Guide](https://google.com).

<a name="commits"></a>
### Commits conventions :computer:

To take advantage of the autogenerator of changelogs, [conventional-changelog](https://github.com/conventional-changelog/conventional-changelog), is need to follow the following conventional commits message format: https://github.com/pvdlg/conventional-changelog-metahub

```
commit -m "feat: the most awesome :shit: feature"
```

You can save time and memory using the next VSCode plugin: https://github.com/KnisterPeter/vscode-commitizen

### Branching strategy 

<img src="https://media.giphy.com/media/cFkiFMDg3iFoI/giphy.gif" width="200" height="150" />

Branching strategy is the way will use GIT for managing the lifecycle of the source code.
Also the branching strategy is aligned with the CI platform tasks in order to manage release generation.

You can find the current branching strategy [here](https://google.com)

:warning: **Remember that all the teams has to follow this strategy**

<a name="proxy"></a>
### Proxy :gun:

Main proxy to be configured in your machine:

+ 192.168.62.5
+ 192.168.62.4


Most of the issues are related the proxy usage. ALL of those commands have a http-proxy option that you must use
in order to redirect all the traffic though our proxy.

For automated set up of the proxy see [resources/proxy-scripts](./resources/proxy-scripts)

#### Git proxy config

```bash
HTTP_PROXY=http://192.168.62.5:3128
HTTPS_PROXY=http://192.168.62.5:3128
git config --global http.proxy $HTTP_PROXY
git config --global https.proxy $HTTPS_PROXY
```

#### Brew install

```bash
ALL_PROXY=http://192.168.62.5:3128 brew install <name>
```

#### Gem install

```bash
sudo gem install --http-proxy http://192.168.62.5:3128 --https-proxy https://192.168.62.5:3128 <gema>
```
### JavaScript transpilers/compilers

+ Babel
+ TypeScript

<a name="desc"></a>

## Projects

Check [our projects list](./docs/projects.md) out.

<a name="openpaas"></a>
## OpenPaaS

Check [a list of OpenShift bash scripts to use in your terminal](./scripts/openshift).

