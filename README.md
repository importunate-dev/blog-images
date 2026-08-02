# blog-images

`importunate-dev.github.io` 블로그에서 jsDelivr CDN으로 사용하는 이미지 저장소다.

## 새 게시글 이미지 경로

여러 이미지를 사용하는 글은 게시글 단위로 디렉터리를 분리한다.

```
{카테고리}/{시리즈}/{YYYY-MM-DD}/{의미-있는-파일명}.{확장자}
```

예시:

```
project/godot/2026-08-02/turn.gif
project/godot/2026-08-02/stock-price.gif
```

- 경로와 파일명은 영문 소문자 kebab-case를 사용한다.
- 시리즈 전체에서 `1.gif`, `2.gif`처럼 전역 순번을 이어 붙이지 않는다.
- 이미 발행된 이미지 경로는 기존 CDN 링크가 깨질 수 있으므로 이동하지 않는다.
- 본문에서는 `https://cdn.jsdelivr.net/gh/importunate-dev/blog-images/{경로}`로 참조한다.
