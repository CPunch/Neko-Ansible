# Neko-Ansible

Running a [Neko]() instance can be expensive due to the high spec demand of running a whole desktop, browser && streaming all of that data to remote peers. Thankfully, here's your solution.

Neko-Ansible lets you setup a Neko instance quick && easy, meaning you get more time actually running neko and less time setting it up!

Things you'll need:
- vps
- domain pointing to said vps

This playbook expects to be ran on the latest debian stable release.

## Usage

You'll need a `hosts` file, an example one looks like:
```
[hosts]
neko-vps ansible_host=45.77.220.92 ansible_user=root ansible_connection=ssh
```

then, just run the playbook and follow the prompts!
```sh
$ ansible-playbook -i hosts run.yml
```

## Why?

Neko is cool, but the price for a vps good enough to run it is not. With this, it makes neko setup easy enough that you can create/destroy the server at will. I've found that in the past month of having a "movie night" with some friends every other weekend I've only spent ~$0.30 on the vps LOL. (roughly 4, 3-4 hour sessions)