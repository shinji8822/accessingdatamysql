# accessingdatamysql
https://spring.pleiades.io/guides/gs/accessing-data-mysql/

### セットアップ
jdkインストール
```
java --version
openjdk 17.0.5 2022-10-18
OpenJDK Runtime Environment (build 17.0.5+8-Ubuntu-2ubuntu1)
OpenJDK 64-Bit Server VM (build 17.0.5+8-Ubuntu-2ubuntu1, mixed mode, sharing)
```
~/.bash_profile
```
export JAVA_HOME=/usr/lib/jvm/java-17-openjdk-amd64
export DOCKER_HOST=tcp://localhost:2376
```

### アプリケーションの実行
```
./mvnw spring-boot:run
```

### データ追加
```
curl http://localhost:8080/demo/add -d name=First -d email=someemail@someemailprovider.com
```

### データ取得
```
curl http://localhost:8080/demo/all
```
