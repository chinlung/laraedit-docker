# laraedit-docker (locale to Asia/Taipei)
Dockerized version of Laravel Homestead

# Documentation
For now you can [check out the wiki](https://github.com/laraedit/laraedit-docker/wiki) for details on using the container. Once the container is stable, I will add more instructions here in the readme.

# Build Information
You can find the latest build details on the [Docker Hub](https://hub.docker.com/r/chinlung/laraedit-docker/)

# What works
- [x] Nginx 1.8.1
- [x] PHP 7.0
- [x] SQLite
- [x] MySQL 5.7
- [x] Redis
- [x] NodeJS
- [ ] PostreSQL
- [x] Beanstalkd
- [x] Blackfire
- [x] Bower
- [x] Gulp
- [x] Composer
- [x] Laravel Envoy
- [x] Laravel Installer
- [ ] Lumen Installer

# How to use the container
### Kitematic (the easy way)
  1. Search for `laraedit-docker`
  2. Create LaraEdit container
  3. Point the `/var/www/html/app` volume to your local application directory.

### CLI (the other easy way)
  1. Pull in the image
  ```
    docker pull chinlung/laraedit-docker
  ```  
  2. Run the container
  ```
    docker run -p 80:80 -v /path/to/your/app:/var/www/html/app chinlung/laraedit-docker
  ```


# MySQL Details

- MySQL Username = `homestead`
- MySQL Password = `secret`
- MySQL Database = `homestead`

You are free to create more databases and/or users, but these are available to you as soon as you run the container!
