# WebStream CENC-Player SDK <br /> ExoPlayer Guide

この文書は以下の情報を示す事を主たる目的として作成されました。

- ExoPlayer の概要
- ExoPlayer ウェブサイトの各種情報の案内
- WebStream ライセンスサービスの利用


## ExoPlayer Home

ExoPlayer - Home  
https://google.github.io/ExoPlayer/

上記ページの序文を意訳して、ExoPlayer をご紹介します。

> ExoPlayer はアプリケーションレベルのメディアプレーヤーです。
> ローカルまたはインターネット経由でオーディオやビデオを再生する場合、
> Android の MediaPlayer API の代替案を ExoPlayer が提供します。
> 現状の Android の MediaPlayer API が対応していない機能に ExoPlayer は対応しています。
> それは DASH や SmoothStreaming のアダプティブな再生です。
> MediaPlayer API とは違って、
> ExoPlayer はカスタマイズや拡張が容易で、
> Play Store のアプリケーション配布機構を通じて更新可能です。


## ExoPlayer Links

ExoPlayer ウェブサイトでは様々な情報が提供されています。
幾つかのリンクをご案内します。

- 開発ガイド  
    ExoPlayer - Developer guide  
    https://google.github.io/ExoPlayer/guide.html
- デモアプリ  
    ExoPlayer - Demo application  
    https://google.github.io/ExoPlayer/demo-application.html
- 対応メディア形式  
    ExoPlayer - Supported formats  
    https://google.github.io/ExoPlayer/supported-formats.html
- 対応デバイス  
    ExoPlayer - Supported devices  
    https://google.github.io/ExoPlayer/supported-devices.html
- よくある質問  
    ExoPlayer - FAQs  
    https://google.github.io/ExoPlayer/faqs.html
- API リファレンス  
    Overview (ExoPlayer library)  
    http://google.github.io/ExoPlayer/doc/reference/


## ExoPlayer Versions

ExoPlayer には新旧のバージョンが存在します。

- 新バージョン  
    Version number: 2.x  
    Developer guide: https://google.github.io/ExoPlayer/guide.html  
    Source code: https://github.com/google/ExoPlayer  

- 旧バージョン  
    Version number: 1.x  
    Developer guide: https://google.github.io/ExoPlayer/guide-v1.html  
    Source code: https://github.com/google/ExoPlayer/tree/release-v1  

ExoPlayer 2.x へのメジャー番号更新に伴うアーキテクチャー変更や新機能、
そして多くのバグ修正については、
リリースノート r2.0.0 の章をご確認ください。  

ExoPlayer/RELEASENOTES.md at release-v2 · google/ExoPlayer  
https://github.com/google/ExoPlayer/blob/release-v2/RELEASENOTES.md#r200
> **r2.0.0**

WebStream CENC-Player SDK では **ExoPlayer 2.x** を対象とした DRM 利用をご案内します。


# DIGITAL RIGHTS MANAGEMENT

ExoPlayer は Digital Rights Managment (DRM) で保護されたコンテンツの再生に対応しています。  
ExoPlayer の DRM 対応については下記の開発ガイドの DRM の章をご確認ください。

ExoPlayer - Developer guide  
https://google.github.io/ExoPlayer/guide.html#digital-rights-management
> **Digital Rights Management**


## Using WebStream License Service

WebStream ライセンスサービスを利用する場合も、
上記の開発ガイドに記載されている汎用的な DRM 処理で対応可能です。
DRM の種類（Widevine または PlayReady）とライセンス発行 URL 、
およびカスタムデータ（必要な場合のみ）をパラメーターとして提供するだけで
WebStream ライセンスサービスに対応できます。

WebStream ライセンスサービスの利用例は
[Samples Guide](../samples/README.md)
をご確認ください。


# ABOUT THIS MANUAL

この文書は WebStream CENC-Player SDK の一部です。  
SDK の概要については
[Introduction and Resources Guide](README.md)
をご確認ください。

|||
|---:|:---|
| Platform | Android |
| Author | WebStream Corporation |
||


## Revision History

この文書の変更履歴です。

| 日付 | 文書 Edition | SDK Version | 内容 |
|:---:|:---:|:---:|:---|
| 2017-03-06 | 1.0 | 2.2 | 初回作成 |
||
