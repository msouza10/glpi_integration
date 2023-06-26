# Integração Zabbix-GLPi :rocket:

[![Zabbix Version](https://img.shields.io/badge/Zabbix-6.0-blue.svg)](https://www.zabbix.com/)
[![GLPi Version](https://img.shields.io/badge/GLPi-<VERSÃO>-blue.svg)](https://glpi-project.org/)

Este projeto implementa uma integração entre o Zabbix e o GLPi, permitindo a criação automática de tickets no GLPi com base em eventos do Zabbix. O código utilizado como base para essa integração foi obtido do repositório oficial do Zabbix. :clipboard:

## Como funciona? :gear:

A integração é realizada por meio de um webhook no Zabbix, que chama um script personalizado para processar os eventos e realizar a criação dos tickets no GLPi. O script utiliza a linguagem JavaScript e é executado dentro do ambiente do Zabbix. :computer:

## Como utilizar? :wrench:

1. Certifique-se de ter o Zabbix e o GLPi configurados e em execução.
2. Faça o download do código do Zabbix utilizado como base para essa integração: [media_glpi.yaml](https://git.zabbix.com/projects/ZBX/repos/zabbix/raw/templates/media/glpi/media_glpi.yaml?at=refs%2Fheads%2Frelease%2F6.0).
3. Realize as configurações necessárias no Zabbix para adicionar o webhook e vinculá-lo aos eventos desejados.
4. Configure os parâmetros do GLPi no arquivo `media_glpi.yaml`, como a URL do GLPi e o token de autenticação.
5. Personalize o script JavaScript de acordo com as necessidades específicas da sua integração.
6. Importe o arquivo `media_glpi.yaml` no Zabbix.
7. Teste a integração criando eventos no Zabbix e verificando a criação dos tickets no GLPi. :test_tube:

## Licença :page_with_curl:

Este projeto está licenciado sob a [MIT License](LICENSE).

## Créditos :clap:

Este projeto foi baseado no código fornecido pelo Zabbix. Você pode encontrar o código original [aqui](https://git.zabbix.com/projects/ZBX/repos/zabbix/raw/templates/media/glpi/media_glpi.yaml?at=refs%2Fheads%2Frelease%2F6.0). :link:

