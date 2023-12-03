# docker-registry

## Install

プロジェクト起動

```bash
docker compose build

docker compose up -d
```

画面アクセス

`http://localhost:8888`

## Command

レジストリに登録したいDockerイメージにタグ付け

```bash
docker tag {イメージ名 or イメージID} {レジストリのホスト名}:{port}/{任意の名称}
```

レジストリにDockerイメージをプッシュ

```bash
docker push {レジストリのホスト名}:{port}/{任意の名称}:latest
```

レジストリからDockerイメージをプル

```bash
docker pull {レジストリのホスト名}:{port}/{任意の名称}
```
