# send_discord
ターミナル上からDiscordに文字を送る

## インストール

```bash
curl https://raw.githubusercontent.com/suzakutakumi/send_discord/main/install.sh|sudo bash
```

上記のコマンドによってインストールできる

## 使い方

1. DiscordのWebhookのURLをコピーします
![image](https://user-images.githubusercontent.com/71514776/127080720-0ae06895-9077-48d7-88c8-a0c5b5f5d5ea.png)

2. 以下のコマンドからWebhookを設定します
```shell
send_discord --set url wenhookのURL
```

3. 以下のコマンドを例にdiscordにデータを送ります  
- 普通に送る例  
```shell
send_discord 送る文章
```
- パイプを利用した例  
```shell
echo "aaa"|send_discord
```

## オプション
|オプション名|引数|詳細|
|----|----|----|
|-n \| --name|表示名|送るときの表示名をその時だけ変える|
|-i \| --icon|アイコンのURL|送るときのアイコンをその時だけ変える|
|-s \| --set|name 表示名|メッセージを送るときのデフォルトの名前を設定できる|
|-s \| --set|icon アイコンのURL|メッセージを送るときのデフォルトのアイコンを設定できる|
|-s \| --set|url\|URL 表示名|メッセージを送るWebhookのURLを設定できる|
