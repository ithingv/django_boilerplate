# django_boilerplate

- 시스템에 `docker`, `docker-compose`가 설치된 것으로 가정합니다.

### 이미지
- django 
- pgadmin
- postgresql

```
# DB 설정 변경
# project/settings.py

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'db',
        'USER': 'postgres',
        'PASSWORD': 'password',
        'HOST': 'pgdb',
        'PORT': 5432,
    }
}
```

## 사용법

- 저장소 클론
```
git clone https://github.com/ithingv/django_boilerplate.git

cd django_boilerplate
```

- 도커컴포즈 빌드 및 실행

```
docker-compose up --build
```

- 컨테이너 쉘 실행
```
docker exec -it [container_name] bash
```
