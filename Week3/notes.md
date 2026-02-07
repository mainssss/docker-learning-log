## Week 3：Docker 基本概念と Ubuntu コンテナ起動

### Docker の基本構造（簡単な理解）

Docker は大きく分けて以下の要素で構成されている。

- **Image（イメージ）**
  - アプリや OS 環境の「設計図」
  - 読み取り専用
  - 例：ubuntu、nginx など

- **Container（コンテナ）**
  - Image から実行された「実体」
  - 実際にコマンドを動かす環境
  - 停止・削除が可能

Image = 静的  
Container = 動的

という理解で問題ない。

---

### Ubuntu イメージの取得

Docker Hub から公式の Ubuntu イメージを取得する。

```bash
docker pull ubuntu

Ubuntu コンテナを対話モードで起動する:docker run -it ubuntu /bin/bash
成功すると、以下のような状態になる：root@xxxxxxxx:/#
