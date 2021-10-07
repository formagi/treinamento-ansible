# Treinamento Descomplicando o Ansible - LinuxTips

Repositório para armazenar e apresentar conteúdo elaborado com o apoio do treinamento [Descomplicando o Ansible](https://www.linuxtips.io/products/treinamento-descomplicando-o-ansible?variant=40789475426453), da [LinuxTips](https://www.linuxtips.io/) - Instrutor [Jeferson Fernando](https://www.instagram.com/badtux_/)

## Roles deste projeto:
* [provisioning-aws](./roles/provisioning-aws/README.md): Criar as instâncias na AWS
* [install-k8s](./roles/install-k8s/README.md): Instalar Docker + K8s
* [create-cluster](./roles/create-cluster/README.md): Iniciar cluster no K8s
* [join-workers](./roles/join-workers/README.md): Agregar os workers ao cluster
* [install-helm](./roles/install-helm/README.md): Instalar helm no k8s-master
* [install-monit-tools](./roles/install-monit-tools/README.md): Instalar [stack prometheus]()
* [deploy-app](./roles/deploy-app/README.md): Executar o deploy de uma aplicação no K8s

## Para utilizar este playbook:
Lembre que você precisará de Pythone Ansible instalados no seu host.

Além do mais, você precisará também das seguintes dependências no Python:
```bash
python3 -m pip install botocore
python3 -m pip install boto3
```

Também será necessário configurar as suas credenciais de acesso à AWS.

Para tal, consulte a [documentação da própria AWS](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html)

Para executar o playbook, basta:
```bash
ansible-playbook main.yml
```
## Observações:
Use deste repositório para aprender. Todo o conteúdo foi construído enquanto eu aprendia sobre o assunto, junto com o mestre Jeferson.

Outro ponto a observar é que nem todas as documentações deste projeto estão finalizadas, serão feitas ao longo do tempo, de forma bem detalhada.

Fique a vontade para me procurar em caso de dúvidas: alan@formagi.com.br
### License: 
[MIT](https://choosealicense.com/licenses/mit/)
