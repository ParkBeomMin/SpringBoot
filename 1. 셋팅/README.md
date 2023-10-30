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