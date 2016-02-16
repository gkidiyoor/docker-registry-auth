# docker-registry-auth
Docker private registry with login

`
//docker run --rm --entrypoint htpasswd registry:2 -Bbn user password >> auth/htpasswd
`


`
docker-compose up -d
`
or

`
cd basic_auth && docker run -d -p 5000:5000 --restart=always --name registry -v `pwd`/certs:/certs -e REGISTRY_HTTP_TLS_CERTIFICATE=/certs/domain.crt -e REGISTRY_HTTP_TLS_KEY=/certs/domain.key registry:2
`


default login
username: user,

password: password



Usefull commands: docker kill <container>, docker rm -v registry
