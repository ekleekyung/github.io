#daily
 - tags : memo.md 참조

##tips
###[intellij] jsp 서버재시작없이 반영
> project structure
> project settings
> artifacts
> exploded war선택 > output directory
> target에서 webapp으로 변경


```
D:\workspace\SignCastV2\target\SignCastV2User
->
D:\workspace\SignCastV2\src\main\webapp
```



##todo solve
###1.[intellij]dc 등 관련 live template 설정 옮기기.
###2.[MC] player_skin null 문제 - event시
###3. Jekyll을 사용하여 GitHub Pages 만들기 - 우선순위 낮아도 됨.
###4. diff classes path
###5.


##solved
###[intellij] hibernate schema run as application 문제.//2017.12.18 : -ek

: intellij hibernate schema관련 작업을 .java run as application 문제.

error log : servlet null 관련  >
 1. pom.xml 수정
 ```
 <dependency>
     <groupId>javax.servlet</groupId>
     <artifactId>javax.servlet-api</artifactId>
     <version>3.1.0</version>
     <scope>provided</scope>
 </dependency>
 ```
 2. cfg 위치수정(resource 쪽으로)


###[SC] jdk complier 1.6으로 재지정문제.//2017.11.?? : -ek
 1. pom.xml 수정
 maven-compiler-plugin 내 config 의 source와 target 을 1.7로 수정

```
<plugin>
    <groupId>org.apache.maven.plugins</groupId>
    <artifactId>maven-compiler-plugin</artifactId>
    <version>2.5.1</version>
    <configuration>
        <source>1.7</source>
        <target>1.7</target>
        <compilerArgument>-Xlint:all</compilerArgument>
        <showWarnings>true</showWarnings>
        <showDeprecation>true</showDeprecation>
    </configuration>
</plugin>
```



블로그 링크:
http://blog.saltfactory.net/upgrade-github-pages-dependency-versions/


그외 좀더 유용한 페이지
https://jekyllrb-ko.github.io/docs/frontmatter/

공식주소 github
https://github.com/jekyll/jekyll

https://github.com/jekyll/jekyll/pull/2031
###3.https://github.com/jekyll/jekyll/pull/2031


##todo organize
###1.


