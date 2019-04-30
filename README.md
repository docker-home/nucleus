# nucleus

atlassian/nucleus:latest

https://github.com/atlassian/nucleus

## deploy step

### pull image

```
docker pull wuyue/nucleus:latest
```

### create an gpg

https://confluence.antio.top/display/~wuyue/nucleus#nucleus-%E7%94%9F%E6%88%90gpg

### config your `config.js`

follow the config.template.js and setup what you want

example here: 

https://confluence.antio.top/display/~wuyue/nucleus#nucleus-%E9%85%8D%E7%BD%AE%E6%96%87%E4%BB%B6

## run

```
docker run --name nucleus-server -d -v <path-to-your-config.js>:/opt/service/config.js -p 8080:3030 wuyue/nucleus:latest
```