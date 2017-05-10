# Splunk / Parallel Piper Playbook

Ansible Playbook for an all-in-one Parallel Piper / Splunk deployment. Parallel Piper is a nice little demo for Splunks HTTP Event Collector (HEC). It is a simple mobile web app that measures device motion and sends an event with the intensity of the motion to Splunk via HEC.

## Prerequisites

* Ansible installation (Ubuntu: `sudo apt install ansible` / Mac OS: `brew install ansible`)
* SSH access to a fresh Debian/Ubuntu server

## Playbook Usage

Install required roles from Ansible Galaxy

```sh
sudo ansible-galaxy install -r requirements.yml
```

Run playbook

```sh
ansible-playbook aio_install.yml -i "<insert_your_fqdn_here>,"
````

---

Thomas Redmer (2017)
