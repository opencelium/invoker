# OpenCelium - Free Invoker Repository

This repository serves as an invoker library. It is an extension of OpenCelium.
Please visit [opencelium.io](https://www.opencelium.io) for more details.

## How to use?

Open your Opencelium installation on the web server and go to the Invoker directory.

You can find it here: 
```
 cd /opt/src/backend/src/main/resources/invokers
```

Move all files temporarily away. After that, clone the repository inside of this folder.

```
git clone https://github.com/opencelium/invoker.git .
```

> **_NOTE:_**  Do not forget the dote at the end of the previous command.

After that you can always update connector files with this command.

```
git pull
```

> **_NOTE:_**  It is possible to automatically synchronize the invoker files when using a cron job.

<b>Example: </b>

First enter to crontab

 ``` crontab -e ```

Now add a job that runs every evening at 1 a.m

```
/usr/bin/git --git-dir=/opt/src/backend/src/main/resources/invokers/.git --work-tree=/opt/src/backend/src/main/resources/invokers pull
```
