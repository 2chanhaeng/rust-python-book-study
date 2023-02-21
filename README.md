# Rust Python Book Study
[파이썬 프로그래머를 위한 러스트 입문](https://indosaram.github.io/rust-python-book/)을 읽고 학습한 내용을 정리합니다.

## rust 프로젝트 생성
1. `cargo init`:
    현재 디렉토리에 프로젝트를 생성합니다.  
    ```
    .
    ├── Cargo.toml
    └── src
        └── main.rs
    ```
2. `cargo new < 프로젝트 이름 >`:
    현재 디렉토리에 해당 프로젝트 이름으로 프로젝트를 생성합니다.  
    ```
    .
    └──프로젝트 이름
        ├── Cargo.toml
        └── src
            └── main.rs
    ```

## rust 프로젝트 컴파일

1. `cargo build`:
    프로젝트를 디버그 모드로 빌드합니다.  
    빌드된 파일은 `target/debug`에 해당 프로젝트 이름의 바이너리 파일로 생성됩니다.  
    디버그 모드로 빌드가 될 경우, 컴파일은 빠르지만 실행 속도가 느리고, 컴파일된 바이너리 파일의 크기가 큽니다.  
    따라서 실제 서비스에 사용할 경우에는 `cargo build --release`로 릴리즈 모드로 빌드해야 합니다.  
2. `cargo build --release`:
    프로젝트를 릴리즈 모드로 빌드합니다.  
    빌드된 파일은 `target/release`에 해당 프로젝트 이름의 바이너리 파일로 생성됩니다.  
    릴리즈 모드로 빌드가 될 경우, 컴파일은 느리지만 실행 속도가 빠르고, 컴파일된 바이너리 파일의 크기가 작습니다.  

## rust 프로젝트 실행

`cargo run` 명령어로 프로젝트를 빌드부터 실행까지 한 번에 진행할 수 있습니다.  
마찬가지로, `--release` 옵션을 추가하면 릴리즈 모드로 빌드부터 실행까지 한 번에 진행할 수 있습니다.

## rustfmt

`rustfmt`은 rust 코드를 포맷팅해주는 도구입니다.  
VSC에서는 `Alt + Shift + F`(Window, Linux), `⌥ + ⇧ + F`(Mac) 단축키로 포맷팅할 수 있습니다.  
