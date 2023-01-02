# Cargo로 로컬에서 코드 실행하기

자신의 시스템에서 코드를 실험하고 싶다면 먼저 러스트를 설치해야 합니다. [instructions in the Rust Book][1]에 따라 설치를 수행하십시오. 이렇게 하면 작동하는 `rustc` 와 `cargo`가 제공됩니다. 작성 시점에 안정적인 최신 러스트 릴리스의 버전은 다음과 같습니다.

```shell
% rustc --version
rustc 1.61.0 (fe5b13d68 2022-05-18)
% cargo --version
cargo 1.61.0 (a028ae4 2022-04-29)
```

도구가 준비되면 다음 단계에 따라 이 트레이닝의 예제 중 하나에서 러스트 바이너리를 빌드합니다.

1. 복사하려는 예제에서 "클립보드에 복사<sup>Copy to clipboard</sup>" 버튼을 클릭합니다.

2. `cargo new exercise`를 사용하여 코드에 대한 새로운 `exercise/` 디렉토리를 만듭니다.

    ```shell
    $ cargo new exercise
         Created binary (application) `exercise` package
    ```

3. `exercise/`로 이동하고 `cargo run`을 사용하여 바이너리를 빌드하고 실행합니다.

    ```shell
    $ cd exercise
    $ cargo run
       Compiling exercise v0.1.0 (/home/mgeisler/tmp/exercise)
        Finished dev [unoptimized + debuginfo] target(s) in 0.75s
         Running `target/debug/exercise`
    Hello, world!
    ```

4. `src/main.rs`에서 상용구<sup>boiler-plate</sup> 코드를 자신의 코드로 교체하십시오. 예를 들어, 이전 페이지의 예를 사용하여 `src/main.rs`를 다음과 같이 만듭니다.

    ```rust
    fn main() {
        println!("Edit me!");
    }
    ```

5. `cargo run`을 사용하여 업데이트된 바이너리를 빌드하고 실행하십시오.

    ```shell
    $ cargo run
       Compiling exercise v0.1.0 (/home/mgeisler/tmp/exercise)
        Finished dev [unoptimized + debuginfo] target(s) in 0.24s
         Running `target/debug/exercise`
    Edit me!
    ```

6. `cargo check`를 사용하여 프로젝트의 오류를 빠르게 확인하고 `cargo build`를 사용하여 실행하지 않고 컴파일하십시오. 일반 디버그 빌드의 경우 `target/debug/`에서 출력을 찾을 수 있습니다. `cargo build --release`를 사용하여 `target/release/`에서 최적화된 릴리스 빌드를 생성합니다.

7. `Cargo.toml`을 수정하여 프로젝트에 의존성<sup>dependencies</sup>을 추가합니다. `cargo` 명령을 실행하면 누락된 의존성을 자동으로 다운로드하고 컴파일합니다.

[1]: https://doc.rust-lang.org/book/ch01-01-installation.html
