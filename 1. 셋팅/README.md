# 셋팅

`Apple M2 Max`
`macOS Ventura 13.5(22G74)`

## java 설치

`brew install openjdk@17`

`sudo ln -sfn /opt/homebrew/opt/openjdk@17/libexec/openjdk.jdk /Library/Java/JavaVirtualMachines/openjdk-17.jdk`

`echo 'export PATH="/opt/homebrew/opt/openjdk@17/bin:$PATH"' >> ~/.zshrc`

`source ~/.zshrc`

`java -version`

[참고](https://velog.io/@may_yun/Mac-M1-Java-17-%EC%84%A4%EC%B9%98)

## VSCode 플러그인 설치

- Extension Pack for java 
- SpringBoot Extension Pack
- Gradle for java

[참고](https://csj000714.tistory.com/711)

## 자바 버전 변경

https://8156217.tistory.com/62
https://developer.apple.com/forums/thread/687489

$ vim ~/.zshrc

 export JAVA_HOME=/Library/Internet Plug-Ins/JavaAppletPlugin.plugin/Contents/Home
    export PATH=$JAVA_HOME/bin:$PATH



sdkman 사용
https://blog.yozi.kr/entry/%EC%A0%9C%EB%8C%80%EB%A1%9C-%EB%90%9C-JDK%EB%A5%BC-%EC%82%AC%EC%9A%A9%ED%95%98%EC%9E%90-M1-mac-%EC%97%90%EC%84%9C-java-%EC%84%A4%EC%B9%98

https://phoby.github.io/sdkman/

sdk use java oracle-21
sdk list java
sdk current