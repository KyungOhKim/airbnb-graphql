# airbnb-graphql

- Register - Send confirmation email
- Login
- Forgot Password
- Logout
- Cookies and Http Header
- Authentication middleware
- Rate limiting
- Locking accounts
- Testing (probably Jest)

# Part 0

typeorm 프로젝트 생성
typeorm init --name 프로젝트명 --database postgres

db 생성
psql -U postgres
password 입력 후 create database DB이름;

QueryFailedError: cnst.consrc 칼럼 없음 at new QueryFailedError
-> typeorm 버전을 0.2.21로 올려서 해결

# Part 1

사용자를 만들때마다 자동으로 uuid를 생성

# Part 2

users 테이블에 email, password를 mutation함

# Part 3

yarn test 할 때 securityerror: localstorage is not available for opaque origins at window.get localstorage [as localstorage]
-> jest 버전을 24.9.0로 올려서 해결
