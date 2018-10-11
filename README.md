

# Welcome to the Javascript Team <img width="40" height="40" src="https://github.com/toti1911/test/blob/master/js.png">

Welcome to AXA Bcn Javascript Team! :raised_hands: You‘re about to become part of a world-class team of software engineering experts.
Innovation lies at the heart of our culture and we need your talent and expertise to stay ahead of the curve.
We would like this to be a zone of sharing and consulting where all the collaborators can solve their doubts about
how we are working as a team and some knowledge about the different projects that we are working on.

Also we would like to share knowledge through **code examples** and **best practises** so everyone can improve.

1. [ Dev tools :wrench: ](#desc)
2. [ Code Style guide :pencil:](#style)
3. [ Commits & Branchs :eyes:](#commits)
4. [ Proxy :gun:](#proxy)
5. [ AXA Libraries & Projects :notebook:](#projects)
6. [ OpenPaaS :rocket:](#openpaas)
7. [ Collaborators :muscle: ](#collaborators)

<a name="desc"></a>
## Getting started
<img src="https://media.giphy.com/media/oS8pRFxbD0d44/giphy.gif" width="200" height="150" />

:one: The first thing you should do is consult the section [Accounts](./docs/accounts.md) to be sure that you will have all the permissions that you need to continue.

### Development tools and workstation setup :wrench:

- :heavy_check_mark: Install **Nose.js** [Download](https://nodejs.org/en/download/)
- :heavy_check_mark: Install **NVM** [Download](https://github.com/creationix/nvm) in order to be able to switch between NodeJS versions.
- :heavy_check_mark: Configure **NPM** Private repository access: [Guide](https://axagroupsolutions.atlassian.net/wiki/display/AGSD/Using+Artifactory+as+NPM+private+registry)

#### Test environment:

```bash
git clone https://github.com/AXA-GROUP-SOLUTIONS/amf-commons-node.git
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
+ Configure **eslint** hook. [Guide](https://axagroupsolutions.atlassian.net/wiki/display/AGSD/HOW+TO+Configure+ESLint+in+GIT+hook)
+ **conEmu**:  Windows console emulator with tabs [Download](https://sourceforge.net/projects/conemu/)
+ **Robomongo**: Native and cross-platform MongoDB manager [Download](https://robomongo.org/download)

<a name="style"></a>
### Code guide style

<img src="https://media.giphy.com/media/QHE5gWI0QjqF2/giphy.gif" width="200" height="150" />

:star: [Eslint](http://eslint.org/)

:star: [javascript airbnb styleguide](https://github.com/airbnb/javascript)

:star: [Tslint](https://palantir.github.io/tslint/)

:star: [typescript airbnb styleguide](https://www.npmjs.com/package/tslint-config-airbnb)

**Want more?** :blue_book: --> More details about why we should lint our javascript code and our styleguide specs can be found [here](./docs/style.md).

Also, you can see the [AXA France Style Guide](https://github.axa.com/axa-france/af-dev-guidelines).

<a name="commits"></a>
### Commits conventions :computer:

To take advantage of the autogenerator of changelogs, [conventional-changelog](https://github.com/conventional-changelog/conventional-changelog), is need to follow the following conventional commits message format: https://github.com/pvdlg/conventional-changelog-metahub

```
commit -m "feat: the most awesome :shit: feature"
```

You can save time and memory using the next VSCode plugin: https://github.com/KnisterPeter/vscode-commitizen

### Branching strategy 

<img src="https://media.giphy.com/media/cFkiFMDg3iFoI/giphy.gif" width="200" height="150" />

Branching strategy is the way AXA Group Solutions Spain will use GIT for managing the lifecycle of the source code.
Also the branching strategy is aligned with the CI platform tasks in order to manage release generation.

You can find the current branching strategy [here](https://axagroupsolutions.atlassian.net/wiki/display/AGSD/Branching+strategy+and+CI)

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
### AXA libraries

+ [amf-commons](https://github.com/AXA-GROUP-SOLUTIONS/amf-commons-node)
+ TBC

## Projects

Check [our projects list](./docs/projects.md) out.

<a name="openpaas"></a>
## OpenPaaS

Check [a list of OpenShift bash scripts to use in your terminal](./scripts/openshift).

<a name="collaborators"></a>
## Collaborators

| Name                      | Github account |  Email                                        | Current project |
|---------------------------|----------------|-----------------------------------------------|-----------------|
| :woman:Beatriz Martín de Juan    | [bmdjuan](https://github.com/bmdjuan) | beatriz.martin@axa-groupsolutions.com    | IceBox |
| :man:Luis Prieto Fernández     | [luisprieto-sp](https://github.com/luisprieto-sp) | luis.prieto.sopra@axa-groupsolutions.com | AUTO Bot |
| :man:Artem Pasichnyk           | [artemidas](https://github.com/artemidas) | artem.pasichnyk.amaris@axa-groupsolutions.com  | OpenPass |
| :woman:Silvia de León            | [sleongonzalez](https://github.com/sleongonzalez) | silvia.leon.sopra@axa-groupsolutions.com | MyAXA |
| :man:Oriol Homedes del Barrio  | [oriol-homedes](https://github.com/oriol-homedes) | oriol.homedes.pasiona@axa-groupsolutions.com | AXA France Websites (Live, HR, Prevention, Mediazone, Newstoprotect) |
| :man:Fran Herrero Pérez        | [franher](https://github.com/franher) | francisco.herrero@axa-groupsolutions.com | Mobile Backend & MANA |
| :man:Jose Lara de Lamo         | [jose-lara](https://github.com/jose-lara) | jose.lara.sopra@axa-groupsolutions.com | Reparadores Bot |
| :man:F. Javier Romero Yesares  | [fromeroy](https://github.com/fromeroy) | francisco.romero.altran@axa-groupsolutions.com | EB Partners |
| :man:Santi Pérez  | [santiago-perez](https://github.com/santiago-perez) | santiago.perez.altran@axa-groupsolutions.com | MyAXA |
| :man:Javier Blanco Martinez    | [javierblancosp](https://github.com/javierblancosp) | javier.blanco@axa-groupsolutions.com | Mobile Backend & MANA |
| :man:Xavier Redondo Bolet      | [Xavier-Redondo](https://github.com/Xavier-Redondo) | xavier.redondo@axa-groupsolutions.com | AXA Home |
| :man:Jesús Seijas              | [jesus-seijas](https://github.axa.com/jesus-seijas) | jesus.seijas@axa-groupsolutions.com |     |
| :woman:Francisca Calabria | [FCalabria](https://github.com/FCalabria) | francisca.calabria@axa-groupsolutions.com    | AXA Advice (Berater) |
| :man:Iván Megías | [Ivan-megias](https://github.com/ivan-megias) | ivan.megias.altran@axa-groupsolutions.com  | EB Partners |
| :man:Martín Palmieri | [Martin-palmieri](https://github.com/martin-palmieri) | martin.palmieri.amaris@axa-groupsolutions.com  | EB Partners |
| :woman:Ana Gamito | [Ana-gamito](https://github.com/ana-gamito) | ana.gamito@axa.com  | AXA LIVE - HR |
| :woman:Andrea Martins   | [martinsandrea](https://github.com/martinsandrea) | andrea.martins.altran@axa-groupsolutions.com    | AxaLive |
| :man:Eric Lara   | [eric-lara-altran](https://github.com/eric-lara-altran) | eric.lara.altran@axa-groupsolutions.com    | OpenPass |

