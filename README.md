# django_boilerplate

- 시스템에 `docker`, `docker-compose`가 설치된 것으로 가정합니다.

# 구성 container
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

## Usage

- repository clone
```
git clone https://github.com/ithingv/django_boilerplate.git

cd django_boilerplate
```

- 도커 빌드 및 실행
```
docker-compose up -d
```

```
- 컨테이너 쉘 실행
```
docker exec -it [container_name] bash
```
