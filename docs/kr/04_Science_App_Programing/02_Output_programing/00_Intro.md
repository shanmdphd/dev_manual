# 출력 프로그래밍 기초

해석 결과 데이터는 파일 형태로 출력해야 하며, result 폴더에 생성되어야 합니다.

> result 폴더 생성하는 예제를 보시면 예제코드에서는 result 폴더를 생성하는 명령어를 실행하기 전 result 폴더를 삭제하는 명령어를 실행합니다.
> 프로그램 테스트를 반복하는 과정에서 결과 파일이 남아있는 경우 문제가 발생할 수 있습니다. 이를 방지하고자 result 폴더를 삭제하는 코드를 추가하였습니다.

이후 파일 입출력 함수 이용해 result 폴더안에 파일을 쓰기 모드로 생성하면 됩니다.

# 언어별 예제 보기

 - [C](../03_C/03_Output_program.md)
 - [Fortran](../04_Fortran/03_Output_program.md)
 - [Python]()
 - [R]()
 - [Octave]()


### Octave
### result 폴더 생성
Octave의 경우 별도의 선언없이 ```mkdir``` 함수를 이용하면 되며, ```result``` 폴더를 생성하는 예제는 아래와 같습니다.

```matlab
...
rmdir result
mkdir result
...
```

### 결과 파일 생성

```matlab
file_out = fopen('result/result.txt', 'w');
...

...
fdisp(file_out, 'Hello EDISON.');
...

...
fclose(file_out);
```
