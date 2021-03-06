---
ID: 7761
post_title: Installing Trellis
author:
  - 'a:1:{i:0;s:25:"a:1:{i:0;s:8:"Ben Word";}";}'
post_date:
  - 'a:1:{i:0;s:37:"a:1:{i:0;s:19:"2015-10-15 12:20:35";}";}'
post_excerpt:
  - 'a:1:{i:0;s:17:"a:1:{i:0;s:0:"";}";}'
layout: doc
permalink:
  - 'a:1:{i:0;s:51:"a:1:{i:0;s:33:"/trellis/docs/installing-trellis/";}";}'
published: true
docs_project:
  - "19"
publish_to_discourse:
  - "0"
---
## Requirements

* Ansible >= 2.0.0.2 - [Install](http://docs.ansible.com/intro_installation.html) • [Docs](http://docs.ansible.com/) • [Windows docs](https://roots.io/trellis/docs/windows/)
* Virtualbox >= 4.3.10 - [Install](https://www.virtualbox.org/wiki/Downloads)
* Vagrant >= 1.5.4 - [Install](http://www.vagrantup.com/downloads.html) • [Docs](https://docs.vagrantup.com/v2/)
* vagrant-bindfs >= 0.3.1 - [Install](https://github.com/gael-ian/vagrant-bindfs#installation) • [Docs](https://github.com/gael-ian/vagrant-bindfs) (Windows users may skip this)
* vagrant-hostmanager - [Install](https://github.com/smdahlen/vagrant-hostmanager#installation) • [Docs](https://github.com/smdahlen/vagrant-hostmanager)

## Installation

1. Download/fork/clone the [Trellis repository](https://github.com/roots/trellis) to your local machine
2. Run `ansible-galaxy install -r requirements.yml` inside your Trellis directory to install external Ansible roles/packages
3. Download/fork/clone [Bedrock](https://github.com/roots/bedrock) or have an existing Bedrock-based site ready

You should now have the following directories at the same level somewhere:

```plain
example.com/    - Primary folder for the project
├── trellis/    - Your clone of the Trellis repository
└── site/       - A Bedrock-based site
```

- You **do not** need a configured `.env` file. Trellis will automatically create and configure one.

You can find a complete working example in the [Roots Example Project](https://github.com/roots/roots-example-project.com) repository.