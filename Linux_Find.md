## Linux Find
##### 'find'는 Linux와 Unix 기반 시스템에서 사용되는 강력한 파일 검색 유틸리티입니다. 'find' 명령어는 파일 시스템에서 파일이나 디렉토리를 검색하고, 사용자가 지정한 조건에 따라 파일을 찾아주는 역할을 수행합니다. 다양한 옵션과 조건을 사용하여 원하는 파일을 찾을 수 있습니다.
<pre>
find [경로] [표현식] [동작]
</pre>
`경로`
- 파일을 검색할 시작 디렉토리 경로를 지정합니다.
- 기본적으로 현재 디렉토리에서 검색을 시작합니다.

`표현식`
- 파일 검색 조건을 지정합니다.
- 이 부분에는 파일 이름, 크기, 수정 시간 등을 지정할 수 있습니다.

`동작`
- 검색 결과에 대해 수행할 동작을 지정합니다.
- 주로 파일을 출력하거나 다른 명령을 실행하는 등의 동작을 지정합니다.
___
`사용 예시`
> 파일 이름으로 검색
> <pre>
> find /patch/to/direcotry -name "filename.txt"
> </pre>

> 특정 유형의 파일 검색
> <pre>
> find /path/to/directory -type f -name "*.txt"
> </pre>
> * 위 명령은 '/path/to/directory' 경로에 확장자가 ".txt"인 모든 파일을 검색합니다.

> 파일 크기로 검색
> <pre>
> find /path/to/directory -size +1M
> </pre>
> * 위 명령은 '/path/to/directory' 경로에서 1MB 크기보다 큰 파일을 검색합니다.

> 파일 수정 시간으로 검색
> <pre>
> find /path/to/directory -mtime -7
> </pre>
> * 위 명령은 '/path/to/directory' 경로에서 7일 이내에 수정된 파일을 검색합니다.
