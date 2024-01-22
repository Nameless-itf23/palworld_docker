## docker-compose for Pal World
Dockerfile を使わず docker-compose.yml 単体で Pal World のサーバー (Pal Server) を動作させます。

## Feature

- コンテナ内の steamapps フォルダが data フォルダにマウントされるため、Pal Server のファイルをコンテナ外から直接変更できるのでとても管理が楽です。

### Usage

```bash
# このリポジトリをクローンしたディレクトリに移動
cd path/to/this/repository

docker compose up
```

### 注意
- 正常に動作しない場合、 data フォルダの中身を削除することをお勧めします。
- data フォルダの所有者・所有グループを非 root ユーザーにしてください。
