# 리플릿 Repl.it 에서 .replit 파일 RUN 설정하는 방법!!!


요즘 repl.it을 참 애용합니다.

<a href="#">
 <img src="https://pbs.twimg.com/profile_images/1181584215818637318/5PSC29ff_400x400.jpg" width="100px">
</a>

깃허브에서 repo를 만들고,
빈 repo를 import 해서 repl.it에서 편집합니다.

하지만 할 때마다 .replit 에서 run 을 설정하라고 하는데,
언어가 바뀔 때 뭘 설정해야할 지 모르겠더라구요...




 > 찾아봐도 자료는 없고 답답해서 내가 정리해서 올립니다.
 
 
 
 

모든 첫 파일이름은 main으로 한다고 가정합니다. (index.html제외)

### C :
run = "clang-7 -pthread -lm -o main main.c \n ./main"

### JAVA :
run = "javac -classpath .:/run_dir/junit-4.12.jar:target/dependency/* -d . Main.java \n java -classpath .:/run_dir/junit-4.12.jar:target/dependency/* Main"

### python :
run="python main.py"

### HTML CSS JS :
run = "index.html"


제가 주로 쓰는 언어들이라 해놨는데,
더 필요하면 업데이트 하겠습니다.
