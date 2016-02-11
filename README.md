# docker-registry-auth
Docker private registry with login

`
#docker run --rm --entrypoint htpasswd registry:2 -Bbn user password >> auth/htpasswd
docker-compose up -d
`

default login
username: user,

password: password
