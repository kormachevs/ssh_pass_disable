# ssh_pass_disable
## Отключение авторизации по ssh паролю

sshd_config

//# If you just want the PAM account and session checks to run without
//# PAM authentication, then enable this but set PasswordAuthentication
//# and ChallengeResponseAuthentication to 'no'.

Использование:

    git clone https://github.com/kormachevs/ssh_pass_disable.git
    cd ./ssh_pass_disable

Поправить hosts, заполнить своими данными...
Запуск:

    ansible-playbook ssh_disable_pass.yaml

Будет отключена авторизация только на тех хостак, куда есть доступ по ключу и ansible_ssh_pass не определена. 
____
