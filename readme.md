# hello devcontainer

## remoteの場合

- `docker -H ssh://user@remote-host ps` にてssh先でdockerが動いていることを確認
- `docker context cretate remotehost --docker 'host=ssh://user@remote-host'` で保存
- `docker context ls` にて一覧に現れていることを確認
- `docker context use remotehost` で以後ローカルからのdockerコマンドは remote-hostにて実行される
- (`docker context use default` で元に戻せる)


## vscodeにて（localでdockerを動かすときにはここから)

- vscode にて `Remote-Containers: Open Repository in unique volume`を実行して `n9d/hello-devcontainer` を指定する

