# greet-ci

인사말 프로그램과 GitHub Actions CI 구성. 모든 명령은 저장소 루트에서 실행한다.

## 실행

```
uv run --locked python greet.py Hee
uv run --locked python greet.py
```

## 검사

```
uv lock
uv run --locked pytest -q greet.py
uv run --locked black --check greet.py
uv run --locked flake8 greet.py
uv run --locked mypy greet.py
uv build
```
