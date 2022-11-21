# analysis-seunjeon

> 은전한닢 프로젝트 - 원하는 elasticsearch 버전에 맞게 빌드하기
>
> [은전한닢 저장소](https://bitbucket.org/eunjeon/seunjeon.git)

scala, elasticsearch analysis plugin 등 잘 모르지만,
원본 레포지토리에서 제시하는 방법대로 빌드 시도함.

|  버전  |        빌드        |        동작        |
| :----: | :----------------: | :----------------: |
| 6.8.18 | :white_check_mark: | :white_check_mark: |

## 6.8.18

- `ESLoggerFactory` 제거 - 6.8.18 버전에 없는 객체로 보임
- `run org.bitbucket.eunjeon.seunjeon` 명령으로 변경 - sbt에서 `run-main` 명령어가 없어진 것으로 보임
- `build.sbt` > `val esVersion = "6.8.18"` 변경

## References

- [elastic document: docker](https://www.elastic.co/guide/en/elasticsearch/reference/current/docker.html)
- [github: elasticsearch Dockerfile](https://github.com/elastic/elasticsearch/blob/8.5/distribution/docker/src/docker/Dockerfile)
- [github: docker-elasticsearch-alpine](https://github.com/blacktop/docker-elasticsearch-alpine/blob/master/6.8/Dockerfile)
