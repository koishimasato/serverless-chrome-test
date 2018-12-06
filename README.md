# 参考
[Puppeteer on AWS Lambda で日本語対応したキャプチャを撮影してS3にアップロードするまでの設定 - Qiita](https://qiita.com/zyyx-matsushita/items/c33f79e33f242395019e)
[PuppeteerをLambdaで使う前段階、serverless-chrome/lambdaのnpmインストールでハマったときの解決法 | PRESSMAN*Tech](https://www.pressmantech.com/tech/serverless/4613)

[sambaiz/puppeteer-lambda-starter-kit: Starter Kit for running Headless-Chrome by Puppeteer on AWS Lambda.](https://github.com/sambaiz/puppeteer-lambda-starter-kit)


# ゴール
- puppeteerでスクショ保存 → slackへ通知
- localからlambdaへremoteでdevtoolでデバッグできる

場合によってはlambdaではなくfargete



# メモ
デプロイに10分かかる


[How to get headless Chrome running on AWS Lambda – Marco Lüthy – Medium](https://medium.com/@marco.luethy/running-headless-chrome-on-aws-lambda-fa82ad33a9eb)

# メインライブラリ
[serverless-chrome/examples/serverless-framework/aws at master · adieuadieu/serverless-chrome](https://github.com/adieuadieu/serverless-chrome/tree/master/examples/serverless-framework/aws)


# 動かない
[serverless-plugin: ECONNREFUSED · Issue #63 · adieuadieu/serverless-chrome](https://github.com/adieuadieu/serverless-chrome/issues/63)

+ @serverless-chrome/
の
bundle.es.jsの340行目をコメントアウト
            // chromePath,


