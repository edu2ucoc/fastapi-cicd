# 구조
.
L app
    L Dockerfile        : fastapi 관련 도커파일 (핵심서비스)
    L main.py           : 파이썬 구성된 fastapi 기반 코드 (개발한 내용)
    L requirements.txt  : 서비스 구동을 위한 필요 패키지 목록
L nginx
    L nginx.conf        : nginx 에서 fastapi로 프록시 하는 구성 (설정파일)
L docker-comspoe.yml    : 컴포즈 파일 -> n개의 컨테이너 구성->연결->구동