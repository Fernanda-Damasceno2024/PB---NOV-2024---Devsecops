# Atividade com monitoramento Nginx - Compass UOL | Atividade Prática 1 #PB - Novembro 2024 | DevSecOps
Atividade devsecops - Linux e AWS na prática

**1. Instalação do WSL no Windows**

Para instalar o WSL (Subsistema do Windows para Linux) no Windows, siga o guia abaixo. Certifique-se de que seu sistema operacional seja Windows 10 (versão 2004 ou superior) ou Windows 11.

**2. Ative o WSL**

Abra o Prompt de Comando ou PowerShell como administrador.
Clique com o botão direito no menu Iniciar e escolha Prompt de Comando (Admin) ou Windows PowerShell (Admin).
Digite o seguinte comando e pressione Enter:

wsl --install

Este comando:
Ativa os componentes necessários do WSL.
Instala a última versão do WSL 2.

**3. Reinicie o computador**

Após a execução do comando acima, reinicie seu computador se solicitado.

**4. Escolher uma Distribuição Linux:**

Após reiniciar o sistema, acesse a Microsoft Store e selecione uma distribuição Linux, como o Ubuntu 20.04 LTS.
Configuração Inicial do WSL:

Após a instalação, abra a distribuição Linux instalada (como o Ubuntu) e configure o nome de usuário e senha para o ambiente Linux.

Após atualizar o Sistema WSL:

No terminal da distribuição Linux (por exemplo, Ubuntu), execute os seguintes comandos para atualizar:

sudo apt update
sudo apt upgrade

**5. Criar uma instância EC2 na AWS**

Entre na console AWS, para criar uma instância Ec2

Na Console da AWS, acesse EC2 > Launch Instance.
Selecione em  imagens de aplicativos e sistemas operacionais (Amazon Machine Image), 
O sistema Linux ubuntu.
Escolha o tipo de instância, por exemplo, t2.micro (instância gratuita).
Crie ou selecione em "Key Pair" um par de chaves para acessar a instância.
No "Security Group", permita tráfego nas portas 22 (SSH) e 80 (HTTP).

**6. Passo a Passo para Instalar o Nginx em uma Instância EC2**

Após a criação da instância, obtenha o IP público da mesma.

No terminal com o WSL, conecte-se via SSH com o comando:

ssh -i parchaves ec2-user@ec2-44-200-246-186.compute-1.amazonaws.com

Atualize os pacotes do sistema
Após conectar-se, atualize os pacotes instalados no sistema:

sudo yum update -y 

**7. Instale o Nginx**

Execute o comando apropriado para instalar o Nginx:

sudo yum install nginx -y

Após a instalação, inicie o serviço do Nginx:

sudo systemctl start nginx



Após alterar a configuração, reinicie o Nginx:

sudo systemctl restart nginx




