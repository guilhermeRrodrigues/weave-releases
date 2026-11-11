# Weave

Este repositório publica os binários do Weave e o feed de atualização dos apps. O código-fonte não fica aqui.

O Weave compartilha um mouse e um teclado entre computadores Mac e Windows na mesma rede. A área de transferência e os arquivos vão junto. No celular, o app vira trackpad e teclado do computador, mostra a tela dele e manda arquivos.

## Instalação

Baixe os arquivos da [última versão](../../releases/latest) e confira o `SHA256SUMS` da release.

| Plataforma | Arquivo | Requisitos | Observações |
|---|---|---|---|
| macOS | `Weave-<versão>-macos-arm64.dmg` ou `.zip` | macOS 14 ou mais novo, Apple Silicon | Arraste o Weave para Aplicativos. O app não é notarizado: na primeira vez, abra em Ajustes do Sistema → Privacidade e Segurança → "Abrir mesmo assim". Depois ele pede Acessibilidade e Monitoramento de Entrada. |
| Windows | `Weave-<versão>-windows-x64-setup.exe` | Windows 10 ou 11, x64 | O instalador não é assinado: na tela do SmartScreen, clique em "Mais informações" → "Executar assim mesmo". |
| Android | `Weave-<versão>-android.apk` | Android 8.0 ou mais novo | O Android pede permissão para instalar apps desta origem. |
| iPhone | — | — | Ainda não há distribuição pública. O app avisa quando sai uma versão nova. |

## Atualizações

Os apps de Mac, Windows e Android procuram versões novas sozinhos, no arquivo `weave-update.json` da última release. Esse arquivo é assinado (Ed25519) e cada pacote é conferido pelo SHA-256 antes de ser instalado: um arquivo adulterado ou uma versão mais antiga são recusados. Depois da atualização, o app mostra o que mudou.

As releases deste repositório são imutáveis depois de publicadas.

## Licença

MIT ou Apache-2.0, à sua escolha (`LICENSE-MIT`, `LICENSE-APACHE`).

---

## English

This repository hosts Weave's binaries and the apps' update feed. The source code is not here.

Weave shares one mouse and keyboard between Mac and Windows computers on the same network, along with the clipboard and files. On a phone, the app becomes the computer's trackpad and keyboard, shows its screen and sends files.

Download from the [latest release](../../releases/latest) and check its `SHA256SUMS`:

| Platform | File | Requirements | Notes |
|---|---|---|---|
| macOS | `.dmg` or `.zip` | macOS 14+, Apple Silicon | Not notarized: the first time, open it from System Settings → Privacy & Security → "Open Anyway". |
| Windows | `-setup.exe` | Windows 10/11 x64 | Unsigned: on the SmartScreen prompt, click "More info" → "Run anyway". |
| Android | `.apk` | Android 8.0+ | Android asks for permission to install apps from this source. |

The Mac, Windows and Android apps update themselves from the signed `weave-update.json` of the latest release. Every package is checked against its SHA-256 before install. Releases are immutable once published.

License: MIT or Apache-2.0, at your option.
