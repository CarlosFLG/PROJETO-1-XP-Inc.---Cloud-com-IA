# PROJETO-1-XP-Inc.---Cloud-com-IA
PROEJTO 1 PARA XP Inc. - Cloud com Inteligência Artificial
# Laboratório: Criação de Máquina Virtual no Azure

Este repositório contém documentação detalhada sobre o processo de criação e configuração de uma máquina virtual Windows no Microsoft Azure, como parte do curso "XP Inc. - Cloud com Inteligência Artificial" da DIO.

## Índice
1. [Introdução ao Azure](#introdução-ao-azure)
2. [Preparação do Ambiente](#preparação-do-ambiente)
3. [Criação da Máquina Virtual](#criação-da-máquina-virtual)
4. [Configuração de Rede](#configuração-de-rede)
5. [Conexão à VM](#conexão-à-vm)
6. [Considerações de Segurança](#considerações-de-segurança)
7. [Gerenciamento de Custos](#gerenciamento-de-custos)
8. [Dicas e Boas Práticas](#dicas-e-boas-práticas)

## Introdução ao Azure

O Microsoft Azure é uma plataforma de computação em nuvem que oferece uma ampla gama de serviços, incluindo máquinas virtuais, bancos de dados, armazenamento, IA e muito mais. Neste laboratório, foco na criação de uma máquina virtual Windows.

## Preparação do Ambiente

Antes de criar uma VM, é necessário:
- Ter uma conta Azure ativa
- Entender conceitos básicos como grupos de recursos e regiões
- Planejar os recursos necessários (tamanho da VM, sistema operacional, etc.)

## Criação da Máquina Virtual

### Passo 1: Acessar o Portal Azure
![image](https://github.com/user-attachments/assets/146c2ae5-d04e-4d75-acbd-b894e79e240c)
Guia: Criação de VM no Azure e Documentação no GitHub
Etapa 1: Acessar o Portal Azure

Acesse o portal Azure em portal.azure.com
Faça login com suas credenciais da conta que você já criou

### Passo 2: Iniciar a Criação da VM
No portal Azure, clique em "Criar um recurso" no canto superior esquerdo
Procure por "Máquina Virtual" na barra de pesquisa e selecione esta opção
Clique em "Criar" para iniciar o processo de criação da VM
Na aba "Básico", preencha as informações:

Assinatura: Selecione sua assinatura Azure
Grupo de recursos: Crie um novo (ex: "lab-vm-resource-group")
Nome da máquina virtual: Escolha um nome único (ex: "vm-windows-lab")
Região: Selecione a região mais próxima (ex: Brazil South)
Opções de disponibilidade: Nenhuma redundância de infraestrutura
Tipo de segurança: Standard
Imagem: Windows 10/11 ou Windows Server 2019/2022
Tamanho: Standard_B2s (2vCPUs, 4GB RAM) ou outro tamanho básico
Nome de usuário: Crie um nome de usuário para acesso
Senha: Defina uma senha forte
Portas de entrada públicas: Permitir RDP (3389)


Na aba "Discos":

Tipo de disco do SO: SSD Standard
Mantenha as configurações padrão para os outros campos


Na aba "Rede":

Rede virtual: Mantenha a rede padrão criada automaticamente
Sub-rede: Mantenha a opção padrão
IP público: Criar novo
Grupo de segurança de rede: Básico
Selecione as portas de entrada: RDP (3389)


Nas abas "Gerenciamento", "Avançado" e "Tags":

Mantenha as configurações padrão


Na aba "Revisar + criar":

Revise todas as configurações
Clique em "Criar"


Aguarde a implantação da VM (pode levar alguns minutos)

![image](https://github.com/user-attachments/assets/62eee80a-1bc7-46dc-bd39-bdae631f66c3)


### Passo 3: Configurações Básicas


### Passo 4: Configuração de Discos


### Passo 5: Revisão e Criação


## Configuração de Rede

Descreva como a rede foi configurada, incluindo:
- Rede virtual
- Sub-rede
- IP público
- Grupo de segurança de rede
- Regras de entrada/saída
- ![image](https://github.com/user-attachments/assets/261a36b8-a60c-48ff-9db0-ba1227b5730e)


## Conexão à VM
Conectar-se à Máquina Virtual

Após a criação, vá para o recurso da VM
Clique em "Conectar" no menu à esquerda
Selecione "RDP" e faça download do arquivo RDP
Abra o arquivo e insira suas credenciais quando solicitado
Explore a máquina virtual para verificar se está funcionando corretamente

Detalhe como se conectar à VM usando RDP:
- Download do arquivo RDP
- Processo de autenticação
- Solução de problemas comuns de conexão

- ![image](https://github.com/user-attachments/assets/a5edc6da-7a5a-46eb-bce7-0f8a3970645d)


## Considerações de Segurança

Liste boas práticas de segurança para VMs no Azure:
- Atualizações regulares
- Configuração de firewall
- Uso de senhas fortes
- Princípio do menor privilégio

## Gerenciamento de Custos

Dicas para otimizar custos:
- Desligar VMs quando não estão em uso
- Escolher o tamanho adequado
- Usar orçamentos e alertas
- Reservas de instância para uso de longo prazo

## Dicas e Boas Práticas

Compartilhe insights e dicas aprendidas durante o processo:
- Backups regulares
- Monitoramento de desempenho
- Escalabilidade
- Automação de tarefas rotineiras

---

Projeto desenvolvido como parte do curso "XP Inc. - Cloud com Inteligência Artificial" da DIO.
