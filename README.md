# Gemini スクレイピングコード・ジェネレーター

このツールは、指定したWebサイトをスクレイピングするためのPythonコードを自動生成するツールです。

各自のパソコン（ローカル環境）で安全に動作します。

![スクリーンショット](https://github.com/securecat/Gemini-scraping-code-generator/blob/main/screenshot.png?raw=true)

## 準備

1. [Google AI Studio](https://aistudio.google.com/)にアクセスし、「API Key」を取得してください（無料枠もあります）。
2. お使いのパソコンにPythonがインストールされていることを確認してください。
3. [gemini_scraping_code_generator.zip](https://github.com/securecat/Gemini-scraping-code-generator/raw/refs/heads/main/gemini_scraping_code_generator.zip)をダウンロードして展開してください。

## 使い方

1. ローカルで `Gemini_scraping_code_generator.html` をブラウザで開きます。
2. 取得したAPI Keyと、スクレイピングしたいサイトの条件を入力します。
3. ボタン「Pythonコードを自動生成する」を押すと、数十秒でコードが生成されます。
4. 生成されたコードを`.py`ファイルとして保存し、ターミナルやコマンドプロンプトで実行してください。

**※必要なライブラリのインストールコマンド：**

- （Windowsの場合）
```
py -m pip install beautifulsoup4 requests
```

- （macOS / Linuxの場合）
```
python3 -m pip install beautifulsoup4 requests
```

## 注意点・免責事項（必ずお読みください）

### 1. 利用規約の遵守と自己責任

本ツールは個人の学習・情報収集の補助を目的としています。スクレイピングを実行する際は、対象となるWebサイトの利用規約（Robots.txt等を含む）を必ず確認し、それに従って使用してください。本ツールの使用によって生じたあらゆる損害やトラブルについて、制作者は一切の責任を負いません（自己責任でご利用ください）。

### 2. サーバーへの負荷軽減（マナー）

自動生成されるPythonコードには、標準で1秒間の待機時間（time.sleep(1)）が設定されています。対象サーバーに過度な負荷をかけ、アクセス禁止（BAN）や迷惑行為とならないよう、この待機時間は削らずに実行してください。

### 3. APIキーの管理

入力したGemini APIキーは、お使いのブラウザ内（ローカル環境）にのみ安全に保存され、外部に送信されることはありません。ただし、この「gemini_scraping_code_generator.html」自体をそのままインターネット上のサーバー（GitHub Pagesなど）にアップロードしてWebサイトとして公開すると、通信データからAPIキーが漏洩する危険があります。必ずご自身のパソコン内にダウンロードした状態のまま（ローカル環境）で実行してください。


