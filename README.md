fa-emoji
=======================

Emoji plugin for [Discourse](http://discourse.org) which adds the FontAwesome icons as emoji

Usage
=====

In your posts, use :fa_NAME: to display the icon as an emoji 
For example:

```
   :fa_steam: will display the Steam Logo
```

Installation
============

* Add the plugin's repo url to your container's `app.yml` file

```yml
hooks:
  after_code:
    - exec:
        cd: $home/plugins
        cmd:
          - mkdir -p plugins
          - git clone https://github.com/discourse/docker_manager.git
          - git clone https://github.com/sg/fa-emoji.git
```

* Rebuild the container

```
cd /var/docker
git pull
./launcher rebuild app
```

License
=======
MIT
