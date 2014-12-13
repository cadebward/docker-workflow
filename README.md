Before use:
 - Install [boot2docker](https://github.com/boot2docker/osx-installer/releases)
 - Install [fig](http://www.fig.sh/install.html)
 - Know your docker ip: `boot2docker ip`

To use django scaffold:
 - `git clone https://github.com/cadew/docker-workflow.git`
 - `cd docker-workflow`
 - `fig build`
 - `fig up`
 - ????
 - profit

You can now edit files and see them live at `your-docker-ip:8000`. For example, try changing the admin url from `/admin` to `/test`. Now go to `your-docker-ip:8000/test` and you'll see the admin interface without reloading docker or fig!