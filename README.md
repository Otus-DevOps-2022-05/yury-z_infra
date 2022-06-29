# yury-z_infra
yury-z Infra repository

setupvpn.sh адаптирован под запуск из РФ

Подключение в одну команду:
ssh -i ~/.ssh/appuser -J appuser@51.250.86.108 appuser@10.128.0.21


Дополнительное задание:
~/.ssh/config
Host someinternalhost
	Hostname 10.128.0.21
	ProxyJump appuser@51.250.86.108
	User appuser
	IdentityFile ~/.ssh/appuser

bastion_IP = 51.250.86.108
someinternalhost_IP = 10.128.0.21
