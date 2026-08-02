# JirauLog 3.1 — Web/PWA

Esta versão mantém a interface Operator e adiciona suporte estrutural à Web/PWA.

## Executar no navegador

```bash
flutter pub get
dart run sqflite_common_ffi_web:setup
flutter run -d chrome --web-port 8080
```

Use sempre a mesma porta durante os testes para preservar o banco local do navegador.

## Gerar versão para publicação

```bash
flutter build web --release
```

A saída ficará em `build/web` e pode ser publicada em serviços como Firebase Hosting, Cloudflare Pages ou servidor próprio.

## Armazenamento

Na versão web, o SQLite é persistido no IndexedDB do navegador. Os dados ficam vinculados ao domínio e à porta usados. A versão desktop/Android continua usando o arquivo SQLite local.

## Instalação como aplicativo

Depois de publicada em HTTPS, a versão web pode ser instalada pelo navegador como PWA. O manifesto, ícones e identidade visual Jirau já estão incluídos.

## Limitação atual

Backup/restauração de arquivo `.db` continua disponível em desktop/Android. No navegador, os dados são salvos automaticamente no armazenamento local; exportação/restauração completa da base web deve ser implementada em formato portátil (JSON/ZIP) antes do uso corporativo definitivo.
