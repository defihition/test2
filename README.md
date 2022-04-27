# hello-package

Github Package Registry에 패키지 올려보기

## Install

0. PAT 발급

> https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-npm-registry#authenticating-to-github-packages

- https://github.com/settings/tokens/new
- `read:packages` 체크

1. package.json과 같은 위치에 **.npmrc** 생성 후 아래 내용 저장

```.npmrc .npmrc
//npm.pkg.github.com/:_authToken=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
@chinsun9:registry=https://npm.pkg.github.com/
```

- 개인 토큰 넣어주기

2. `yarn add @chinsun9/hello-package`
