# stable-diffusion-webuiのAPIを試す

# 事前準備

## stable-diffusion-webuiをセットアップする
http://127.0.0.1:7860/docs<br>
ブラウザで動くことを確認する。

## APIを有効にする
webui-user.sh（またはwebui-user.bat）を編集

`COMMANDLINE_ARGS`に`--api`を設定し、実行し直す。<br>
macの場合は`./run_webui_mac.sh --api`

<br>
http://127.0.0.1:7860/sdapi/v1/txt2img<br>
を確認する（正しくないので"Method Not Allowed"のエラーが返る）

## インストール
```bash
npm i
```

## デバッグ実行

```bash
npm run dev
```

http://localhost:3000/sdapi/v1/txt2img<br>
"Method Not Allowed"が返ることを確認する。

http://localhost:3000 へアクセス
