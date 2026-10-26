# Manual Test Page

> Use this page to test the extension. Open it on GitHub.

[Switch to localhost](?_socket_dev)

## Gem

```sh
gem install rails sinatra
gem fetch rails sinatra
```

Invalid package names

```sh
gem install gem!pkg
```

## Go

```sh
go get -u github.com/go-chi/chi/v5
```

## NPM

Inline code

- `npm install lodash`
- foo `npm install axios` bar

Block code without formatting

```sh
npm install tslib
```

Block code with formatting (without breaking syntax highlighting)

```shell
# Comments should appear in gray
npm install chalk # Comment
# Comment
```

Separators

```sh
npm install commander && npm install express
npm install inquirer; npm install vue
```

Multiple packages

```sh
npm install vue pinia
```

Multiple packages with common prefix

```sh
npm install react react-dom
```

CLI options

```sh
npm install -D typescript
npm install remix --production=false
```

<details>
<summary><b>Scopes, versions, aliases, and edge cases</b> - the rest of the npm matrix</summary>

Package scope

```sh
npm install @koa/router
```

Package version

```sh
npm install express@5.0.0-beta.1
```

Package scope with version

```sh
npm install @koa/router
npm install @koa/router@11.0.2
```

Aliases

```sh
npm i bootstrap
npm add preact
```

Other package managers

```sh
pnpm add react-colorful
yarn add yo
bun add elysia
```

Same package should not result in multiple requests

```sh
npm install docusaurus docusaurus docusaurus docusaurus
npm install docusaurus docusaurus docusaurus docusaurus
npm install docusaurus docusaurus docusaurus docusaurus
npm install docusaurus docusaurus docusaurus docusaurus
```

Unknown package

```sh
npm install egldvxjvsdikngtvhyyrymyhhfnmzd
```

Unknown version

```sh
npm install react@9001
```

Package with many alerts

```sh
npm install bowserify
```

Invalid package names

```sh
npm install .npmpkg _npmpkg scope/npmpkg @scope
```

</details>

## Nuget

```sh
dotnet add package Azure.Core
```

## PyPI

```sh
pip install numpy
pip install numpy==1.25.2
```

<details>
<summary><b>Other Python installers</b> - pip2, pip3, pipx, conda, pdm, poetry, and invalid names</summary>

```sh
pip2 install numpy
```

```sh
pip3 install numpy
```

```sh
pipx install pycowsay
```

```sh
conda install matplotlib
```

```sh
pdm add django
```

```sh
poetry add requests
```

Invalid package names

```sh
pip install py!pkg
```

</details>

## PURL support

Text

- some text pkg:maven/org.springframework/spring-core some text
- with version pkg:maven/org.springframework/spring-core@6.1.8

Block code

```shell
# Comment
pkg:maven/org.springframework/spring-core # Comment
# Comment
```

Should ignore non supported PURL:

- pkg:rpm/fedora/curl@7.50.3-1.fc25?arch=i386&distro=fedora-25

## Enhance links to package repositories

Should add popover but not modify existing href, ignore non package URLs and add an outline to badges

Should ignore:

- <https://translate.google.com/translate?u=https://www.npmjs.com/package/express>

### Gem

- <https://rubygems.org/gems/rails>
- <https://rubygems.org/gems/rails/versions/7.0.0>

Should ignore:

- <https://rubygems.org/gems/rails/versions>
- <https://rubygems.org/releases>

### Go

- <https://pkg.go.dev/github.com/go-chi/chi>
- <https://pkg.go.dev/github.com/go-chi/chi@1.5.0>

Should ignore:

- <https://pkg.go.dev/about>

### Maven

- <https://central.sonatype.com/artifact/org.springframework/spring>
- <https://central.sonatype.com/artifact/org.springframework/spring/5.3.36>

Should ignore:

- <https://central.sonatype.org/pages/support/>

### Nuget

- <https://www.nuget.org/packages/Newtonsoft.Json>
- <https://www.nuget.org/packages/Newtonsoft.Json/12.0.1>

Should ignore:

- <https://www.nuget.org/blahblah>

### NPM

- <https://npmjs.com/package/express>
  - <https://npmjs.org/package/express> (old domain))
- <https://www.npmjs.com/package/express/v/5.0.0-beta.3>

Should ignore:

- <https://npmjs.com/about>

### PyPI

- <https://pypi.org/project/torch>
- <https://pypi.org/project/torch/2.2.0/>

Should ignore:

- <https://pypi.org/help>

## 404

Unknown version

- `npm i express@100`
- <https://npmjs.com/package/express/v/100>
- pkg:npm/express@100

Unknown name

- `npm i foo-940f8e03a16e`
- <https://npmjs.com/package/foo-940f8e03a16e>
- pkg:npm/foo-940f8e03a16e

## Dark mode

Switch to dark mode.

## SPA support

Navigate to another page, then go back.
