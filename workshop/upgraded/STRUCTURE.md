# upgraded 디렉터리 파일 구조 설명

이 디렉터리는 legacy 프로젝트의 모든 파일과 폴더를 동일하게 복사한 업그레이드 작업 공간입니다.

## 주요 폴더 및 파일

- `MANIFEST.in`, `README.rst`, `distribute_setup.py`, `distribute-0.6.10.tar.gz`, `setup.py`: 프로젝트 메타 및 설치 관련 파일
- `docs/`: Sphinx 기반 문서 폴더
  - `build/`: 빌드 결과물 (doctrees, html 등)
  - `source/`: 문서 소스(rst, conf.py, _static 등)
- `guachi/`: 주요 Python 패키지 소스
  - `__init__.py`, `config.py`, `database.py`: 핵심 모듈
  - `tests/`: 단위 테스트 모듈
- `guachi.egg-info/`: 패키징 정보
  - `PKG-INFO`, `SOURCES.txt`, `dependency_links.txt`, `top_level.txt`

## 목적

이 디렉터리는 레거시 코드를 최신 Python 환경으로 포팅 및 업그레이드하기 위한 작업 공간입니다. 모든 파일은 원본과 동일하게 복사되었으며, 이후 단계별로 코드 수정 및 현대화 작업이 진행됩니다.

---

> 이 구조 설명 파일은 업그레이드 작업의 이해를 돕기 위해 작성되었습니다.