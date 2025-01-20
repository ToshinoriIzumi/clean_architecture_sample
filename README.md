# clean_architecture_sample
### アプリケーションの起動方法

- アプリケーションルートディレクトリに移動する。

```bash
cd [アプリのルートディレクトリ]
```

- イメージの作成

```bash
docker build . -t clean_architecture_sample_app
```

- コンテナの起動

```bash
docker run -p 8501:8501 -v $(pwd)/src:/opt/app/src --rm  --name clean_architecture_sample_app -it clean_architecture_sample_app
```
