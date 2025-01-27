# 러스트 생태계

러스트 생태계는 여러 도구로 구성되어 있으며 주요 도구는 다음과 같습니다.

* `rustc`: `.rs` 파일을 바이너리와 기타 중간 형식으로 변환하는 러스트 컴파일러

* `cargo`: 러스트 의존성 관리자와 빌드 도구. Cargo는 <https://crates.io>에서 호스팅되고 있는 의존성<sup>dependencies</sup>을 다운로드하는 방법을 알고 있으며 프로젝트를 빌드할 때 `rustc`로 의존성을 전달합니다. Cargo에는 단위 테스트를 실행하는 데 사용되는 내장 테스트 러너<sup>built-in test runnter</sup>도 함께 제공됩니다.

* `rustup`: 러스트 툴체인 설치 프로그램과 업데이트 프로그램. 이 도구는 러스트의 새 버전이 릴리스될 때 `rustc` 와 `cargo`를 설치하고 업데이트하는 데 사용됩니다. 또한 `rustup`은 표준 라이브러리에 대한 문서도 다운로드합니다. 한 번에 여러 버전의 러스트를 설치할 수 있으며 `rustup`을 사용하면 필요에 따라 버전 간에 전환할 수 있습니다.