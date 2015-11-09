# dokku-deploy-script

For use with [dokku](https://github.com/progrium/dokku)

Run commands in the container before its deployment. Using this plugin allows to use commands that needs volumes for example.

## Requirements

* Dokku version `0.4` or higher

## Installation

On the dokku server, you need to install the plugin in the standard Dokku way. Specifically:

```
# dokku 0.4.x
dokku plugin:install https://github.com/OzConseil/dokku-deploy-script.git
```

## Usage

In your application's folder, add a `.deploy` file with your commands:

```
cd /var/www && composer run-script deploy
```

## Thanks
Thanks to [dokku-predeploy-tasks](https://github.com/michaelshobbs/dokku-app-predeploy-tasks).
