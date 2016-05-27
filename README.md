# Partiu

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](http://choosealicense.com/licenses/mit/)
[![Code Climate](https://codeclimate.com/github/mdsgpp2016/frontend/badges/gpa.svg)](https://codeclimate.com/github/mdsgpp2016/frontend)
[![Build Status](https://circleci.com/gh/mdsgpp2016/frontend.svg?style=shield)](https://circleci.com/gh/mdsgpp2016/frontend)

Aplicativo multiplataforma que permite pessoas com amigos em comum combinarem caronas.

## Dependências

- Node.js (v5.9.0)
  - Recomendamos a utilização do [NVM](https://github.com/creationix/nvm)

## Ambiente de Desenvolvimento

Na raiz do repositório, execute:

```
 $ npm install
 $ npm install -g cordova ionic
 $ ionic serve --lab
```

## Executando os Testes

```
npm test
```

O resultado da cobertura de testes gerado após a execução dos testes encontra-se em: coverage/lcov-report/index.html

### Build de desenvolvimento Android

#### Pré-requisitos

- JDK (v8)
- Android SDK
- ADB
- Celular Android com "USB debugging" ativado e conectado ao PC
  - Verifique se o celular foi reconhecido pelo adb com o comando **adb devices**

#### Gerando a build e instalando

```
 $ ionic build android
 $ adb install -r platforms/android/build/outputs/apk/android-debug.apk
```