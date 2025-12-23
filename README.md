Mini-Projeto – Administração de Sistemas

Autores: Rodrigo de Jesus Marques (127829) e João Botelho (126991)
Curso: Redes e Sistemas Informáticos – ESTGA, Universidade de Aveiro
Data: 20/12/2025

Descrição do Projeto

Este projeto demonstra a automação de infraestrutura e configuração de serviços na Microsoft Azure, utilizando Terraform para provisionamento e Ansible para configuração.

Exercício 1: Criação de uma máquina virtual com um servidor web Nginx e uma página customizada (index.html).

Pré-requisitos

Para executar o projeto corretamente, é necessário:
 - Terraform instalado
 - Ansible instalado
 - Conta Azure configurada
 - Azure CLI autenticado
 - Permissões para criar recursos na Azure
 - Chave SSH (RSA) no ambiente local com permissões 600

Observação: Escolher uma região elegível na Azure para criar a VM, conforme definido no main.tf.

Passos para Executar
1. Inicializar Terraform:
terraform init

2. Validar plano de criação:
terraform plan

3. Aplicar o plano:
terraform apply

4. Alterar o IP público no ansible/inventory.ini para o da VM criada.

5. Executar o playbook Ansible:
ansible-playbook -i ansible/inventory.ini ansible/playbook.yml

