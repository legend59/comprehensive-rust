# 러스트 종합편에 오신 것을 환영합니다 🦀

* 이 문서는 [Welcome to Comprehensive Rust](https://google.github.io/comprehensive-rust)에서 영어 원문을 확인하실 수 있으며, [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0) 라이센스를 따릅니다.

구글 안드로이드 팀에서 개발한 4일짜리 러스트 과정입니다. 이 과정은 기본 구문에서 제네릭<sup>generic</sup>과 오류 처리와 같은 고급 주제에 이르기까지 러스트의 전체 스펙트럼을 다룹니다. 마지막 날에는 안드로이드 전용 콘텐츠도 포함되어 있습니다.

과정의 목표는 러스트를 가르치는 것입니다. 당신이 러스트에 대해 아무것도 모른다고 가정하고 다음을 희망합니다:

* 러스트 구문과 언어에 대한 종합적인 이해를 제공합니다.
* 러스트에서 기존 프로그램을 수정하고 새 프로그램을 작성할 수 있습니다.
* 일반적인 러스트 관용구<sup>idioms</sup>를 보여줍니다.

4일 차에는 다음과 같은 안드로이드 관련 사항을 다룹니다.

* 러스트에서 안드로이드 구성요소 빌드
* AIDL 서버와 클라이언트
* C, C++, 자바와의 상호 운용성

이 과정은 러스트에서 안드로이드 **애플리케이션** 개발을 다루지 않으며 안드로이드 관련 부분은 특히 운영 체제인 안드로이드 자체를 위한 코드 작성에 관한 것임을 유의하는 것이 중요합니다.

## 목표로 하지 않는 것

러스트는 방대한 언어이며 며칠 안에 모든 것을 다룰 수는 없습니다.
이 과정에서 목표로 하지 않는 것은 다음과 같습니다.

* 비동기<sup>async</sup> 러스트 사용 방법 배우기 --- 전통적인 동시성 프리미티브<sup>concurrency primitives</sup>를 다룰 때 비동기 러스트에 대해서만 조금 이야기할 것입니다. 이 주제에 대한 자세한 내용은 대신 [Asynchronous Programming in Rust](https://rust-lang.github.io/async-book/)를 참조 하세요.
* 매크로 개발 방법에 대해 알아보려면 [Rust Book의 19.5절](https://doc.rust-lang.org/book/ch19-06-macros.html) 과 [Rust by Example](https:// doc.rust-lang.org/rust-by-example/macros.html)을 대신 참고하세요.
* unsafe 러스트를 작성하는 방법에 대해 자세히 알아보세요. 3일 차에 unsafe 러스트에 대해 이야기하겠지만 미묘한 세부 사항은 다루지 않습니다. 대신 [Rust Book의 19.1절](https://doc.rust-lang.org/book/ch19-01-unsafe-rust.html) 과 [Rustonomicon](https://doc.rust-lang)을 참조 하세요.

## 가정

이 과정에서는 프로그래밍 방법을 이미 알고 있다고 가정합니다. 러스트는 정적으로 타입이 지정되는 언어<sup>statically
typed language</sup>이며 때때로 러스트 접근 방식을 더 잘 설명하거나 비교하기 위해 C/C++와 비교할 것입니다.

파이썬 또는 자바스크립트와 같은 동적 타입 언어로 프로그래밍하는 방법을 알고 있다면 잘 따라갈 수 있습니다.
