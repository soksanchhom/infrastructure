<h1 align="center">
  Test Task Infrastructure
</h1>

## Step in main.yml file

- Install Docker via geerlingguy.docker
- Install git
- Clone  project from repo https://github.com/soksanchhom/test-task.git
- Build Image via Dockerfile in repo
- Running Container with built image

<h4>If you doesn't have Ansible in your machine, please install via below command</h4>
<p>How to install Ansible</p>

```
sudo pip install ansible
```

<p>Install Ansible geerlingguy.docker role</p>

```
ansible-galaxy install geerlingguy.docker
```

<h4>How To Run Ansible</h4>

Before running main.yml, you have set variable value in main.yml or you can skip it
```
  - port: 8000
```
Note: Port 80 is already running in server, it won't running if we choose duplicate port.

<p>Then Running command below to run Ansible</p>

```
ansible-playbook -i hosts main.yml
```
<h4>Test Result on Server</h4>

http://51.15.126.60:port/timezones
