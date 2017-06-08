# Intent Parameters of ExoPlayer Demo Application

ExoPlayer デモアプリの PlayerActivity を起動する Intent について解説します。


## Features

この文書は以下の情報を示す事を主たる目的として作成されました。

- ExoPlayer デモアプリのプレイヤーを用いて独自に動画再生を行うための手引き
- ExoInside demoplayerライブラリを用いたプレイヤーアプリ作成時の手引き

## Intent Parameters
### 必須パラメータ

ExoPlayer のデモアプリならびに、demoplayerライブラリを用いて動画再生を行う際、  
使用するパッケージ、アクティビティ、ならびに必須となる情報は以下の通りです。

|||
|:---:|:---|
| Package | com.google.android.exoplayer2.demo |
| Activity | PlayerActivity |
| ACTION | PlayerActivity.ACTION_VIEW |
| | (com.google.android.exoplayer.demo.action.VIEW) |
| Data | 動画URL |
|||

再生する動画のURLは `intent#setData` で指定します。

### 追加可能なパラメータ

以下は主な追加可能パラメータです。  
`intent#putExtra` を使用し、key-valueの形式で指定します。

|key|Class|value|
|:---:|:---|:---|
|drm_scheme_uuid|String|ライセンス種別|
|drm_license_url|String|ライセンス発行URI|
|||

drm_schme_uuid、およびdrm_license_urlはそれぞれオプショナルな要素ではありますが、  
drm_license_url を指定する場合、 drm_scheme_uuid も必須な要素です。

また、drm_scheme_uuid で指定するべき値は ExoPlayer のライブラリ内に定義されています。  
詳しくは以下のドキュメントから、UUID型のデータをご確認ください。

ExoPlayer Class Reference - C  
http://google.github.io/ExoPlayer/doc/reference/com/google/android/exoplayer2/C.html


その他更に使用可能なパラメータがありますが、  
詳細については以下のドキュメントを参照してください。

ExoPlayer - Developer guide  
https://google.github.io/ExoPlayer/demo-application.html
> **Playing your own content**

# ABOUT THIS MANUAL

この文書は WebStream CENC-Player SDK の一部です。  
SDK の概要については
[Introduction and Resources Guide](../documents/README.md)
をご確認ください。

|||
|---:|:---|
| Platform | Android |
| Author | WebStream Corporation |
|||


## Revision History

| 日付 | 文書 Edition | SDK Version | 内容 |
|:---:|:---:|:---:|:---|
| 2017-03-06 | 1.0 | 2.2 | 初回作成 |
||
